---
title: Homophily-oriented Heterogeneous Graph Rewiring
arxiv_id: '2302.06299'
source_url: ''
authors:
- name: Jiayan Guo
  orcid: null
  s2_author_id: '5765645'
  s2_url: null
- name: Lun Du
  orcid: null
  s2_author_id: '12723949'
  s2_url: null
- name: Wendong Bi
  orcid: null
  s2_author_id: '1429833857'
  s2_url: null
- name: Qiang Fu
  orcid: null
  s2_author_id: '2113771309'
  s2_url: null
- name: Xiaojun Ma
  orcid: null
  s2_author_id: '150344398'
  s2_url: null
- name: Xu Chen
  orcid: null
  s2_author_id: '2144230023'
  s2_url: null
- name: Shi Han
  orcid: null
  s2_author_id: '2109750123'
  s2_url: null
- name: Dongmei Zhang
  orcid: null
  s2_author_id: '2140415600'
  s2_url: null
- name: Yan Zhang
  orcid: null
  s2_author_id: '2152821652'
  s2_url: null
published_date: Feb 13, 2023
published_date_iso: '2023-02-13'
published_venue: WWW 2023
published_conference: WWW 2023
published_conference_short: WWW
published_conference_slug: www
abstract: With the rapid development of the World Wide Web (WWW), heterogeneous graphs
  (HG) have explosive growth. Recently, heterogeneous graph neural network (HGNN)
  has shown great potential in learning on HG. Current studies of HGNN mainly focus
  on some HGs with strong homophily properties (nodes connected by meta-path tend
  to have the same labels), while few discussions are made in those that are less
  homophilous. Recently, there have been many works on homogeneous graphs with heterophily.
  However, due to heterogeneity, it is non-trivial to extend their approach to deal
  with HGs with heterophily. In this work, based on empirical observations, we propose
  a meta-path-induced metric to measure the homophily degree of a HG. We also find
  that current HGNNs may have degenerated performance when handling HGs with less
  homophilous properties. Thus it is essential to increase the generalization ability
  of HGNNs on non-homophilous HGs. To this end, we propose HDHGR, a homophily-oriented
  deep heterogeneous graph rewiring approach that modifies the HG structure to increase
  the performance of HGNN. We theoretically verify HDHGR. In addition, experiments
  on real-world HGs demonstrate the effectiveness of HDHGR, which brings at most more
  than 10\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN HDHGR
- GAT HDHGR
- H2GCN HDHGR
- LINKX HDHGR
- RGCN HDHGR
- HAN HDHGR
- HGT HDHGR
- SHGN HDHGR
- HDHGR
mrr: 0.0103
adjusted_mrr: 0.0034
mrr_dataset_count: 1
benchmark_categories:
- Heterophilic Graphs
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 3
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: ACM
  is_multi_metric: true
  rows:
  - model: SlotGAT
    model_key: hetgnn
    model_plain: SlotGAT
    metric_values:
    - 0.979
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    published_venue: ''
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.979
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
  - model: SlotGAT
    model_key: comch
    model_plain: SlotGAT
    metric_values:
    - 0.947
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    published_venue: ''
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.947
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
  - model: SlotGAT
    model_key: lmsps
    model_plain: SlotGAT
    metric_values:
    - 0.9469
    - null
    metric_stds:
    - 0.0036
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    published_venue: ''
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9469
    sort_std: 0.0036
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    metric_values:
    - 0.9141
    - 0.9155
    metric_stds:
    - 0.0075
    - 0.0074
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9402
    sort_std: null
    true_value: 0.9402
    true_std: null
    paper_value: 0.9141
    paper_std: 0.0075
    has_value_gap: true
    has_value_note: false
    value_gap: 0.026100000000000012
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_note: ''
    at_pub_value: 0.9141
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: HDHGR
    model_key: hdhgr
    model_plain: HDHGR
    metric_values:
    - 0.938
    - 0.9388
    metric_stds:
    - 0.002
    - 0.002
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.938
    sort_std: 0.002
    true_value: 0.938
    true_std: 0.002
    paper_value: 0.938
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: SHGN
    model_key: shgn
    model_plain: SHGN
    metric_values:
    - 0.9335
    - 0.9342
    metric_stds:
    - 0.0045
    - 0.0044
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9335
    sort_std: 0.0045
    true_value: 0.9335
    true_std: 0.0045
    paper_value: 0.9335
    paper_std: 0.0045
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.9219
    - 0.9226
    metric_stds:
    - 0.0093
    - 0.0094
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9278
    sort_std: null
    true_value: 0.9278
    true_std: null
    paper_value: 0.9219
    paper_std: 0.0093
    has_value_gap: true
    has_value_note: false
    value_gap: 0.005899999999999905
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_note: ''
    at_pub_value: 0.9278
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.005899999999999905
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.9212
    - 0.9217
    metric_stds:
    - 0.0023
    - 0.0024
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9246
    sort_std: null
    true_value: 0.9246
    true_std: null
    paper_value: 0.9212
    paper_std: 0.0023
    has_value_gap: true
    has_value_note: false
    value_gap: 0.0033999999999999586
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_note: ''
    at_pub_value: 0.9246
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.0033999999999999586
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: HAN
    model_key: han
    model_plain: HAN
    metric_values:
    - 0.9079
    - 0.9089
    metric_stds:
    - 0.0043
    - 0.0043
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9185
    sort_std: null
    true_value: 0.9185
    true_std: null
    paper_value: 0.9079
    paper_std: 0.0043
    has_value_gap: true
    has_value_note: false
    value_gap: 0.010599999999999943
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_note: ''
    at_pub_value: 0.9079
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    metric_values:
    - 0.8863
    - 0.8879
    metric_stds:
    - 0.0048
    - 0.0045
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8863
    sort_std: 0.0048
    true_value: 0.8863
    true_std: 0.0048
    paper_value: 0.8863
    paper_std: 0.0048
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 79
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    metric_values:
    - 0.848
    - 0.8475
    metric_stds:
    - 0.0038
    - 0.0038
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.848
    sort_std: 0.0038
    true_value: 0.848
    true_std: 0.0038
    paper_value: 0.848
    paper_std: 0.0038
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 102
  metrics:
  - Micro-F1
  - Macro-F1
  primary_metric: Micro-F1
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Macro-F1
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Actor
  is_multi_metric: true
  rows:
  - model: HDHGR
    model_key: cthge
    model_plain: HDHGR
    metric_values:
    - 0.8258
    - null
    - null
    metric_stds:
    - 0.0039
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2501.14600'
    title: 'On the Cross-type Homophily of Heterogeneous Graphs: Understanding and
      Unleashing'
    published_venue: ''
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: true
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.8258
    sort_std: 0.0039
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
  - model: HGT HDHGR
    model_key: hgt hdhgr
    model_plain: HGT HDHGR
    metric_values:
    - null
    - 0.7725
    - 0.8406
    metric_stds:
    - null
    - 0.0053
    - 0.0029
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7725
    sort_std: 0.0053
    true_value: 0.7725
    true_std: 0.0053
    paper_value: 0.7725
    paper_std: 0.0053
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: HDHGR
    model_key: pshgcn
    model_plain: HDHGR
    metric_values:
    - 0.762
    - null
    - null
    metric_stds:
    - 0.0128
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2501.14600'
    title: 'On the Cross-type Homophily of Heterogeneous Graphs: Understanding and
      Unleashing'
    published_venue: ''
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.762
    sort_std: 0.0128
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
  - model: HGT origin
    model_key: hgt origin
    model_plain: HGT origin
    metric_values:
    - null
    - 0.7558
    - 0.8297
    metric_stds:
    - null
    - 0.0048
    - 0.0029
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7558
    sort_std: 0.0048
    true_value: 0.7558
    true_std: 0.0048
    paper_value: 0.7558
    paper_std: 0.0048
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: SHGN HDHGR
    model_key: shgn hdhgr
    model_plain: SHGN HDHGR
    metric_values:
    - null
    - 0.7273
    - 0.8136
    metric_stds:
    - null
    - 0.0035
    - 0.0037
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7273
    sort_std: 0.0035
    true_value: 0.7273
    true_std: 0.0035
    paper_value: 0.7273
    paper_std: 0.0035
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: SHGN origin
    model_key: shgn origin
    model_plain: SHGN origin
    metric_values:
    - null
    - 0.7166
    - 0.8085
    metric_stds:
    - null
    - 0.0162
    - 0.0029
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7166
    sort_std: 0.0162
    true_value: 0.7166
    true_std: 0.0162
    paper_value: 0.7166
    paper_std: 0.0162
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: HAN HDHGR
    model_key: han hdhgr
    model_plain: HAN HDHGR
    metric_values:
    - null
    - 0.7113
    - 0.8089
    metric_stds:
    - null
    - 0.0138
    - 0.0039
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7113
    sort_std: 0.0138
    true_value: 0.7113
    true_std: 0.0138
    paper_value: 0.7113
    paper_std: 0.0138
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: GCN HDHGR
    model_key: gcn hdhgr
    model_plain: GCN HDHGR
    metric_values:
    - null
    - 0.6721
    - 0.7507
    metric_stds:
    - null
    - 0.0094
    - 0.0038
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.6721
    sort_std: 0.0094
    true_value: 0.6721
    true_std: 0.0094
    paper_value: 0.6721
    paper_std: 0.0094
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: HDHGR
    model_key: hdhgr
    model_plain: HDHGR
    metric_values:
    - null
    - 0.6721
    - 0.7507
    metric_stds:
    - null
    - 0.0094
    - 0.0038
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.6721
    sort_std: 0.0094
    true_value: 0.6721
    true_std: 0.0094
    paper_value: 0.6721
    paper_std: 0.0094
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: GAT HDHGR
    model_key: gat hdhgr
    model_plain: GAT HDHGR
    metric_values:
    - null
    - 0.6383
    - 0.7423
    metric_stds:
    - null
    - 0.0056
    - 0.0028
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.6383
    sort_std: 0.0056
    true_value: 0.6383
    true_std: 0.0056
    paper_value: 0.6383
    paper_std: 0.0056
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: LINKX HDHGR
    model_key: linkx hdhgr
    model_plain: LINKX HDHGR
    metric_values:
    - null
    - 0.6379
    - 0.7023
    metric_stds:
    - null
    - 0.0205
    - 0.0183
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.6379
    sort_std: 0.0205
    true_value: 0.6379
    true_std: 0.0205
    paper_value: 0.6379
    paper_std: 0.0205
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: H2GCN HDHGR
    model_key: h2gcn hdhgr
    model_plain: H2GCN HDHGR
    metric_values:
    - null
    - 0.6267
    - 0.7266
    metric_stds:
    - null
    - 0.0113
    - 0.0051
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.6267
    sort_std: 0.0113
    true_value: 0.6267
    true_std: 0.0113
    paper_value: 0.6267
    paper_std: 0.0113
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: IDGL
    model_key: idgl
    model_plain: IDGL
    metric_values:
    - null
    - 0.5964
    - 0.6591
    metric_stds:
    - null
    - 0.0171
    - 0.0273
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5964
    sort_std: 0.0171
    true_value: 0.5964
    true_std: 0.0171
    paper_value: 0.5964
    paper_std: 0.0171
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: HGSL
    model_key: hgsl
    model_plain: HGSL
    metric_values:
    - null
    - 0.5835
    - 0.6326
    metric_stds:
    - null
    - 0.0123
    - 0.0254
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5835
    sort_std: 0.0123
    true_value: 0.5835
    true_std: 0.0123
    paper_value: 0.5835
    paper_std: 0.0123
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: LINKX origin
    model_key: linkx origin
    model_plain: LINKX origin
    metric_values:
    - null
    - 0.5798
    - 0.6397
    metric_stds:
    - null
    - 0.0201
    - 0.0177
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.5798
    sort_std: 0.0201
    true_value: 0.5798
    true_std: 0.0201
    paper_value: 0.5798
    paper_std: 0.0201
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 18
  - model: LDS
    model_key: lds
    model_plain: LDS
    metric_values:
    - null
    - 0.5622
    - 0.6235
    metric_stds:
    - null
    - 0.0324
    - 0.0289
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5622
    sort_std: 0.0324
    true_value: 0.5622
    true_std: 0.0324
    paper_value: 0.5622
    paper_std: 0.0324
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: GCN origin
    model_key: gcn origin
    model_plain: GCN origin
    metric_values:
    - null
    - 0.5538
    - 0.6579
    metric_stds:
    - null
    - 0.0032
    - 0.0021
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.5538
    sort_std: 0.0032
    true_value: 0.5538
    true_std: 0.0032
    paper_value: 0.5538
    paper_std: 0.0032
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: HAN origin
    model_key: han origin
    model_plain: HAN origin
    metric_values:
    - null
    - 0.5478
    - 0.6895
    metric_stds:
    - null
    - 0.0154
    - 0.0026
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.5478
    sort_std: 0.0154
    true_value: 0.5478
    true_std: 0.0154
    paper_value: 0.5478
    paper_std: 0.0154
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: RGCN HDHGR
    model_key: rgcn hdhgr
    model_plain: RGCN HDHGR
    metric_values:
    - null
    - 0.5333
    - 0.7483
    metric_stds:
    - null
    - 0.0158
    - 0.0039
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.5333
    sort_std: 0.0158
    true_value: 0.5333
    true_std: 0.0158
    paper_value: 0.5333
    paper_std: 0.0158
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: H2GCN origin
    model_key: h2gcn origin
    model_plain: H2GCN origin
    metric_values:
    - null
    - 0.497
    - 0.6365
    metric_stds:
    - null
    - 0.0067
    - 0.0076
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.497
    sort_std: 0.0067
    true_value: 0.497
    true_std: 0.0067
    paper_value: 0.497
    paper_std: 0.0067
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: RGCN origin
    model_key: rgcn origin
    model_plain: RGCN origin
    metric_values:
    - null
    - 0.4921
    - 0.7161
    metric_stds:
    - null
    - 0.0248
    - 0.0082
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.4921
    sort_std: 0.0248
    true_value: 0.4921
    true_std: 0.0248
    paper_value: 0.4921
    paper_std: 0.0248
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: GAT origin
    model_key: gat origin
    model_plain: GAT origin
    metric_values:
    - null
    - 0.4578
    - 0.6091
    metric_stds:
    - null
    - 0.01
    - 0.0058
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.4578
    sort_std: 0.01
    true_value: 0.4578
    true_std: 0.01
    paper_value: 0.4578
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
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
  - model: OriMetapath
    model_key: orimetapath
    model_plain: OriMetapath
    metric_values:
    - null
    - 0.4218
    - 0.5851
    metric_stds:
    - null
    - 0.0046
    - 0.0021
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.4218
    sort_std: 0.0046
    true_value: 0.4218
    true_std: 0.0046
    paper_value: 0.4218
    paper_std: 0.0046
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
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
    published_venue: WWW 2023
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  metrics:
  - Accuracy
  - Macro-F1
  - Micro-F1
  primary_metric: Accuracy
  rank_metric: Macro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Macro-F1
  - Micro-F1
  metric: Macro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: DBLP
  rows:
  - model: SlotGAT
    model_key: herec
    model_plain: SlotGAT
    value: 0.9993
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9993
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: hetsann
    model_plain: SlotGAT
    value: 0.9972
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9972
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: deepwalk
    model_plain: SlotGAT
    value: 0.9941
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9941
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SHGN (HDHGR)
    model_key: shgn (hdhgr)
    model_plain: SHGN (HDHGR)
    value: 0.9473
    std: 0.0016
    paper_value: 0.9473
    paper_std: 0.0016
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before SHGN
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9473
    true_std: 0.0016
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9473
    sort_std: 0.0016
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT (HDHGR)
    model_key: gat (hdhgr)
    model_plain: GAT (HDHGR)
    value: 0.947
    std: 0.0011
    paper_value: 0.947
    paper_std: 0.0011
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before GAT
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.947
    true_std: 0.0011
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.947
    sort_std: 0.0011
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX (HDHGR)
    model_key: linkx (hdhgr)
    model_plain: LINKX (HDHGR)
    value: 0.9369
    std: 0.0026
    paper_value: 0.9369
    paper_std: 0.0026
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before LINKX
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9369
    true_std: 0.0026
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9369
    sort_std: 0.0026
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN (HDHGR)
    model_key: h2gcn (hdhgr)
    model_plain: H2GCN (HDHGR)
    value: 0.9277
    std: 0.0031
    paper_value: 0.9277
    paper_std: 0.0031
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before H2GCN
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9277
    true_std: 0.0031
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9277
    sort_std: 0.0031
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN (HDHGR)
    model_key: rgcn (hdhgr)
    model_plain: RGCN (HDHGR)
    value: 0.9259
    std: 0.0063
    paper_value: 0.9259
    paper_std: 0.0063
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before RGCN
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9259
    true_std: 0.0063
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9259
    sort_std: 0.0063
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN (HDHGR)
    model_key: han (hdhgr)
    model_plain: HAN (HDHGR)
    value: 0.9257
    std: 0.0056
    paper_value: 0.9257
    paper_std: 0.0056
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before HAN
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9257
    true_std: 0.0056
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9257
    sort_std: 0.0056
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN (HDHGR)
    model_key: gcn (hdhgr)
    model_plain: GCN (HDHGR)
    value: 0.9201
    std: 0.001
    paper_value: 0.9201
    paper_std: 0.001
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification; HDHGR rewires the
      graph before GCN
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9201
    true_std: 0.001
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9201
    sort_std: 0.001
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: IMDB
  rows:
  - model: SlotGAT
    model_key: gat bgnn(m)-sc
    model_plain: SlotGAT
    value: 0.8133
    std: 0.0179
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8133
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: sage ban
    model_plain: SlotGAT
    value: 0.8073
    std: 0.002
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8073
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: gat bgnn(m)-cs
    model_plain: SlotGAT
    value: 0.8033
    std: 0.0094
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8033
    sort_std: 0.0094
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HAN HDHGR
    model_key: han hdhgr
    model_plain: HAN HDHGR
    value: 0.5932
    std: 0.0053
    paper_value: 0.5932
    paper_std: 0.0053
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5932
    true_std: 0.0053
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5932
    sort_std: 0.0053
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN HDHGR
    model_key: gcn hdhgr
    model_plain: GCN HDHGR
    value: 0.5897
    std: 0.0041
    paper_value: 0.5897
    paper_std: 0.0041
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5897
    true_std: 0.0041
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5897
    sort_std: 0.0041
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT HDHGR
    model_key: gat hdhgr
    model_plain: GAT HDHGR
    value: 0.5799
    std: 0.0216
    paper_value: 0.5799
    paper_std: 0.0216
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5799
    true_std: 0.0216
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5799
    sort_std: 0.0216
    global_rank: 99
    paper_rank: 99
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN origin
    model_key: gcn origin
    model_plain: GCN origin
    value: 0.5684
    std: 0.0266
    paper_value: 0.5684
    paper_std: 0.0266
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5684
    true_std: 0.0266
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5684
    sort_std: 0.0266
    global_rank: 103
    paper_rank: 103
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SHGN HDHGR
    model_key: shgn hdhgr
    model_plain: SHGN HDHGR
    value: 0.5656
    std: 0.0048
    paper_value: 0.5656
    paper_std: 0.0048
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5656
    true_std: 0.0048
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5656
    sort_std: 0.0048
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN HDHGR
    model_key: h2gcn hdhgr
    model_plain: H2GCN HDHGR
    value: 0.5603
    std: 0.0024
    paper_value: 0.5603
    paper_std: 0.0024
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5603
    true_std: 0.0024
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5603
    sort_std: 0.0024
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT origin
    model_key: gat origin
    model_plain: GAT origin
    value: 0.5582
    std: 0.0211
    paper_value: 0.5582
    paper_std: 0.0211
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5582
    true_std: 0.0211
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5582
    sort_std: 0.0211
    global_rank: 109
    paper_rank: 109
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN origin
    model_key: han origin
    model_plain: HAN origin
    value: 0.5581
    std: 0.0169
    paper_value: 0.5581
    paper_std: 0.0169
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5581
    true_std: 0.0169
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5581
    sort_std: 0.0169
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN HDHGR
    model_key: rgcn hdhgr
    model_plain: RGCN HDHGR
    value: 0.5545
    std: 0.0071
    paper_value: 0.5545
    paper_std: 0.0071
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5545
    true_std: 0.0071
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5545
    sort_std: 0.0071
    global_rank: 111
    paper_rank: 111
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN origin
    model_key: h2gcn origin
    model_plain: H2GCN origin
    value: 0.5429
    std: 0.0062
    paper_value: 0.5429
    paper_std: 0.0062
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5429
    true_std: 0.0062
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5429
    sort_std: 0.0062
    global_rank: 113
    paper_rank: 113
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT HDHGR
    model_key: hgt hdhgr
    model_plain: HGT HDHGR
    value: 0.5293
    std: 0.0162
    paper_value: 0.5293
    paper_std: 0.0162
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5293
    true_std: 0.0162
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5293
    sort_std: 0.0162
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN origin
    model_key: rgcn origin
    model_plain: RGCN origin
    value: 0.5251
    std: 0.0267
    paper_value: 0.5251
    paper_std: 0.0267
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5251
    true_std: 0.0267
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5251
    sort_std: 0.0267
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SHGN origin
    model_key: shgn origin
    model_plain: SHGN origin
    value: 0.525
    std: 0.0091
    paper_value: 0.525
    paper_std: 0.0091
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.525
    true_std: 0.0091
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.525
    sort_std: 0.0091
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT origin
    model_key: hgt origin
    model_plain: HGT origin
    value: 0.5088
    std: 0.0041
    paper_value: 0.5088
    paper_std: 0.0041
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5088
    true_std: 0.0041
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5088
    sort_std: 0.0041
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX HDHGR
    model_key: linkx hdhgr
    model_plain: LINKX HDHGR
    value: 0.483
    std: 0.0085
    paper_value: 0.483
    paper_std: 0.0085
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.483
    true_std: 0.0085
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.483
    sort_std: 0.0085
    global_rank: 128
    paper_rank: 128
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX origin
    model_key: linkx origin
    model_plain: LINKX origin
    value: 0.4411
    std: 0.0112
    paper_value: 0.4411
    paper_std: 0.0112
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on IMDB
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-13'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4411
    true_std: 0.0112
    value_gap_source_arxiv: '2302.06299'
    value_gap_source_title: Homophily-oriented Heterogeneous Graph Rewiring
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4411
    sort_std: 0.0112
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: IMDB
      dataset_slug: imdb
main_figure: /figures/2302.06299/main_figure.jpegoptim.jpg
---

