---
title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for QM9 Molecules'
arxiv_id: '2306.09549'
source_url: ''
authors:
- name: Haiyang Yu
  orcid: null
  s2_author_id: '2119316118'
  s2_url: null
- name: Meng Liu
  orcid: null
  s2_author_id: '38813990'
  s2_url: null
- name: Youzhi Luo
  orcid: null
  s2_author_id: '2004524780'
  s2_url: null
- name: A. Strasser
  orcid: null
  s2_author_id: '103618574'
  s2_url: null
- name: X. Qian
  orcid: null
  s2_author_id: '49258586'
  s2_url: null
- name: Xiaoning Qian
  orcid: null
  s2_author_id: '2067730514'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '1743600'
  s2_url: null
published_date: Jun 15, 2023
published_date_iso: '2023-06-15'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Supervised machine learning approaches have been increasingly used in accelerating
  electronic structure prediction as surrogates of first-principle computational methods,
  such as density functional theory (DFT). While numerous quantum chemistry datasets
  focus on chemical properties and atomic forces, the ability to achieve accurate
  and efficient prediction of the Hamiltonian matrix is highly desired, as it is the
  most important and fundamental physical quantity that determines the quantum states
  of physical systems and chemical properties. In this work, we generate a new Quantum
  Hamiltonian dataset, named as QH9, to provide precise Hamiltonian matrices for 999
  or 2998 molecular dynamics trajectories and 130,831 stable molecular geometries,
  based on the QM9 dataset. By designing benchmark tasks with various molecules, we
  show that current machine learning models have the capacity to predict Hamiltonian
  matrices for arbitrary molecules. Both the QH9 dataset and the baseline models are
  provided to the community through an open-source benchmark, which can be highly
  valuable for developing machine learning methods and accelerating molecular and
  materials design for scientific and technological applications. Our benchmark is
  publicly available at.
codebase_url: https://github.com/divelab/AIRS
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
  total: 3
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
    value: 8.312e-05
    std: null
    paper_value: 8.312e-05
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
    table_ref: text
    source_ref: yu2023efficient
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: reported as 83.12 x 10^-6 Eh in text for mixed MD17
    date: Jun 15, 2023
    date_display: Jun 2023
    date_iso: '2023-06-15'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-11'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.036e-05
    true_std: null
    value_gap_source_arxiv: '2506.09398'
    value_gap_source_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian
      Matrices via SO(2) Local Frames
    value_gap_source_is_current_paper: false
    value_gap: 7.276e-05
    has_value_note: false
    value_note: ''
    sort_value: 1.036e-05
    sort_std: null
    global_rank: 1
    paper_rank: 4
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
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
main_figure: /figures/2306.09549/main_figure.jpegoptim.jpg
---

