---
title: SchNet -- a deep learning architecture for molecules and materials
arxiv_id: '1712.06113'
source_url: ''
authors:
- name: K.T. Sch\"utt
  orcid: null
  s2_author_id: null
  s2_url: null
- name: H.E. Sauceda
  orcid: null
  s2_author_id: null
  s2_url: null
- name: P.-J. Kindermans
  orcid: null
  s2_author_id: null
  s2_url: null
- name: A. Tkatchenko
  orcid: null
  s2_author_id: null
  s2_url: null
- name: K.-R. M\"uller
  orcid: null
  s2_author_id: null
  s2_url: null
published_date: Dec 17, 2017
published_date_iso: '2017-12-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Deep learning has led to a paradigm shift in artificial intelligence, including
  web, text and image search, speech recognition, as well as bioinformatics, with
  growing impact in chemical physics. Machine learning in general and deep learning
  in particular is ideally suited for representing quantum-mechanical interactions,
  enabling to model nonlinear potential-energy surfaces or enhancing the exploration
  of chemical compound space. Here we present the deep learning architecture SchNet
  that is specifically designed to model atomistic systems by making use of continuous-filter
  convolutional layers. We demonstrate the capabilities of SchNet by accurately predicting
  a range of properties across chemical space for molecules and materials where our
  model learns chemically plausible embeddings of atom types across the periodic table.
  Finally, we employ SchNet to predict potential-energy surfaces and energy-conserving
  force fields for molecular dynamics simulations of small molecules and perform an
  exemplary study of the quantum-mechanical properties of C$_20$-fullerene that would
  have been infeasible with regular ab initio molecular dynamics.
codebase_url: https://github.com/atomistic-machine-learning/SchNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SchNet
mrr: 0.0217
adjusted_mrr: 0.0072
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
  - model: DTNN
    model_key: dtnn
    model_plain: DTNN
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schutt2017quantum
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test error for Benzene (N=1,000) trained on energy
    date: Dec 17, 2017
    date_display: Dec 2017
    date_iso: '2017-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-12-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.04
    true_std: null
    value_gap_source_arxiv: '1712.06113'
    value_gap_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.04
    sort_std: null
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDML
    model_key: gdml
    model_plain: GDML
    value: 0.07
    std: null
    paper_value: 0.07
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chmiela2017machine
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test error for Benzene (N=1,000) using forces-trained GDML
    date: Dec 17, 2017
    date_display: Dec 2017
    date_iso: '2017-12-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-12-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.07
    true_std: null
    value_gap_source_arxiv: '1712.06113'
    value_gap_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.07
    sort_std: null
    global_rank: 43
    paper_rank: 43
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
    protocol_note: Test error for Benzene (N=1,000) trained on energy+forces
    date: Dec 17, 2017
    date_display: Dec 2017
    date_iso: '2017-12-17'
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
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 46
    paper_rank: 46
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
single_proposed_model: SchNet
main_figure: /figures/1712.06113/main_figure.jpegoptim.jpg
---

