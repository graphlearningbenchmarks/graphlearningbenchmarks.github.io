---
title: Pre-training with fractional denoising to enhance molecular property prediction
arxiv_id: '2407.11086'
source_url: ''
authors:
- name: Yuyan Ni
  orcid: null
  s2_author_id: '2835047'
  s2_url: null
- name: Shikun Feng
  orcid: null
  s2_author_id: '2261357853'
  s2_url: null
- name: Xin Hong
  orcid: null
  s2_author_id: '2303474336'
  s2_url: null
- name: Yuancheng Sun
  orcid: null
  s2_author_id: '2311644134'
  s2_url: null
- name: Weiying Ma
  orcid: null
  s2_author_id: '2258072090'
  s2_url: null
- name: Zhiming Ma
  orcid: null
  s2_author_id: '2174196923'
  s2_url: null
- name: Qiwei Ye
  orcid: null
  s2_author_id: '2311501663'
  s2_url: null
- name: Yanyan Lan
  orcid: null
  s2_author_id: '2223114891'
  s2_url: null
published_date: Jul 14, 2024
published_date_iso: '2024-07-14'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Deep learning methods have been considered promising for accelerating molecular
  screening in drug discovery and material design. Due to the limited availability
  of labelled data, various self-supervised molecular pre-training methods have been
  presented. Although many existing methods utilize common pre-training tasks in computer
  vision and natural language processing, they often overlook the fundamental physical
  principles governing molecules. In contrast, applying denoising in pre-training
  can be interpreted as an equivalent force learning, but the limited noise distribution
  introduces bias into the molecular distribution. To address this issue, we introduce
  a molecular pre-training framework called fractional denoising, which decouples
  noise design from the constraints imposed by force learning equivalence. In this
  way, the noise becomes customizable, allowing for incorporating chemical priors
  to substantially improve the molecular distribution modelling. Experiments demonstrate
  that our framework consistently outperforms existing methods, establishing state-of-the-art
  results across force prediction, quantum chemical properties and binding affinity
  tasks. The refined noise design enhances force accuracy and sampling coverage, which
  contribute to the creation of physically consistent molecular representations, ultimately
  leading to superior predictive performance. Denoising methods introduce useful priors
  in pre-training methods for molecular property prediction, but chemically unaware
  noise can lead to inaccurate predictions in downstream tasks. A molecular pre-training
  framework that uses fractional denoising to improve molecular distribution modelling
  is proposed, resulting in better predictions in various property prediction tasks.
codebase_url: https://github.com/fengshikun/FradNMI
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Frad
mrr: 0.0238
adjusted_mrr: 0.0079
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
  - model: Frad
    model_key: frad
    model_plain: Frad
    value: 0.2476
    std: null
    paper_value: 0.2476
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
    protocol_note: Aspirin (Force) task using uniformly random splitting as per text.
    date: Jul 14, 2024
    date_display: Jul 2024
    date_iso: '2024-07-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.053
    at_pub_std: null
    at_pub_source_arxiv: '2311.02124'
    at_pub_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    at_pub_source_date_iso: '2023-11-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1946
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
    value_gap: 0.2045
    has_value_note: false
    value_note: ''
    sort_value: 0.0431
    sort_std: null
    global_rank: 42
    paper_rank: 102
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    comparison_source_arxiv: '2311.02124'
    is_best: false
    is_std_outlier: false
  - model: Coord
    model_key: coord
    model_plain: Coord
    value: 0.2497
    std: null
    paper_value: 0.2497
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: SheheryarZaidi2022PretrainingVD
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin (Force) task using uniformly random splitting as per text.
    date: Jul 14, 2024
    date_display: Jul 2024
    date_iso: '2024-07-14'
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
    gap_vs_at_pub: 0.1968
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
    value_gap: 0.1968
    has_value_note: false
    value_note: ''
    sort_value: 0.0529
    sort_std: null
    global_rank: 58
    paper_rank: 102
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    comparison_source_arxiv: '2311.02124'
    is_best: false
    is_std_outlier: false
  - model: pre-training by learning DFT forces
    model_key: pre-training by learning dft forces
    model_plain: pre-training by learning DFT forces
    value: 0.2361
    std: null
    paper_value: 0.2361
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
    protocol_note: Aspirin (Force) task using uniformly random splitting as per text.
    date: Jul 14, 2024
    date_display: Jul 2024
    date_iso: '2024-07-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2361
    true_std: null
    value_gap_source_arxiv: '2407.11086'
    value_gap_source_title: Pre-training with fractional denoising to enhance molecular
      property prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2361
    sort_std: null
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: training from scratch
    model_key: training from scratch
    model_plain: training from scratch
    value: 0.253
    std: null
    paper_value: 0.253
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
    protocol_note: Aspirin (Force) task using uniformly random splitting as per text.
    date: Jul 14, 2024
    date_display: Jul 2024
    date_iso: '2024-07-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.253
    true_std: null
    value_gap_source_arxiv: '2407.11086'
    value_gap_source_title: Pre-training with fractional denoising to enhance molecular
      property prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.253
    sort_std: null
    global_rank: 104
    paper_rank: 104
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
single_proposed_model: Frad
main_figure: /figures/2407.11086/main_figure.jpegoptim.jpg
---

