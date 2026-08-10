---
title: Clifford Group Equivariant Simplicial Message Passing Networks
arxiv_id: '2402.10011'
source_url: ''
authors:
- name: Cong Liu
  orcid: null
  s2_author_id: '2284229676'
  s2_url: null
- name: David Ruhe
  orcid: null
  s2_author_id: '2284218320'
  s2_url: null
- name: Floor Eijkelboom
  orcid: null
  s2_author_id: '2208907804'
  s2_url: null
- name: Patrick Forr'e
  orcid: null
  s2_author_id: '51131843'
  s2_url: null
published_date: Feb 15, 2024
published_date_iso: '2024-02-15'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: We introduce, a method for steerable $E(n)$-equivariant message passing
  on simplicial complexes. Our method integrates the expressivity of Clifford group-equivariant
  layers with simplicial message passing, which is topologically more intricate than
  regular graph message passing. Clifford algebras include higher-order objects such
  as bivectors and trivectors, which express geometric features (e.g., areas, volumes)
  derived from vectors. Using this knowledge, we represent simplex features through
  geometric products of their vertices. To achieve efficient simplicial message passing,
  we share the parameters of the message network across different dimensions. Additionally,
  we restrict the final message to an aggregation of the incoming messages from different
  dimensions, leading to what we term shared simplicial message passing. Experimental
  results show that our method is able to outperform both equivariant and simplicial
  graph neural networks on a variety of geometric tasks. Our implementation is available
  on GitHub.
codebase_url: https://github.com/congliuUvA/Clifford-Group-Equivariant-Simplicial-Message-Passing-Networks
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- shared simplicial message passing (300K)
mrr: 0.0
adjusted_mrr: 0.0
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
  is_multi_metric: true
  rows:
  - model: empsn (300K)
    model_key: empsn (300k)
    model_plain: empsn (300K)
    metric_values:
    - null
    - 0.0103
    - 0.0112
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
    sort_value: 0.0103
    sort_std: null
    true_value: 0.0103
    true_std: null
    paper_value: 0.0103
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: cgenn (300K)
    model_key: cgenn (300k)
    model_plain: cgenn (300K)
    metric_values:
    - null
    - 0.037
    - 0.0563
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
    sort_value: 0.037
    sort_std: null
    true_value: 0.037
    true_std: null
    paper_value: 0.037
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: shared simplicial message passing (300K)
    model_key: shared simplicial message passing (300k)
    model_plain: shared simplicial message passing (300K)
    metric_values:
    - null
    - 0.0382
    - 0.0575
    metric_stds:
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
    sort_value: 0.0382
    sort_std: null
    true_value: 0.0382
    true_std: null
    paper_value: 0.0382
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: EqMotion (300K)
    model_key: eqmotion (300k)
    model_plain: EqMotion (300K)
    metric_values:
    - null
    - 0.0595
    - 0.0838
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
    sort_value: 0.0595
    sort_std: null
    true_value: 0.0595
    true_std: null
    paper_value: 0.0595
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: GMN-L
    model_key: gmn-l
    model_plain: GMN-L
    metric_values:
    - null
    - 0.0976
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
    sort_value: 0.0976
    sort_std: null
    true_value: 0.0976
    true_std: null
    paper_value: 0.0976
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: NMMP
    model_key: nmmp
    model_plain: NMMP
    metric_values:
    - null
    - 0.1041
    - 0.1467
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
    sort_value: 0.1041
    sort_std: null
    true_value: 0.1041
    true_std: null
    paper_value: 0.1041
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: GroupNet
    model_key: groupnet
    model_plain: GroupNet
    metric_values:
    - null
    - 0.1062
    - 0.14
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
    sort_value: 0.1062
    sort_std: null
    true_value: 0.1062
    true_std: null
    paper_value: 0.1062
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: NRI
    model_key: nri
    model_plain: NRI
    metric_values:
    - null
    - 0.126
    - 0.185
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
    sort_value: 0.126
    sort_std: null
    true_value: 0.126
    true_std: null
    paper_value: 0.126
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: S-LSTM
    model_key: s-lstm
    model_plain: S-LSTM
    metric_values:
    - null
    - 0.1312
    - 0.1814
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
    sort_value: 0.1312
    sort_std: null
    true_value: 0.1312
    true_std: null
    paper_value: 0.1312
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    metric_values:
    - null
    - 0.1461
    - 0.2065
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
    sort_value: 0.1461
    sort_std: null
    true_value: 0.1461
    true_std: null
    paper_value: 0.1461
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: TFN
    model_key: tfn
    model_plain: TFN
    metric_values:
    - null
    - 0.1502
    - 0.2135
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
    sort_value: 0.1502
    sort_std: null
    true_value: 0.1502
    true_std: null
    paper_value: 0.1502
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: SE(3)-Tr
    model_key: se(3)-tr
    model_plain: SE(3)-Tr
    metric_values:
    - null
    - 0.157
    - 0.2239
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.157
    sort_std: null
    true_value: 0.157
    true_std: null
    paper_value: 0.157
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: Radial Field
    model_key: radial field
    model_plain: Radial Field
    metric_values:
    - null
    - 0.1798
    - 0.262
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
    sort_value: 0.1798
    sort_std: null
    true_value: 0.1798
    true_std: null
    paper_value: 0.1798
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2402.10011'
    value_gap_source_title: Clifford Group Equivariant Simplicial Message Passing
      Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-15'
    value_gap_source_date_label: ICLR 2024
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
    published_venue: ICLR 2024
    date: Feb 15, 2024
    date_display: Feb 2024
    date_iso: '2024-02-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  metrics:
  - MAE
  - ADE
  - FDE
  primary_metric: MAE
  rank_metric: ADE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - ADE
  - FDE
  metric: ADE
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
single_proposed_model: shared simplicial message passing (300K)
main_figure: /figures/2402.10011/main_figure.jpegoptim.jpg
---

