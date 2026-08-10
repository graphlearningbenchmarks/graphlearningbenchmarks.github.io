---
title: Molecule Graph Networks with Many-body Equivariant Interactions
arxiv_id: '2406.13265'
source_url: ''
authors:
- name: Zetian Mao
  orcid: null
  s2_author_id: '2307470435'
  s2_url: null
- name: Jiawen Li
  orcid: null
  s2_author_id: '2144508722'
  s2_url: null
- name: Chen Liang
  orcid: null
  s2_author_id: '2307562685'
  s2_url: null
- name: Diptesh Das
  orcid: null
  s2_author_id: '2307852612'
  s2_url: null
- name: Masato Sumita
  orcid: null
  s2_author_id: '2243442446'
  s2_url: null
- name: Koji Tsuda
  orcid: null
  s2_author_id: '2238629291'
  s2_url: null
published_date: Jun 19, 2024
published_date_iso: '2024-06-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Message passing neural networks have demonstrated significant efficacy in
  predicting molecular interactions. Introducing equivariant vectorial representations
  augments expressivity by capturing geometric data symmetries, thereby improving
  model accuracy. However, two-body bond vectors in opposition may cancel each other
  out during message passing, leading to the loss of directional information on their
  shared node. In this study, we develop Equivariant N-body Interaction Networks (ENINet)
  that explicitly integrates $l = 1$ equivariant many-body interactions to enhance
  directional symmetric information in the message passing scheme. We provided a mathematical
  analysis demonstrating the necessity of incorporating many-body equivariant interactions
  and generalized the formulation to $N$-body interactions. Experiments indicate that
  integrating many-body equivariant representations enhances prediction accuracy across
  diverse scalar and tensorial quantum chemical properties.
codebase_url: https://github.com/tsudalab/ENINet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ENINet
mrr: 0.0244
adjusted_mrr: 0.0081
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for force on Naphthalene
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
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
    paper_rank: 67
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: ENINet
    model_key: eninet
    model_plain: ENINet
    value: 0.043
    std: null
    paper_value: 0.043
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy on Ethanol
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.043
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.043
    sort_std: null
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 0.08
    std: null
    paper_value: 0.08
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
    protocol_note: MAE for energy on Benzene
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
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
    gap_vs_at_pub: 0.03
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
    value_gap: 0.03
    has_value_note: false
    value_note: ''
    sort_value: 0.05
    sort_std: null
    global_rank: 46
    paper_rank: 67
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: ET
    model_key: et
    model_plain: ET
    value: 0.052
    std: null
    paper_value: 0.052
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy on Ethanol
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2202.02541'
    at_pub_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    at_pub_source_date_iso: '2022-01-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NewtonNet
    model_key: newtonnet
    model_plain: NewtonNet
    value: 0.078
    std: null
    paper_value: 0.078
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy on Ethanol
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.061
    at_pub_std: 0.009
    at_pub_source_arxiv: '2108.02913'
    at_pub_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    at_pub_source_date_iso: '2021-08-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.017
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
    value_gap: 0.017
    has_value_note: false
    value_note: ''
    sort_value: 0.061
    sort_std: null
    global_rank: 63
    paper_rank: 67
    rank_delta: 4
    rank_delta_abs: 4
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
    value: 0.064
    std: null
    paper_value: 0.064
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
    protocol_note: MAE for energy on Ethanol
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
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
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.064
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip(l=1)
    model_plain: NequIP
    value: 0.097
    std: null
    paper_value: 0.097
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
    protocol_note: MAE for force on Naphthalene
    date: Jun 19, 2024
    date_display: Jun 2024
    date_iso: '2024-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.097
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.097
    sort_std: null
    global_rank: 74
    paper_rank: 74
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
single_proposed_model: ENINet
main_figure: /figures/2406.13265/main_figure.jpegoptim.jpg
---

