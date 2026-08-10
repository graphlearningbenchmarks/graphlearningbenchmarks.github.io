---
title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and Crystalline
  Materials
arxiv_id: '2306.09375'
source_url: ''
authors:
- name: Shengchao Liu
  orcid: null
  s2_author_id: '1563693999'
  s2_url: null
- name: Weitao Du
  orcid: null
  s2_author_id: '134861298'
  s2_url: null
- name: Yanjing Li
  orcid: null
  s2_author_id: '2110500972'
  s2_url: null
- name: Zhuoxinran Li
  orcid: null
  s2_author_id: '2220238808'
  s2_url: null
- name: Zhiling Zheng
  orcid: null
  s2_author_id: '120964397'
  s2_url: null
- name: Chenru Duan
  orcid: null
  s2_author_id: '35473448'
  s2_url: null
- name: Zhiming Ma
  orcid: null
  s2_author_id: '2174196923'
  s2_url: null
- name: O. Yaghi
  orcid: null
  s2_author_id: '3563734'
  s2_url: null
- name: Anima Anandkumar
  orcid: null
  s2_author_id: '2047844'
  s2_url: null
- name: C. Borgs
  orcid: null
  s2_author_id: '1721812'
  s2_url: null
- name: J. Chayes
  orcid: null
  s2_author_id: '1695997'
  s2_url: null
- name: Hongyu Guo
  orcid: null
  s2_author_id: '1694050'
  s2_url: null
- name: Jian Tang
  orcid: null
  s2_author_id: '2115855484'
  s2_url: null
published_date: Jun 15, 2023
published_date_iso: '2023-06-15'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Artificial intelligence for scientific discovery has recently generated
  significant interest within the machine learning and scientific communities, particularly
  in the domains of chemistry, biology, and material discovery. For these scientific
  problems, molecules serve as the fundamental building blocks, and machine learning
  has emerged as a highly effective and powerful tool for modeling their geometric
  structures. Nevertheless, due to the rapidly evolving process of the field and the
  knowledge gap between science (, physics, chemistry, & biology) and machine learning
  communities, a benchmarking study on geometrical representation for such data has
  not been conducted. To address such an issue, in this paper, we first provide a
  unified view of the current symmetry-informed geometric methods, classifying them
  into three main categories: invariance, equivariance with spherical frame basis,
  and equivariance with vector frame basis. Then we propose a platform, coined Geom3D,
  which enables benchmarking the effectiveness of geometric strategies. Geom3D contains
  16 advanced symmetry-informed geometric representation models and 14 geometric pretraining
  methods over 46 diverse datasets, including small molecules, proteins, and crystalline
  materials. We hope that Geom3D can, on the one hand, eliminate barriers for machine
  learning researchers interested in exploring scientific problems; and, on the other
  hand, provide valuable guidance for researchers in computational chemistry, structural
  biology, and materials science, aiding in the informed selection of representation
  techniques for specific applications. The source code is available on the GitHub
  repository. =-1'
codebase_url: https://github.com/chao1224/Geom3D
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  is_multi_metric: true
  rows:
  - model: QHNet
    model_key: qhnet
    model_plain: QHNet
    metric_values:
    - 1.036e-05
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 1.036e-05
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
  - model: QHNetV2
    model_key: qhnetv2
    model_plain: QHNetV2
    metric_values:
    - 1.038e-05
    - null
    - null
    metric_stds:
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
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 1.038e-05
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
  - model: PhiSNet
    model_key: phisnet
    model_plain: PhiSNet
    metric_values:
    - 1.759e-05
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 1.759e-05
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
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    metric_values:
    - 0.936
    - 8.333
    - 23.769
    metric_stds:
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
    sort_value: 0.0009
    sort_std: null
    true_value: 0.0009
    true_std: null
    paper_value: 0.936
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.9351
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_note: ''
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.896
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: Allegro
    model_key: allegro
    model_plain: Allegro
    metric_values:
    - 0.029
    - 1.138
    - 3.405
    metric_stds:
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
    sort_value: 0.0046
    sort_std: null
    true_value: 0.0046
    true_std: null
    paper_value: 0.029
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.0244
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_note: ''
    at_pub_value: 0.2
    at_pub_std: null
    at_pub_source_arxiv: '2306.06482'
    at_pub_source_title: 'TensorNet: Cartesian Tensor Representations for Efficient
      Learning of Molecular Potentials'
    at_pub_source_date_iso: '2023-06-10'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.171
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    metric_values:
    - 0.315
    - 17.892
    - 3.042
    metric_stds:
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
    sort_value: 0.0047
    sort_std: 0.0002
    true_value: 0.0047
    true_std: 0.0002
    paper_value: 0.315
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.3103
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: GemNet-T
    model_key: gemnet-t
    model_plain: GemNet-T
    metric_values:
    - 0.007
    - 0.684
    - 0.558
    metric_stds:
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
    sort_value: 0.007
    sort_std: null
    true_value: 0.007
    true_std: null
    paper_value: 0.007
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_note: ''
    at_pub_value: 0.22
    at_pub_std: null
    at_pub_source_arxiv: '2102.05013'
    at_pub_source_title: Spherical Message Passing for 3D Molecular Graphs
    at_pub_source_date_iso: '2021-02-09'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.213
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    metric_values:
    - 0.01
    - 27.626
    - 0.572
    metric_stds:
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
    sort_value: 0.01
    sort_std: null
    true_value: 0.01
    true_std: null
    paper_value: 0.01
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_note: ''
    at_pub_value: 0.063
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.053
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: Equiformer
    model_key: equiformer
    model_plain: Equiformer
    metric_values:
    - 0.02
    - 0.308
    - 0.286
    metric_stds:
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
    sort_value: 0.02
    sort_std: null
    true_value: 0.02
    true_std: null
    paper_value: 0.02
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
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
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - 0.111
    - 0.475
    - 1.203
    metric_stds:
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
    sort_value: 0.05
    sort_std: null
    true_value: 0.05
    true_std: null
    paper_value: 0.111
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.061
    value_gap_source_arxiv: '1902.08408'
    value_gap_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    value_note: ''
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-02-22'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.061
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 46
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    metric_values:
    - 0.052
    - 0.244
    - 0.546
    metric_stds:
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
    sort_value: 0.052
    sort_std: null
    true_value: 0.052
    true_std: null
    paper_value: 0.052
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_note: ''
    at_pub_value: 0.147
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.095
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 52
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - 0.34
    - 4.168
    - 7.212
    metric_stds:
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
    sort_value: 0.064
    sort_std: null
    true_value: 0.064
    true_std: null
    paper_value: 0.34
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.276
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_note: ''
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.276
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 64
  - model: SEGNN
    model_key: segnn
    model_plain: SEGNN
    metric_values:
    - 0.13
    - 17.774
    - 9.003
    metric_stds:
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
    sort_value: 0.13
    sort_std: null
    true_value: 0.13
    true_std: null
    paper_value: 0.13
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
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
    published_venue: NeurIPS 2023
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 89
  metrics:
  - MAE
  - Energy
  - Force
  primary_metric: MAE
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - Energy
  - Force
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
main_figure: /figures/2306.09375/main_figure.jpegoptim.jpg
---

