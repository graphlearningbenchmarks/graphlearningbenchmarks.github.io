---
title: DualEquiNet RNA Benchmarks
arxiv_id: '2506.19862'
source_url: ''
authors:
- name: Junjie Xu
  orcid: null
  s2_author_id: '2326454620'
  s2_url: null
- name: Jiahao Zhang
  orcid: null
  s2_author_id: '2351823582'
  s2_url: null
- name: M. Prakash
  orcid: null
  s2_author_id: '2309178178'
  s2_url: null
- name: Xiang Zhang
  orcid: null
  s2_author_id: '2254295097'
  s2_url: null
- name: Suhang Wang
  orcid: null
  s2_author_id: '2283209331'
  s2_url: null
published_date: Jun 10, 2025
published_date_iso: '2025-06-10'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Geometric graph neural networks (GNNs) that respect E(3) symmetries have
  achieved strong performance on small molecule modeling, but they face scalability
  and expressiveness challenges when applied to large biomolecules such as RNA and
  proteins. These systems require models that can simultaneously capture fine-grained
  atomic interactions, long-range dependencies across spatially distant components,
  and biologically relevant hierarchical structure—such as atoms forming residues,
  which in turn form higher-order domains. Existing geometric GNNs, which typically
  operate exclusively in either Euclidean or Spherical Harmonics space, are limited
  in their ability to capture both the fine-scale atomic details and the long-range,
  symmetry-aware dependencies required for modeling the multi-scale structure of large
  biomolecules. We introduce DualEquiNet, a Dual-Space Hierarchical Equivariant Network
  that constructs complementary representations in both Euclidean and Spherical Harmonics
  spaces to capture local geometry and global symmetry-aware features. DualEquiNet
  employs bidirectional cross-space message passing and a novel Cross-Space Interaction
  Pooling mechanism to hierarchically aggregate atomic features into biologically
  meaningful units, such as residues, enabling efficient and expressive multi-scale
  modeling for large biomolecular systems. DualEquiNet achieves state-of-the-art performance
  on multiple existing benchmarks for RNA property prediction and protein modeling,
  and outperforms prior methods on two newly introduced 3D structural benchmarks demonstrating
  its broad effectiveness across a range of large biomolecule modeling tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DualEquiNet
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- DualEquiNet RNA Benchmarks
benchmark_coverage:
- benchmark: DualEquiNet RNA Benchmarks
  benchmark_slug: dualequinet-rna-benchmarks
  evaluated: 4
  total: 4
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id004
  dataset: COVID
  is_multi_metric: true
  rows:
  - model: DualEquiNet
    model_key: dualequinet
    model_plain: DualEquiNet
    metric_values:
    - null
    - 0.272
    - 0.448
    - 0.34
    - 0.353
    metric_stds:
    - null
    - 0.004
    - 0.01
    - 0.005
    - 0.006
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.272
    sort_std: 0.004
    true_value: 0.272
    true_std: 0.004
    paper_value: 0.272
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: GotenNet
    model_key: gotennet
    model_plain: GotenNet
    metric_values:
    - null
    - 0.388
    - 0.582
    - 0.455
    - 0.475
    metric_stds:
    - null
    - 0.002
    - 0.011
    - 0.008
    - 0.009
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.388
    sort_std: 0.002
    true_value: 0.388
    true_std: 0.002
    paper_value: 0.388
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: FastEGNN
    model_key: fastegnn
    model_plain: FastEGNN
    metric_values:
    - null
    - 0.39
    - 0.582
    - 0.463
    - 0.478
    metric_stds:
    - null
    - 0.019
    - 0.029
    - 0.027
    - 0.031
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.39
    sort_std: 0.019
    true_value: 0.39
    true_std: 0.019
    paper_value: 0.39
    paper_std: 0.019
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: GVPGNN
    model_key: gvpgnn
    model_plain: GVPGNN
    metric_values:
    - null
    - 0.448
    - 0.631
    - 0.515
    - 0.531
    metric_stds:
    - null
    - 0.006
    - 0.012
    - 0.009
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.448
    sort_std: 0.006
    true_value: 0.448
    true_std: 0.006
    paper_value: 0.448
    paper_std: 0.006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: HEGNN
    model_key: hegnn
    model_plain: HEGNN
    metric_values:
    - null
    - 0.45
    - 0.632
    - 0.517
    - 0.533
    metric_stds:
    - null
    - 0.005
    - 0.012
    - 0.009
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.45
    sort_std: 0.005
    true_value: 0.45
    true_std: 0.005
    paper_value: 0.45
    paper_std: 0.005
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - null
    - 0.451
    - 0.633
    - 0.518
    - 0.534
    metric_stds:
    - null
    - 0.006
    - 0.012
    - 0.01
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.451
    sort_std: 0.006
    true_value: 0.451
    true_std: 0.006
    paper_value: 0.451
    paper_std: 0.006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    metric_values:
    - null
    - 0.453
    - 0.634
    - 0.52
    - 0.535
    metric_stds:
    - null
    - 0.006
    - 0.013
    - 0.01
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.453
    sort_std: 0.006
    true_value: 0.453
    true_std: 0.006
    paper_value: 0.453
    paper_std: 0.006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: TFN
    model_key: tfn
    model_plain: TFN
    metric_values:
    - null
    - 0.453
    - 0.634
    - 0.52
    - 0.535
    metric_stds:
    - null
    - 0.006
    - 0.012
    - 0.01
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.453
    sort_std: 0.006
    true_value: 0.453
    true_std: 0.006
    paper_value: 0.453
    paper_std: 0.006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
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
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  metrics:
  - RMSE
  - Reactivity
  - pH10
  - Mg pH10
  - Avg.
  primary_metric: RMSE
  rank_metric: Reactivity
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - Reactivity
  - pH10
  - Mg pH10
  - Avg.
  metric: Reactivity
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Ribonanza
  rows:
  - model: DualEquiNet
    model_key: dualequinet
    model_plain: DualEquiNet
    value: 0.505
    std: 0.024
    paper_value: 0.505
    paper_std: 0.024
    metric: RMSE
    higher_is_better: false
    is_baseline: false
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
    protocol_note: Standard split for Ribonanza RNA property prediction (2A3 task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.505
    true_std: 0.024
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.505
    sort_std: 0.024
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: G-Heyna
    model_key: g-heyna
    model_plain: G-Heyna
    value: 0.529
    std: 0.005
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.529
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: G-Heyna
    model_key: g-transformer
    model_plain: G-Heyna
    value: 0.537
    std: 0.007
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.537
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastEGNN
    model_key: fastegnn
    model_plain: FastEGNN
    value: 0.808
    std: 0.022
    paper_value: 0.808
    paper_std: 0.022
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.873
    at_pub_std: 0.01
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.06499999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.808
    true_std: 0.022
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.022
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Geometric Hyena Networks for Large-scale Equivariant
      Learning
    comparison_source_arxiv: '2505.22560'
    is_best: false
    is_std_outlier: false
  - model: GotenNet
    model_key: gotennet
    model_plain: GotenNet
    value: 0.832
    std: 0.017
    paper_value: 0.832
    paper_std: 0.017
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.832
    true_std: 0.017
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: 0.017
    global_rank: 10
    paper_rank: 10
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
    value: 0.909
    std: 0.018
    paper_value: 0.909
    paper_std: 0.018
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.891
    at_pub_std: 0.008
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.018000000000000016
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.891
    true_std: 0.008
    value_gap_source_arxiv: '2505.22560'
    value_gap_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.018000000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.008
    global_rank: 12
    paper_rank: 14
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GVPGNN
    model_key: gvpgnn
    model_plain: GVPGNN
    value: 0.901
    std: 0.015
    paper_value: 0.901
    paper_std: 0.015
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.901
    true_std: 0.015
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.015
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HEGNN
    model_key: hegnn
    model_plain: HEGNN
    value: 0.904
    std: 0.015
    paper_value: 0.904
    paper_std: 0.015
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.015
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.015
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFN
    model_key: tfn
    model_plain: TFN
    value: 0.911
    std: 0.018
    paper_value: 0.911
    paper_std: 0.018
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.91
    at_pub_std: 0.011
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.91
    true_std: 0.011
    value_gap_source_arxiv: '2505.22560'
    value_gap_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.91
    sort_std: 0.011
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    value: 0.912
    std: 0.017
    paper_value: 0.912
    paper_std: 0.017
    metric: RMSE
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
    protocol_note: Standard split for Ribonanza RNA property prediction (DMS task).
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.928
    at_pub_std: 0.022
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.017
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.017
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Tc-Ribo
  rows:
  - model: G-Heyna
    model_key: g-heyna
    model_plain: G-Heyna
    value: 0.548
    std: 0.008
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.548
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: G-Heyna
    model_key: equiformer
    model_plain: G-Heyna
    value: 0.55
    std: 0.009
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.55
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: G-Heyna
    model_key: transformer
    model_plain: G-Heyna
    value: 0.553
    std: 0.002
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.553
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DualEquiNet
    model_key: dualequinet
    model_plain: DualEquiNet
    value: 0.636
    std: 0.049
    paper_value: 0.636
    paper_std: 0.049
    metric: RMSE
    higher_is_better: false
    is_baseline: false
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.636
    true_std: 0.049
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.636
    sort_std: 0.049
    global_rank: 6
    paper_rank: 6
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
    value: 0.737
    std: 0.002
    paper_value: 0.737
    paper_std: 0.002
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.691
    at_pub_std: 0.018
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.04600000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.691
    true_std: 0.018
    value_gap_source_arxiv: '2505.22560'
    value_gap_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.04600000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.691
    sort_std: 0.018
    global_rank: 7
    paper_rank: 13
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Geometric Hyena Networks for Large-scale Equivariant
      Learning
    comparison_source_arxiv: '2505.22560'
    is_best: false
    is_std_outlier: false
  - model: TFN
    model_key: tfn
    model_plain: TFN
    value: 0.694
    std: 0.008
    paper_value: 0.694
    paper_std: 0.008
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.71
    at_pub_std: 0.009
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.694
    true_std: 0.008
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.694
    sort_std: 0.008
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastEGNN
    model_key: fastegnn
    model_plain: FastEGNN
    value: 0.731
    std: 0.006
    paper_value: 0.731
    paper_std: 0.006
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.704
    at_pub_std: 0.005
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.027000000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.704
    true_std: 0.005
    value_gap_source_arxiv: '2505.22560'
    value_gap_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.027000000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.704
    sort_std: 0.005
    global_rank: 9
    paper_rank: 12
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Geometric Hyena Networks for Large-scale Equivariant
      Learning
    comparison_source_arxiv: '2505.22560'
    is_best: false
    is_std_outlier: false
  - model: GotenNet
    model_key: gotennet
    model_plain: GotenNet
    value: 0.718
    std: 0.002
    paper_value: 0.718
    paper_std: 0.002
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.718
    true_std: 0.002
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: 0.002
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    value: 0.72
    std: 0.022
    paper_value: 0.72
    paper_std: 0.022
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.728
    at_pub_std: 0.001
    at_pub_source_arxiv: '2505.22560'
    at_pub_source_title: Geometric Hyena Networks for Large-scale Equivariant Learning
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.72
    true_std: 0.022
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72
    sort_std: 0.022
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HEGNN
    model_key: hegnn
    model_plain: HEGNN
    value: 0.729
    std: 0.007
    paper_value: 0.729
    paper_std: 0.007
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: 0.007
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.007
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GVPGNN
    model_key: gvpgnn
    model_plain: GVPGNN
    value: 0.736
    std: 0.003
    paper_value: 0.736
    paper_std: 0.003
    metric: RMSE
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
    protocol_note: Standard split for Tc-Ribo regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.736
    true_std: 0.003
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.736
    sort_std: 0.003
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: TorsionAngle
  rows:
  - model: DualEquiNet
    model_key: dualequinet
    model_plain: DualEquiNet
    value: 15.87
    std: 2.03
    paper_value: 15.87
    paper_std: 2.03
    metric: Circular MAE
    higher_is_better: false
    is_baseline: false
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 15.87
    true_std: 2.03
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 15.87
    sort_std: 2.03
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GotenNet
    model_key: gotennet
    model_plain: GotenNet
    value: 16.27
    std: 1.19
    paper_value: 16.27
    paper_std: 1.19
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 16.27
    true_std: 1.19
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 16.27
    sort_std: 1.19
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GVPGNN
    model_key: gvpgnn
    model_plain: GVPGNN
    value: 17.56
    std: 0.21
    paper_value: 17.56
    paper_std: 0.21
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 17.56
    true_std: 0.21
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 17.56
    sort_std: 0.21
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    value: 17.79
    std: 0.61
    paper_value: 17.79
    paper_std: 0.61
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 17.79
    true_std: 0.61
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 17.79
    sort_std: 0.61
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HEGNN
    model_key: hegnn
    model_plain: HEGNN
    value: 18.41
    std: 0.22
    paper_value: 18.41
    paper_std: 0.22
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 18.41
    true_std: 0.22
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 18.41
    sort_std: 0.22
    global_rank: 5
    paper_rank: 5
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
    value: 18.54
    std: 0.86
    paper_value: 18.54
    paper_std: 0.86
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 18.54
    true_std: 0.86
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 18.54
    sort_std: 0.86
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FastEGNN
    model_key: fastegnn
    model_plain: FastEGNN
    value: 18.89
    std: 0.22
    paper_value: 18.89
    paper_std: 0.22
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 18.89
    true_std: 0.22
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 18.89
    sort_std: 0.22
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFN
    model_key: tfn
    model_plain: TFN
    value: 21.97
    std: 0.45
    paper_value: 21.97
    paper_std: 0.45
    metric: Circular MAE
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
    protocol_note: Standard split for TorsionAngle regression task
    date: Jun 10, 2025
    date_display: Jun 2025
    date_iso: '2025-06-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 21.97
    true_std: 0.45
    value_gap_source_arxiv: '2506.19862'
    value_gap_source_title: DualEquiNet RNA Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 21.97
    sort_std: 0.45
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
  rank_metric: Circular MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Circular MAE
  paper_metrics:
  - Circular MAE
  metric: Circular MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: DualEquiNet RNA Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: DualEquiNet RNA Benchmarks
    benchmark_slug: dualequinet-rna-benchmarks
    datasets:
    - dataset: Ribonanza
      dataset_slug: ribonanza
    - dataset: Tc-Ribo
      dataset_slug: tc-ribo
    - dataset: TorsionAngle
      dataset_slug: torsionangle
    - dataset: COVID
      dataset_slug: covid
single_proposed_model: DualEquiNet
main_figure: /figures/2506.19862/main_figure.jpegoptim.jpg
---

