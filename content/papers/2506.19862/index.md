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
  evaluated: 1
  total: 1
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
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
  - model: Equiformer
    model_key: equiformer
    model_plain: Equiformer
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
  - model: Transformer
    model_key: transformer
    model_plain: Transformer
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
results_grouped:
- benchmark: DualEquiNet RNA Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: DualEquiNet RNA Benchmarks
    benchmark_slug: dualequinet-rna-benchmarks
    datasets:
    - dataset: Tc-Ribo
      dataset_slug: tc-ribo
single_proposed_model: DualEquiNet
main_figure: /figures/2506.19862/main_figure.jpegoptim.jpg
---

