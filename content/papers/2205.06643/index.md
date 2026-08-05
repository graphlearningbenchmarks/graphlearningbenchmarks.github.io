---
title: The design space of E(3)-equivariant atom-centred interatomic potentials
arxiv_id: '2205.06643'
source_url: ''
authors:
- name: Ilyes Batatia
  orcid: null
  s2_author_id: '2040711516'
  s2_url: null
- name: Simon Batzner
  orcid: null
  s2_author_id: '96427180'
  s2_url: null
- name: D\'avid P\'eter Kov\'acs
  orcid: null
  s2_author_id: '2165311424'
  s2_url: null
- name: Albert Musaelian
  orcid: null
  s2_author_id: '103291062'
  s2_url: null
- name: Gregor N.\ C.\ Simm
  orcid: null
  s2_author_id: '46338741'
  s2_url: null
- name: Ralf Drautz
  orcid: null
  s2_author_id: '3411633'
  s2_url: null
- name: Christoph Ortner
  orcid: null
  s2_author_id: '2060586'
  s2_url: null
- name: Boris Kozinsky
  orcid: null
  s2_author_id: '51443274'
  s2_url: null
- name: G\'abor Cs\'anyi
  orcid: null
  s2_author_id: '2559761'
  s2_url: null
published_date: May 13, 2022
published_date_iso: '2022-05-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Molecular dynamics simulation is an important tool in computational materials
  science and chemistry, and in the past decade it has been revolutionized by machine
  learning. This rapid progress in machine learning interatomic potentials has produced
  a number of new architectures in just the past few years. Particularly notable among
  these are the atomic cluster expansion, which unified many of the earlier ideas
  around atom-density-based descriptors, and Neural Equivariant Interatomic Potentials
  (NequIP), a message-passing neural network with equivariant features that exhibited
  state-of-the-art accuracy at the time. Here we construct a mathematical framework
  that unifies these models: atomic cluster expansion is extended and recast as one
  layer of a multi-layer architecture, while the linearized version of NequIP is understood
  as a particular sparsification of a much larger polynomial model. Our framework
  also provides a practical tool for systematically probing different choices in this
  unified design space. An ablation study of NequIP, via a set of experiments looking
  at in- and out-of-domain accuracy and smooth extrapolation very far from the training
  data, sheds some light on which design choices are critical to achieving high accuracy.
  A much-simplified version of NequIP, which we call BOTnet (for body-ordered tensor
  network), has an interpretable architecture and maintains its accuracy on benchmark
  datasets. Batatia and colleagues introduce a computational framework that combines
  message-passing networks with the atomic cluster expansion architecture and incorporates
  a many-body description of the geometry of molecular structures. The resulting models
  are interpretable and accurate.'
codebase_url: https://github.com/gncs/botnet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BOTNet
mrr: 0.0278
adjusted_mrr: 0.0093
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
  is_multi_metric: true
  rows:
  - model: SliDe
    model_key: qhnet
    model_plain: SliDe
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
  - model: SliDe
    model_key: qhnetv2
    model_plain: SliDe
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
  - model: SliDe
    model_key: phisnet
    model_plain: SliDe
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
  - model: BOTNet
    model_key: botnet
    model_plain: BOTNet
    metric_values:
    - 0.03
    - 2.3
    - 8.5
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
    sort_value: 0.053
    sort_std: null
    true_value: 0.053
    true_std: null
    paper_value: 0.03
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.023
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
    insignificant_value_gap: true
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 36
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    metric_values:
    - 2.3
    - 2.3
    - 8.2
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
    sort_value: 0.053
    sort_std: null
    true_value: 0.053
    true_std: null
    paper_value: 2.3
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 2.247
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_note: ''
    at_pub_value: 0.348
    at_pub_std: null
    at_pub_source_arxiv: '2202.02541'
    at_pub_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    at_pub_source_date_iso: '2022-01-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 1.952
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 34
  - model: Linear ACE
    model_key: linear ace
    model_plain: Linear ACE
    metric_values:
    - null
    - 6.1
    - 17.9
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
    sort_value: 6.1
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 6.1
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 88
  - model: FCHL
    model_key: fchl
    model_plain: FCHL
    metric_values:
    - null
    - 6.2
    - 20.9
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 6.2
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 6.2
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 88
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    metric_values:
    - null
    - 6.9
    - 16.1
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
    sort_value: 6.9
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 6.9
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 45
  - model: sGDML
    model_key: sgdml
    model_plain: sGDML
    metric_values:
    - null
    - 7.2
    - 31.8
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 7.2
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 7.2
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 40
  - model: NewtonNet
    model_key: newtonnet
    model_plain: NewtonNet
    metric_values:
    - null
    - 7.3
    - 15.1
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
    sort_value: 7.3
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 7.3
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 41
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - null
    - 8.8
    - 21.6
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
    sort_value: 8.8
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 8.8
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 42
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - null
    - 16.0
    - 58.5
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
    sort_value: 16.0
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 16.0
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
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
  - model: GMsNN
    model_key: gmsnn
    model_plain: GMsNN
    metric_values:
    - null
    - 16.5
    - 29.9
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
    sort_value: 16.5
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 16.5
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 90
  - model: ANI
    model_key: ani
    model_plain: ANI
    metric_values:
    - null
    - 16.6
    - 40.6
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
    sort_value: 16.6
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 16.6
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 90
  - model: GAP
    model_key: gap
    model_plain: GAP
    metric_values:
    - null
    - 17.7
    - 44.9
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
    sort_value: 17.7
    sort_std: null
    true_value: null
    true_std: null
    paper_value: 17.7
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
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
    date: May 13, 2022
    date_display: May 2022
    date_iso: '2022-05-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 91
  metrics:
  - MAE
  - E
  - F
  primary_metric: MAE
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - E
  - F
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
single_proposed_model: BOTNet
main_figure: /figures/2205.06643/main_figure.jpegoptim.jpg
---

