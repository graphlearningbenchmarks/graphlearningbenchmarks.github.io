---
title: HSG-12M
arxiv_id: '2506.08618'
source_url: ''
authors:
- name: Xianquan Yan
  orcid: null
  s2_author_id: '2330181730'
  s2_url: null
- name: Hakan Akgun
  orcid: null
  s2_author_id: '2330189502'
  s2_url: null
- name: Kenji Kawaguchi
  orcid: null
  s2_author_id: '2268400351'
  s2_url: null
- name: N. D. Loh
  orcid: null
  s2_author_id: '2250864067'
  s2_url: null
- name: Ching Hua Lee
  orcid: null
  s2_author_id: '2330392191'
  s2_url: null
published_date: Jun 10, 2025
published_date_iso: '2025-06-10'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'AI is transforming scientific research by revealing new ways to understand
  complex physical systems, but its impact remains constrained by the lack of large,
  high-quality domain-specific datasets. A rich, largely untapped resource lies in
  non-Hermitian quantum physics, where the energy spectra of crystals form intricate
  geometries on the complex plane -- termed as Hamiltonian spectral graphs. Despite
  their significance as fingerprints for electronic behavior, their systematic study
  has been intractable due to the reliance on manual extraction. To unlock this potential,
  we introduce Poly2Graph: a high-performance, open-source pipeline that automates
  the mapping of 1-D crystal Hamiltonians to spectral graphs. Using this tool, we
  present HSG-12M: a dataset containing 11.6 million static and 5.1 million dynamic
  Hamiltonian spectral graphs across 1401 characteristic-polynomial classes, distilled
  from 177 TB of spectral potential data. Crucially, HSG-12M is the first large-scale
  dataset of spatial multigraphs -- graphs embedded in a metric space where multiple
  geometrically distinct trajectories between two nodes are retained as separate edges.
  This simultaneously addresses a critical gap, as existing graph benchmarks overwhelmingly
  assume simple, non-spatial edges, discarding vital geometric information. Benchmarks
  with popular GNNs expose new challenges in learning spatial multi-edges at scale.
  Beyond its practical utility, we show that spectral graphs serve as universal topological
  fingerprints of polynomials, vectors, and matrices, forging a new algebra-to-graph
  link. HSG-12M lays the groundwork for data-driven scientific discovery in condensed
  matter physics, new opportunities in geometry-aware graph learning and beyond.'
codebase_url: https://github.com/sarinstein-yan/HSG-12M
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- HSG-12M
benchmark_coverage:
- benchmark: HSG-12M
  benchmark_slug: hsg-12m
  evaluated: 2
  total: 2
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: HSG-12M
  is_multi_metric: true
  rows:
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.546
    - 0.952
    metric_stds:
    - 0.004
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.546
    sort_std: 0.004
    true_value: 0.546
    true_std: 0.004
    paper_value: 0.546
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: CGCNN
    model_key: cgcnn
    model_plain: CGCNN
    metric_values:
    - 0.531
    - null
    metric_stds:
    - 0.004
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.531
    sort_std: 0.004
    true_value: 0.531
    true_std: 0.004
    paper_value: 0.531
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GINE
    model_key: gine
    model_plain: GINE
    metric_values:
    - 0.46
    - 0.921
    metric_stds:
    - 0.025
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.46
    sort_std: 0.025
    true_value: 0.46
    true_std: 0.025
    paper_value: 0.46
    paper_std: 0.025
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.365
    - null
    metric_stds:
    - 0.021
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.365
    sort_std: 0.021
    true_value: 0.365
    true_std: 0.021
    paper_value: 0.365
    paper_std: 0.021
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.365
    - null
    metric_stds:
    - 0.01
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.365
    sort_std: 0.01
    true_value: 0.365
    true_std: 0.01
    paper_value: 0.365
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    metric_values:
    - 0.351
    - null
    metric_stds:
    - 0.002
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.351
    sort_std: 0.002
    true_value: 0.351
    true_std: 0.002
    paper_value: 0.351
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: MF
    model_key: mf
    model_plain: MF
    metric_values:
    - 0.295
    - null
    metric_stds:
    - 0.01
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.295
    sort_std: 0.01
    true_value: 0.295
    true_std: 0.01
    paper_value: 0.295
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.063
    - null
    metric_stds:
    - 0.031
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.063
    sort_std: 0.031
    true_value: 0.063
    true_std: 0.031
    paper_value: 0.063
    paper_std: 0.031
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - Accuracy
  - Top-10 Acc.
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - Top-10 Acc.
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: HSG-topology
  is_multi_metric: true
  rows:
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.62
    - 0.622
    - 0.958
    - 1.019
    - 0.898
    metric_stds:
    - 0.003
    - 0.001
    - 0.001
    - 0.002
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.62
    sort_std: 0.003
    true_value: 0.62
    true_std: 0.003
    paper_value: 0.62
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: CGCNN
    model_key: cgcnn
    model_plain: CGCNN
    metric_values:
    - 0.566
    - 0.563
    - 0.94
    - 1.191
    - 0.87
    metric_stds:
    - 0.016
    - 0.018
    - 0.005
    - 0.065
    - 0.008
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.566
    sort_std: 0.016
    true_value: 0.566
    true_std: 0.016
    paper_value: 0.566
    paper_std: 0.016
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GINE
    model_key: gine
    model_plain: GINE
    metric_values:
    - 0.533
    - 0.531
    - 0.927
    - 1.316
    - 0.848
    metric_stds:
    - 0.017
    - 0.011
    - 0.008
    - 0.057
    - 0.013
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.533
    sort_std: 0.017
    true_value: 0.533
    true_std: 0.017
    paper_value: 0.533
    paper_std: 0.017
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.434
    - 0.431
    - 0.855
    - 1.825
    - 0.752
    metric_stds:
    - 0.015
    - 0.011
    - 0.01
    - 0.053
    - 0.014
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.434
    sort_std: 0.015
    true_value: 0.434
    true_std: 0.015
    paper_value: 0.434
    paper_std: 0.015
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    metric_values:
    - 0.401
    - 0.397
    - 0.833
    - 1.968
    - 0.723
    metric_stds:
    - 0.003
    - 0.001
    - 0.005
    - 0.025
    - 0.005
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.401
    sort_std: 0.003
    true_value: 0.401
    true_std: 0.003
    paper_value: 0.401
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.397
    - 0.392
    - 0.825
    - 2.062
    - 0.715
    metric_stds:
    - 0.009
    - 0.011
    - 0.006
    - 0.062
    - 0.007
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.397
    sort_std: 0.009
    true_value: 0.397
    true_std: 0.009
    paper_value: 0.397
    paper_std: 0.009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: MF
    model_key: mf
    model_plain: MF
    metric_values:
    - 0.348
    - 0.343
    - 0.793
    - 2.222
    - 0.673
    metric_stds:
    - 0.012
    - 0.012
    - 0.01
    - 0.051
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.348
    sort_std: 0.012
    true_value: 0.348
    true_std: 0.012
    paper_value: 0.348
    paper_std: 0.012
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.095
    - 0.082
    - 0.39
    - 4.179
    - 0.276
    metric_stds:
    - 0.059
    - 0.06
    - 0.148
    - 0.612
    - 0.127
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.095
    sort_std: 0.059
    true_value: 0.095
    true_std: 0.059
    paper_value: 0.095
    paper_std: 0.059
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.08618'
    value_gap_source_title: HSG-12M
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-10'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
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
  - Accuracy
  - Macro F1
  - Top-10 Acc.
  - Loss
  - Top-5 Accuracy
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - Macro F1
  - Top-10 Acc.
  - Loss
  - Top-5 Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: HSG-12M
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: HSG-12M
    benchmark_slug: hsg-12m
    datasets:
    - dataset: HSG-12M
      dataset_slug: hsg-12m
    - dataset: HSG-topology
      dataset_slug: hsg-topology
main_figure: /figures/2506.08618/main_figure.jpegoptim.jpg
---

