---
title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing in Position-Orientation
  Space
arxiv_id: '2310.02970'
source_url: ''
authors:
- name: E. Bekkers
  orcid: null
  s2_author_id: '2231179'
  s2_url: null
- name: Sharvaree P. Vadgama
  orcid: null
  s2_author_id: '101290348'
  s2_url: null
- name: Rob D. Hesselink
  orcid: null
  s2_author_id: '117361255'
  s2_url: null
- name: P. A. V. D. Linden
  orcid: null
  s2_author_id: '2057694734'
  s2_url: null
- name: David W. Romero
  orcid: null
  s2_author_id: '2064243209'
  s2_url: null
published_date: Oct 4, 2023
published_date_iso: '2023-10-04'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Based on the theory of homogeneous spaces we derive geometrically optimal
  edge attributes to be used within the flexible message-passing framework. We formalize
  the notion of weight sharing in convolutional networks as the sharing of message
  functions over point-pairs that should be treated equally. We define equivalence
  classes of point-pairs that are identical up to a transformation in the group and
  derive attributes that uniquely identify these classes. Weight sharing is then obtained
  by conditioning message functions on these attributes. As an application of the
  theory, we develop an efficient equivariant group convolutional network for processing
  3D point clouds. The theory of homogeneous spaces tells us how to do group convolutions
  with feature maps over the homogeneous space of positions $ ^3$, position and orientations
  $ ^3 S^2$, and the group $ (3)$ itself. Among these, $ ^3 S^2$ is an optimal choice
  due to the ability to represent directional information, which $ ^3$ methods cannot,
  and it significantly enhances computational efficiency compared to indexing features
  on the full $ (3)$ group. We support this claim with state-of-the-art results --in
  accuracy and speed-- on five different benchmarks in 2D and 3D, including interatomic
  potential energy prediction, trajectory forecasting in N-body systems, and generating
  molecules via equivariant diffusion models.
codebase_url: https://github.com/ebekkers/ponita
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PθNITA​ (fiber bundle)
- PΘNITA‑ (fiber bundle)
- PΘNITA‑ (point cloud)
- PΘNITA​ (point cloud)
mrr: 0.0435
adjusted_mrr: 0.0145
mrr_dataset_count: 1
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 2
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
  - model: ViSNet
    model_key: visnet
    model_plain: ViSNet
    value: 1.9
    std: null
    paper_value: 1.9
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
    source_ref: Wang 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.039
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 1.861
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.039
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 1.861
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 19
    paper_rank: 83
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: MACE
    model_key: mace
    model_plain: MACE
    value: 2.2
    std: null
    paper_value: 2.2
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
    source_ref: Batatia 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.0507
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.1493
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0507
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 2.1493
    has_value_note: false
    value_note: ''
    sort_value: 0.0507
    sort_std: null
    global_rank: 29
    paper_rank: 85
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 2.3
    std: null
    paper_value: 2.3
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
    source_ref: Batzner 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.26
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 2.247
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 34
    paper_rank: 85
    rank_delta: 51
    rank_delta_abs: 51
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
    is_best: false
    is_std_outlier: false
  - model: BOTNet
    model_key: botnet
    model_plain: BOTNet
    value: 2.3
    std: null
    paper_value: 2.3
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
    source_ref: Batatia 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.03
    at_pub_std: null
    at_pub_source_arxiv: '2205.06643'
    at_pub_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    at_pub_source_date_iso: '2022-05-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.27
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.247
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 36
    paper_rank: 85
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    comparison_source_arxiv: '2205.06643'
    is_best: false
    is_std_outlier: false
  - model: Allegro
    model_key: allegro
    model_plain: Allegro
    value: 2.3
    std: null
    paper_value: 2.3
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
    source_ref: Musaelian 2023
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.029
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.271
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.247
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 35
    paper_rank: 85
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: UNiTE
    model_key: unite
    model_plain: UNiTE
    value: 2.4
    std: null
    paper_value: 2.4
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
    source_ref: Qiao 2022
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.055
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.3449999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.055
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 2.3449999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.055
    sort_std: null
    global_rank: 38
    paper_rank: 86
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: PNITA
    model_key: pnita
    model_plain: PNITA
    value: 4.7
    std: null
    paper_value: 4.7
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
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for Energy (E) on Aspirin
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.7
    true_std: null
    value_gap_source_arxiv: '2310.02970'
    value_gap_source_title: Fast, Expressive SE$(n)$ Equivariant Networks through
      Weight-Sharing in Position-Orientation Space
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.7
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
- &id002
  dataset: QM9
  is_multi_metric: true
  rows:
  - model: PΘNITA​ (point cloud)
    model_key: pθnita​ (point cloud)
    model_plain: PΘNITA​ (point cloud)
    metric_values:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - 0.0115
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.0115
    sort_std: null
    true_value: 0.0115
    true_std: null
    paper_value: 0.0115
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.02970'
    value_gap_source_title: Fast, Expressive SE$(n)$ Equivariant Networks through
      Weight-Sharing in Position-Orientation Space
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2023
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: DimeNet++
    model_key: pf-gnn
    model_plain: DimeNet++
    metric_values:
    - 0.017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    published_venue: ''
    date: Jan 31, 2024
    date_display: Jan 2024
    date_iso: '2024-01-31'
    codebase_url: https://github.com/pfgnn/PF-GNN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: false
    sort_value: 0.017
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - 34.8
    - 8.02
    - 7.89
    - 8.11
    - 0.0249
    - 0.0249
    - 27.8
    - 19.7
    - 1.29
    - 0.0286
    - 0.0469
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.019
    sort_std: 0.001
    true_value: 0.019
    true_std: 0.001
    paper_value: 34.8
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 34.781
    value_gap_source_arxiv: '2401.17752'
    value_gap_source_title: 'PF-GNN: Differentiable particle filtering based approximation
      of universal graph representations'
    value_note: ''
    at_pub_value: 0.032
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-01-31'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 34.768
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2023
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    comparison_source_arxiv: '2110.01191'
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: DimeNet++
    model_key: molformer
    model_plain: DimeNet++
    metric_values:
    - 0.025
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    published_venue: ''
    date: Oct 4, 2021
    date_display: Oct 2021
    date_iso: '2021-10-04'
    codebase_url: https://github.com/smiles724/Molformer
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.025
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: PΘNITA‑ (point cloud)
    model_key: pθnita‑ (point cloud)
    model_plain: PΘNITA‑ (point cloud)
    metric_values:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - 1.29
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 1.29
    sort_std: null
    true_value: 1.29
    true_std: null
    paper_value: 1.29
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.02970'
    value_gap_source_title: Fast, Expressive SE$(n)$ Equivariant Networks through
      Weight-Sharing in Position-Orientation Space
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2023
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: PΘNITA‑ (fiber bundle)
    model_key: pθnita‑ (fiber bundle)
    model_plain: PΘNITA‑ (fiber bundle)
    metric_values:
    - null
    - null
    - null
    - null
    - null
    - null
    - 16.0
    - 14.5
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 16.0
    sort_std: null
    true_value: 16.0
    true_std: null
    paper_value: 16.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.02970'
    value_gap_source_title: Fast, Expressive SE$(n)$ Equivariant Networks through
      Weight-Sharing in Position-Orientation Space
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2023
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: PθNITA​ (fiber bundle)
    model_key: pθnita​ (fiber bundle)
    model_plain: PθNITA​ (fiber bundle)
    metric_values:
    - 30.4
    - 8.31
    - 8.67
    - 8.04
    - 0.00863
    - 0.0242
    - null
    - null
    - null
    - null
    - 0.0375
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 30.4
    sort_std: null
    true_value: 30.4
    true_std: null
    paper_value: 30.4
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2310.02970'
    value_gap_source_title: Fast, Expressive SE$(n)$ Equivariant Networks through
      Weight-Sharing in Position-Orientation Space
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2023
    date: Oct 4, 2023
    date_display: Oct 2023
    date_iso: '2023-10-04'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  metrics:
  - gap
  - U0
  - U
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - mu
  - alpha
  primary_metric: gap
  rank_metric: gap
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - U0
  - U
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - mu
  - alpha
  - gap
  metric: gap
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: MD17
      dataset_slug: md17
    - dataset: QM9
      dataset_slug: qm9
main_figure: /figures/2310.02970/main_figure.jpegoptim.jpg
---

