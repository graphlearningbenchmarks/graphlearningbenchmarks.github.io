---
title: Graph Anisotropic Diffusion
arxiv_id: '2205.00354'
source_url: ''
authors:
- name: Ahmed A. A. Elhag
  orcid: null
  s2_author_id: '2164036742'
  s2_url: null
- name: Gabriele Corso
  orcid: null
  s2_author_id: '2164036816'
  s2_url: null
- name: Hannes Stärk
  orcid: null
  s2_author_id: '2164102905'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2060916506'
  s2_url: null
published_date: Apr 30, 2022
published_date_iso: '2022-04-30'
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Traditional Graph Neural Networks (GNNs) rely on message passing, which
  amounts to permutation-invariant local aggregation of neighbour features. Such a
  process is isotropic and there is no notion of `direction' on the graph. We present
  a new GNN architecture called Graph Anisotropic Diffusion. Our model alternates
  between linear diffusion, for which a closed-form solution is available, and local
  anisotropic filters to obtain efficient multi-hop anisotropic kernels. We test our
  model on two common molecular property prediction benchmarks (ZINC and QM9) and
  show its competitive performance.
codebase_url: https://github.com/Ahmed-A-A-Elhag/GAD
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- new way to perform isotropic diffusion on graphs
mrr: 0.0244
adjusted_mrr: 0.0081
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
    metric_stds:
    - 0.001
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
    - 0.019
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
    is_baseline: true
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
    global_rank: 2
    is_best: true
    sort_value: 0.019
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
    metric_stds:
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
  - model: new way to perform isotropic diffusion on graphs
    model_key: new way to perform isotropic diffusion on graphs
    model_plain: new way to perform isotropic diffusion on graphs
    metric_values:
    - 96.8
    - 0.338
    - 0.24
    - 64.3
    - 63.0
    - 4.84
    - null
    metric_stds:
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
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 96.8
    sort_std: null
    true_value: 96.8
    true_std: null
    paper_value: 96.8
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2205.00354'
    value_gap_source_title: Graph Anisotropic Diffusion
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-30'
    value_gap_source_date_label: ICLR 2022
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
    published_venue: ICLR 2022
    date: Apr 30, 2022
    date_display: Apr 2022
    date_iso: '2022-04-30'
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
  - model: GAD-s
    model_key: gad-s
    model_plain: GAD-s
    metric_values:
    - 96.8
    - 0.338
    - 0.24
    - 64.3
    - 63.0
    - 4.84
    - 16.5
    metric_stds:
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
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 96.8
    sort_std: null
    true_value: 96.8
    true_std: null
    paper_value: 96.8
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2205.00354'
    value_gap_source_title: Graph Anisotropic Diffusion
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-30'
    value_gap_source_date_label: ICLR 2022
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
    published_venue: ICLR 2022
    date: Apr 30, 2022
    date_display: Apr 2022
    date_iso: '2022-04-30'
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
  - model: DGN
    model_key: dgn
    model_plain: DGN
    metric_values:
    - 99.2
    - 0.354
    - 0.25
    - 71.1
    - 68.0
    - 6.03
    - 17.2
    metric_stds:
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
    sort_value: 99.2
    sort_std: null
    true_value: 99.2
    true_std: null
    paper_value: 99.2
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2205.00354'
    value_gap_source_title: Graph Anisotropic Diffusion
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-30'
    value_gap_source_date_label: ICLR 2022
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
    published_venue: ICLR 2022
    date: Apr 30, 2022
    date_display: Apr 2022
    date_iso: '2022-04-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 43
  - model: PNA
    model_key: pna
    model_plain: PNA
    metric_values:
    - 100.2
    - 0.365
    - 0.255
    - 71.5
    - 70.1
    - 6.57
    - 18.3
    metric_stds:
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
    sort_value: 100.2
    sort_std: null
    true_value: 100.2
    true_std: null
    paper_value: 100.2
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2205.00354'
    value_gap_source_title: Graph Anisotropic Diffusion
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-30'
    value_gap_source_date_label: ICLR 2022
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
    published_venue: ICLR 2022
    date: Apr 30, 2022
    date_display: Apr 2022
    date_iso: '2022-04-30'
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
  metrics:
  - gap
  - mu
  - alpha
  - HOMO
  - LUMO
  - zpve
  - R2
  primary_metric: gap
  rank_metric: gap
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - mu
  - alpha
  - gap
  - HOMO
  - LUMO
  - zpve
  - R2
  metric: gap
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
    - dataset: QM9
      dataset_slug: qm9
single_proposed_model: new way to perform isotropic diffusion on graphs
main_figure: /figures/2205.00354/main_figure.jpegoptim.jpg
---

