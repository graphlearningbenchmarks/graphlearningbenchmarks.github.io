---
title: On the Completeness of Invariant Geometric Deep Learning Models
arxiv_id: '2402.04836'
source_url: ''
authors:
- name: Zian Li
  orcid: null
  s2_author_id: '2255313980'
  s2_url: null
- name: Xiyuan Wang
  orcid: null
  s2_author_id: '2167480960'
  s2_url: null
- name: Shijia Kang
  orcid: null
  s2_author_id: '2283263791'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '2264103931'
  s2_url: null
published_date: Feb 7, 2024
published_date_iso: '2024-02-07'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Invariant models, one important class of geometric deep learning models,
  are capable of generating meaningful geometric representations by leveraging informative
  geometric features in point clouds. These models are characterized by their simplicity,
  good experimental results and computational efficiency. However, their theoretical
  expressive power still remains unclear, restricting a deeper understanding of the
  potential of such models. In this work, we concentrate on characterizing the theoretical
  expressiveness of a wide range of invariant models under fully-connected conditions.
  We first rigorously characterize the expressiveness of the most classic invariant
  model, message-passing neural networks incorporating distance (DisGNN), restricting
  its unidentifiable cases to be only highly symmetric point clouds. We then prove
  that GeoNGNN, the geometric counterpart of one of the simplest subgraph graph neural
  networks, can effectively break these corner cases'' symmetry and thus achieve E(3)-completeness.
  By leveraging GeoNGNN as a theoretical tool, we further prove that: 1) most subgraph
  GNNs developed in traditional graph learning can be seamlessly extended to geometric
  scenarios with E(3)-completeness; 2) DimeNet, GemNet and SphereNet, three well-established
  invariant models, are also all capable of achieving E(3)-completeness. Our theoretical
  results fill the gap in the expressive power of invariant models, contributing to
  a rigorous and comprehensive understanding of their capabilities.'
codebase_url: ''
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
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.012999999999999998
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
    value_gap: 0.0521
    has_value_note: false
    value_note: ''
    sort_value: 0.0009
    sort_std: null
    global_rank: 7
    paper_rank: 58
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
  - model: GeoNGNN
    model_key: geongnn
    model_plain: GeoNGNN
    value: 0.0014
    std: null
    paper_value: 0.0014
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Benzene Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0014
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0014
    sort_std: null
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.1591
    std: null
    paper_value: 0.1591
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.01
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.14909999999999998
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
    value_gap: 0.14909999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.01
    sort_std: null
    global_rank: 22
    paper_rank: 96
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: 2F-DisGNN
    model_key: 2f-disgnn
    model_plain: 2F-DisGNN
    value: 0.0465
    std: null
    paper_value: 0.0465
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0465
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0465
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
  - model: GemNet
    model_key: gemnet
    model_plain: GemNet
    value: 0.0502
    std: null
    paper_value: 0.0502
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.085
    at_pub_std: null
    at_pub_source_arxiv: '2210.16518'
    at_pub_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural network
      with vector-scalar interactive message passing for molecules'
    at_pub_source_date_iso: '2022-10-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.034800000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0502
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0502
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    comparison_source_arxiv: '2210.16518'
    is_best: false
    is_std_outlier: false
  - model: MACE
    model_key: mace
    model_plain: MACE
    value: 0.0507
    std: null
    paper_value: 0.0507
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.3
    at_pub_std: null
    at_pub_source_arxiv: '2310.16802'
    at_pub_source_title: 'From Molecules to Materials: Pre-training Large Generalizable
      Models for Atomic Property Prediction'
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.2493
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0507
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0507
    sort_std: null
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'From Molecules to Materials: Pre-training Large Generalizable
      Models for Atomic Property Prediction'
    comparison_source_arxiv: '2310.16802'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.1321
    std: null
    paper_value: 0.1321
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0681
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
    value_gap: 0.0681
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 64
    paper_rank: 90
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: DisGNN
    model_key: disgnn
    model_plain: DisGNN
    value: 0.1565
    std: null
    paper_value: 0.1565
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin Energy (E) test set MAE
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1565
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1565
    sort_std: null
    global_rank: 96
    paper_rank: 96
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
main_figure: /figures/2402.04836/main_figure.jpegoptim.jpg
---

