---
title: A new perspective on building efficient and expressive 3D equivariant graph
  neural networks
arxiv_id: '2304.04757'
source_url: ''
authors:
- name: Weitao Du
  orcid: null
  s2_author_id: '134861298'
  s2_url: null
- name: Yuanqi Du
  orcid: null
  s2_author_id: '93584228'
  s2_url: null
- name: Limei Wang
  orcid: null
  s2_author_id: '2109120459'
  s2_url: null
- name: Dieqiao Feng
  orcid: null
  s2_author_id: '7841666'
  s2_url: null
- name: Guifeng Wang
  orcid: null
  s2_author_id: '2118561363'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '1743600'
  s2_url: null
- name: Carla P. Gomes
  orcid: null
  s2_author_id: '2188778449'
  s2_url: null
- name: Zhixin Ma
  orcid: null
  s2_author_id: '2116416699'
  s2_url: null
published_date: Apr 7, 2023
published_date_iso: '2023-04-07'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Geometric deep learning enables the encoding of physical symmetries in modeling
  3D objects. Despite rapid progress in encoding 3D symmetries into Graph Neural Networks
  (GNNs), a comprehensive evaluation of the expressiveness of these networks through
  a local-to-global analysis lacks today. In this paper, we propose a local hierarchy
  of 3D isomorphism to evaluate the expressive power of equivariant GNNs and investigate
  the process of representing global geometric information from local patches. Our
  work leads to two crucial modules for designing expressive and efficient geometric
  GNNs; namely local substructure encoding (LSE) and frame transition encoding (FTE).
  To demonstrate the applicability of our theory, we propose LEFTNet which effectively
  implements these modules and achieves state-of-the-art performance on both scalar-valued
  and vector-valued molecular property prediction tasks. We further point out the
  design space for future developments of equivariant graph neural networks. Our codes
  are available at.
codebase_url: https://github.com/yuanqidu/LeftNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LEFTNet
mrr: 0.0085
adjusted_mrr: 0.0028
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 6.9
    std: null
    paper_value: 6.9
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
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.063
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 6.837000000000001
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
    value_gap: 6.890000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.01
    sort_std: null
    global_rank: 22
    paper_rank: 121
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
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
    protocol_note: per-atom forces prediction (Benzene)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    paper_rank: 105
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: GemNet
    model_key: gemnet
    model_plain: GemNet
    value: 0.145
    std: null
    paper_value: 0.145
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
    protocol_note: per-atom forces prediction (Benzene, WoFE=1000)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.085
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.059999999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0502
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0948
    has_value_note: false
    value_note: ''
    sort_value: 0.0502
    sort_std: null
    global_rank: 47
    paper_rank: 91
    rank_delta: 44
    rank_delta_abs: 44
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.147
    std: null
    paper_value: 0.147
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
    protocol_note: per-atom forces prediction (Benzene, WoFE=1000)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.209
    at_pub_std: null
    at_pub_source_arxiv: '2102.05013'
    at_pub_source_title: Spherical Message Passing for 3D Molecular Graphs
    at_pub_source_date_iso: '2021-02-09'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.062
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_gap_source_is_current_paper: false
    value_gap: 0.095
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 52
    paper_rank: 94
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Spherical Message Passing for 3D Molecular Graphs
    comparison_source_arxiv: '2102.05013'
    is_best: false
    is_std_outlier: false
  - model: SpookyNet
    model_key: spookynet
    model_plain: SpookyNet
    value: 0.258
    std: null
    paper_value: 0.258
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
    protocol_note: per-atom forces prediction
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.052
    at_pub_std: 0.001
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.20600000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2205.14276'
    value_gap_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    value_gap_source_is_current_paper: false
    value_gap: 0.20600000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 51
    paper_rank: 102
    rank_delta: 51
    rank_delta_abs: 51
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    comparison_source_arxiv: '2105.00304'
    is_best: false
    is_std_outlier: false
  - model: sGDML
    model_key: sgdml
    model_plain: sGDML
    value: 0.2
    std: null
    paper_value: 0.2
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: per-atom forces prediction (Benzene)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.06
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-03-06'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.14
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
    value_gap: 0.14
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
  - model: NewtonNet
    model_key: newtonnet
    model_plain: NewtonNet
    value: 0.348
    std: null
    paper_value: 0.348
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: per-atom forces prediction (Others)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.061
    at_pub_std: 0.009
    at_pub_source_arxiv: '2108.02913'
    at_pub_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    at_pub_source_date_iso: '2021-08-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.287
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.061
    true_std: null
    value_gap_source_arxiv: '2205.14276'
    value_gap_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    value_gap_source_is_current_paper: false
    value_gap: 0.287
    has_value_note: false
    value_note: ''
    sort_value: 0.061
    sort_std: null
    global_rank: 63
    paper_rank: 106
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    comparison_source_arxiv: '2108.02913'
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
    protocol_note: per-atom forces prediction (Benzene)
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    global_rank: 64
    paper_rank: 98
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: FCHL
    model_key: fchl
    model_plain: FCHL
    value: 6.2
    std: null
    paper_value: 6.2
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.182
    at_pub_std: null
    at_pub_source_arxiv: '2302.05743'
    at_pub_source_title: Is Distance Matrix Enough for Geometric Deep Learning?
    at_pub_source_date_iso: '2023-02-11'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-02-11'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 6.018
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.182
    true_std: null
    value_gap_source_arxiv: '2302.05743'
    value_gap_source_title: Is Distance Matrix Enough for Geometric Deep Learning?
    value_gap_source_is_current_paper: false
    value_gap: 6.018
    has_value_note: false
    value_note: ''
    sort_value: 0.182
    sort_std: null
    global_rank: 97
    paper_rank: 121
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Is Distance Matrix Enough for Geometric Deep Learning?
    comparison_source_arxiv: '2302.05743'
    is_best: false
    is_std_outlier: false
  - model: LEFTNet
    model_key: leftnet
    model_plain: LEFTNet
    value: 2.1
    std: null
    paper_value: 2.1
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
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.1
    true_std: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.1
    sort_std: null
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACE
    model_key: ace
    model_plain: ACE
    value: 6.1
    std: null
    paper_value: 6.1
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.1
    true_std: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.1
    sort_std: null
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ANI
    model_key: ani
    model_plain: ANI
    value: 16.6
    std: null
    paper_value: 16.6
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 16.6
    true_std: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 16.6
    sort_std: null
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAP
    model_key: gap
    model_plain: GAP
    value: 17.7
    std: null
    paper_value: 17.7
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
    table_ref: Table 5
    source_ref: batatiamace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Energy prediction (E) for Aspirin
    date: Apr 7, 2023
    date_display: Apr 2023
    date_iso: '2023-04-07'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 17.7
    true_std: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 17.7
    sort_std: null
    global_rank: 126
    paper_rank: 126
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
single_proposed_model: LEFTNet
main_figure: /figures/2304.04757/main_figure.jpegoptim.jpg
---

