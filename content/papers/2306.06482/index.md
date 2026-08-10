---
title: 'TensorNet: Cartesian Tensor Representations for Efficient Learning of Molecular
  Potentials'
arxiv_id: '2306.06482'
source_url: ''
authors:
- name: Guillem Simeon
  orcid: null
  s2_author_id: '103131925'
  s2_url: null
- name: G. D. Fabritiis
  orcid: null
  s2_author_id: '144186698'
  s2_url: null
published_date: Jun 10, 2023
published_date_iso: '2023-06-10'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: The development of efficient machine learning models for molecular systems
  representation is becoming crucial in scientific research. We introduce TensorNet,
  an innovative $O(3)$-equivariant message-passing neural network architecture that
  leverages Cartesian tensor representations. By using Cartesian tensor atomic embeddings,
  feature mixing is simplified through matrix product operations. Furthermore, the
  cost-effective decomposition of these tensors into rotation group irreducible representations
  allows for the separate processing of scalars, vectors, and tensors when necessary.
  Compared to higher-rank spherical tensor models, TensorNet demonstrates state-of-the-art
  performance with significantly fewer parameters. For small molecule potential energies,
  this can be achieved even with a single interaction layer. As a result of all these
  properties, the model's computational cost is substantially decreased. Moreover,
  the accurate prediction of vector and tensor molecular quantities on top of potential
  energies and forces is possible. In summary, TensorNet's framework opens up a new
  space for the design of state-of-the-art equivariant models.
codebase_url: https://github.com/torchmd/torchmd-net
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TensorNet
- TensorNet 1L (535k)
- TensorNet 2L (770k)
mrr: 0.0357
adjusted_mrr: 0.0119
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
    value: 0.03
    std: null
    paper_value: 0.03
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
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: botnet
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
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
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.0293
    has_value_note: false
    value_note: ''
    sort_value: 0.0007
    sort_std: null
    global_rank: 5
    paper_rank: 27
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
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
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: nequip
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
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
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.0391
    has_value_note: false
    value_note: ''
    sort_value: 0.0009
    sort_std: null
    global_rank: 7
    paper_rank: 38
    rank_delta: 31
    rank_delta_abs: 31
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
    value: 0.2
    std: null
    paper_value: 0.2
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 17.9
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: allegro
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 2.3
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 2.0999999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0046
    true_std: null
    value_gap_source_arxiv: '2407.02263'
    value_gap_source_title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform
      for Machine Learning Force Fields'
    value_gap_source_is_current_paper: false
    value_gap: 0.19540000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.0046
    sort_std: null
    global_rank: 14
    paper_rank: 98
    rank_delta: 84
    rank_delta_abs: 84
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    comparison_source_arxiv: '2304.04757'
    is_best: false
    is_std_outlier: false
  - model: TensorNet 2L (770k)
    model_key: tensornet 2l (770k)
    model_plain: TensorNet 2L (770k)
    value: 0.02
    std: null
    paper_value: 0.02
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-10'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.02
    true_std: null
    value_gap_source_arxiv: '2306.06482'
    value_gap_source_title: 'TensorNet: Cartesian Tensor Representations for Efficient
      Learning of Molecular Potentials'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.02
    sort_std: null
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TensorNet 1L (535k)
    model_key: tensornet 1l (535k)
    model_plain: TensorNet 1L (535k)
    value: 0.03
    std: null
    paper_value: 0.03
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-10'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.03
    true_std: null
    value_gap_source_arxiv: '2306.06482'
    value_gap_source_title: 'TensorNet: Cartesian Tensor Representations for Efficient
      Learning of Molecular Potentials'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.03
    sort_std: null
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MACE
    model_key: mace
    model_plain: MACE
    value: 0.4
    std: null
    paper_value: 0.4
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
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: mace
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 10, 2023
    date_display: Jun 2023
    date_iso: '2023-06-10'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 2.2
    at_pub_std: null
    at_pub_source_arxiv: '2304.04757'
    at_pub_source_title: A new perspective on building efficient and expressive 3D
      equivariant graph neural networks
    at_pub_source_date_iso: '2023-04-07'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 1.8000000000000003
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0507
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.3493
    has_value_note: false
    value_note: ''
    sort_value: 0.0507
    sort_std: null
    global_rank: 48
    paper_rank: 109
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    comparison_source_arxiv: '2304.04757'
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
main_figure: /figures/2306.06482/main_figure.jpegoptim.jpg
---

