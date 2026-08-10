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
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
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
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.27
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0007
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 2.2992999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.0007
    sort_std: null
    global_rank: 5
    paper_rank: 118
    rank_delta: 113
    rank_delta_abs: 113
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    comparison_source_arxiv: '2205.06643'
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
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 1.861
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0007
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 1.8993
    has_value_note: false
    value_note: ''
    sort_value: 0.0007
    sort_std: null
    global_rank: 6
    paper_rank: 116
    rank_delta: 110
    rank_delta_abs: 110
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
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.26
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0009
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 2.2990999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.0009
    sort_std: null
    global_rank: 7
    paper_rank: 118
    rank_delta: 111
    rank_delta_abs: 111
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
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
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.002
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 2.398
    has_value_note: false
    value_note: ''
    sort_value: 0.002
    sort_std: null
    global_rank: 9
    paper_rank: 119
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.271
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0046
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 2.2954
    has_value_note: false
    value_note: ''
    sort_value: 0.0046
    sort_std: null
    global_rank: 14
    paper_rank: 118
    rank_delta: 104
    rank_delta_abs: 104
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
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
    at_pub_value: 0.4
    at_pub_std: null
    at_pub_source_arxiv: '2306.06482'
    at_pub_source_title: 'TensorNet: Cartesian Tensor Representations for Efficient
      Learning of Molecular Potentials'
    at_pub_source_date_iso: '2023-06-10'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 1.8000000000000003
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
    global_rank: 48
    paper_rank: 118
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TensorNet: Cartesian Tensor Representations for Efficient
      Learning of Molecular Potentials'
    comparison_source_arxiv: '2306.06482'
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
    global_rank: 120
    paper_rank: 120
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
main_figure: /figures/2310.02970/main_figure.jpegoptim.jpg
---

