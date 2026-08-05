---
title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
  interactive message passing for molecules'
arxiv_id: '2210.16518'
source_url: ''
authors:
- name: Yusong Wang
  orcid: null
  s2_author_id: '2130355145'
  s2_url: null
- name: Shaoning Li
  orcid: null
  s2_author_id: '2118846263'
  s2_url: null
- name: Xinheng He
  orcid: null
  s2_author_id: '2116555201'
  s2_url: null
- name: Mingyu Li
  orcid: null
  s2_author_id: '2219645402'
  s2_url: null
- name: Zun Wang
  orcid: null
  s2_author_id: '2189440018'
  s2_url: null
- name: Nanning Zheng
  orcid: null
  s2_author_id: '2144620206'
  s2_url: null
- name: Bin Shao
  orcid: null
  s2_author_id: '2064567675'
  s2_url: null
- name: Tie-Yan Liu
  orcid: null
  s2_author_id: '2149579639'
  s2_url: null
- name: Tong Wang
  orcid: null
  s2_author_id: '2155339611'
  s2_url: null
published_date: Oct 29, 2022
published_date_iso: '2022-10-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Geometric deep learning has been revolutionizing the molecular modeling
  field. Despite the state-of-the-art neural network models are approaching ab initio
  accuracy for molecular property prediction, their applications, such as drug discovery
  and molecular dynamics (MD) simulation, have been hindered by insufficient utilization
  of geometric information and high computational costs. Here we propose an equivariant
  geometry-enhanced graph neural network called ViSNet, which elegantly extracts geometric
  features and efficiently models molecular structures with low computational costs.
  Our proposed ViSNet outperforms state-of-the-art approaches on multiple MD benchmarks,
  including MD17, revised MD17 and MD22, and achieves excellent chemical property
  prediction on QM9 and Molecule3D datasets. Additionally, ViSNet achieved the top
  winners of PCQM4Mv2 track in the OGB-LCS@NeurIPS2022 competition. Furthermore, through
  a series of simulations and case studies, ViSNet can efficiently explore the conformational
  space and provide reasonable interpretability to map geometric representations to
  molecular structures.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ViSNet
mrr: 0.0463
adjusted_mrr: 0.0309
mrr_dataset_count: 2
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
    value: 0.039
    std: null
    paper_value: 0.039
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
    protocol_note: Force MAE for Naphthalene
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
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
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 19
    paper_rank: 19
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
    value: 0.217
    std: null
    paper_value: 0.217
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
    protocol_note: Force MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.0502
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.1668
    has_value_note: false
    value_note: ''
    sort_value: 0.0502
    sort_std: null
    global_rank: 28
    paper_rank: 70
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.0507
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0507
    sort_std: null
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SpookyNet
    model_key: spookynet
    model_plain: SpookyNet
    value: 0.151
    std: null
    paper_value: 0.151
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.052
    at_pub_std: 0.001
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-05-01'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.099
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: 0.001
    value_gap_source_arxiv: '2105.00304'
    value_gap_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    value_gap_source_is_current_paper: false
    value_gap: 0.099
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: 0.001
    global_rank: 32
    paper_rank: 68
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    comparison_source_arxiv: '2105.00304'
    is_best: false
    is_std_outlier: false
  - model: ET
    model_key: et
    model_plain: ET
    value: 0.123
    std: null
    paper_value: 0.123
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2202.02541'
    at_pub_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    at_pub_source_date_iso: '2022-01-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2202.02541'
    value_gap_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    value_gap_source_is_current_paper: false
    value_gap: 0.07100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 30
    paper_rank: 63
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    comparison_source_arxiv: '2202.02541'
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 0.131
    std: null
    paper_value: 0.131
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.091
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
    value_gap: 0.07800000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 34
    paper_rank: 64
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
    is_best: false
    is_std_outlier: false
  - model: NequlP
    model_key: nequlp
    model_plain: NequlP
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BOTNet
    model_key: botnet
    model_plain: BOTNet
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.03
    at_pub_std: null
    at_pub_source_arxiv: '2205.06643'
    at_pub_source_title: The design space of E(3)-equivariant atom-centred interatomic
      potentials
    at_pub_source_date_iso: '2022-05-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.023
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to md17 (score=89)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UNiTE
    model_key: unite
    model_plain: UNiTE
    value: 0.055
    std: null
    paper_value: 0.055
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
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.055
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.055
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
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.204
    std: null
    paper_value: 0.204
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
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
    gap_vs_at_pub: 0.13999999999999999
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
    value_gap: 0.13999999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 42
    paper_rank: 70
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.167
    std: null
    paper_value: 0.167
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.063
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-11-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.10400000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.077
    true_std: null
    value_gap_source_arxiv: '2311.02124'
    value_gap_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    value_gap_source_is_current_paper: false
    value_gap: 0.09000000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.077
    sort_std: null
    global_rank: 45
    paper_rank: 69
    rank_delta: 24
    rank_delta_abs: 24
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
    value: 0.37
    std: null
    paper_value: 0.37
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 0.29
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 46
    paper_rank: 79
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: So3krates
    model_key: so3krates
    model_plain: So3krates
    value: 0.139
    std: null
    paper_value: 0.139
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
    protocol_note: Energy MAE for Aspirin
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2205.14276'
    at_pub_source_title: 'So3krates: Equivariant attention for interactions on arbitrary
      length-scales in molecular systems'
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08700000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.139
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.139
    sort_std: null
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    comparison_source_arxiv: '2205.14276'
    is_best: false
    is_std_outlier: false
  - model: ACE
    model_key: ace
    model_plain: ACE
    value: 0.141
    std: null
    paper_value: 0.141
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
    protocol_note: MAE for energy and forces on rMD17 molecules
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.141
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.141
    sort_std: null
    global_rank: 66
    paper_rank: 66
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
    is_best: true
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
    - 32.6
    - 29.7
    - 43.5
    - 6.32
    - 6.53
    - 7.56
    - 23.0
    - 24.6
    - 19.5
    - 1.21
    - 6.28
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
    paper_value: 32.6
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 32.581
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
    gap_vs_at_pub: 32.568000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    comparison_source_arxiv: '2110.01191'
    is_best: true
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
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    metric_values:
    - 31.1
    - 24.5
    - 44.9
    - 6.26
    - 6.33
    - 7.78
    - 22.0
    - 22.8
    - 18.9
    - 1.12
    - 6.36
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
    sort_value: 0.032
    sort_std: null
    true_value: 0.032
    true_std: null
    paper_value: 31.1
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 31.068
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.032
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 31.068
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
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
    global_rank: 6
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    metric_values:
    - 45.7
    - 12.0
    - 45.0
    - 5.85
    - 5.98
    - 7.35
    - 24.0
    - 27.6
    - 20.4
    - 1.28
    - 5.83
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
    sort_value: 0.046
    sort_std: null
    true_value: 0.046
    true_std: null
    paper_value: 45.7
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 45.654
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.046
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 45.654
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
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
    global_rank: 10
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - 63.0
    - 33.0
    - 235.0
    - 14.0
    - 14.0
    - 14.0
    - 33.0
    - 41.0
    - 34.0
    - 1.7
    - 19.0
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
    sort_value: 0.063
    sort_std: null
    true_value: 0.063
    true_std: null
    paper_value: 63.0
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 62.937
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.063
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 62.937
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Fast and Uncertainty-Aware Directional Message Passing
      for Non-Equilibrium Molecules
    comparison_source_arxiv: '2011.14115'
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: PaxNet
    model_key: paxnet
    model_plain: PaxNet
    metric_values:
    - 31.0
    - 10.8
    - 44.7
    - 5.9
    - 6.04
    - 7.14
    - 23.1
    - 22.8
    - 19.2
    - 1.17
    - 5.92
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
    sort_value: 31.0
    sort_std: null
    true_value: 31.0
    true_std: null
    paper_value: 31.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
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
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 24
  - model: ViSNet
    model_key: visnet
    model_plain: ViSNet
    metric_values:
    - 31.7
    - 9.5
    - 41.1
    - 4.23
    - 4.52
    - 5.86
    - 23.0
    - 17.3
    - 14.8
    - 1.56
    - 4.25
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
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 31.7
    sort_std: null
    true_value: 31.7
    true_std: null
    paper_value: 31.7
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
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
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 25
  - model: ComENet
    model_key: comenet
    model_plain: ComENet
    metric_values:
    - 32.4
    - 24.5
    - 45.2
    - 6.59
    - 6.86
    - 7.98
    - 24.0
    - 23.1
    - 19.8
    - 1.2
    - 6.82
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
    sort_value: 32.4
    sort_std: null
    true_value: 32.4
    true_std: null
    paper_value: 32.4
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_note: ''
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
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: ET
    model_key: et
    model_plain: ET
    metric_values:
    - 36.1
    - 11.0
    - 59.0
    - 6.15
    - 6.16
    - 7.62
    - 26.0
    - 20.3
    - 17.5
    - 1.84
    - 6.38
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
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 36.1
    sort_std: null
    true_value: 36.1
    true_std: null
    paper_value: 36.1
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_note: ''
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
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 29
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    metric_values:
    - 48.0
    - 29.0
    - 71.0
    - 11.0
    - 12.0
    - 12.0
    - 31.0
    - 29.0
    - 25.0
    - 1.55
    - 12.0
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
    sort_value: 48.0
    sort_std: null
    true_value: 48.0
    true_std: null
    paper_value: 48.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_note: ''
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
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 29, 2022
    date_display: Oct 2022
    date_iso: '2022-10-29'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 32
  metrics:
  - gap
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - U
  primary_metric: gap
  rank_metric: gap
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - mu
  - alpha
  - gap
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - zpve
  - U
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
single_proposed_model: ViSNet
main_figure: /figures/2210.16518/main_figure.jpegoptim.jpg
---

