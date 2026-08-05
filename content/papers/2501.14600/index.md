---
title: 'On the Cross-type Homophily of Heterogeneous Graphs: Understanding and Unleashing'
arxiv_id: '2501.14600'
source_url: ''
authors:
- name: Zhen Tao
  orcid: null
  s2_author_id: '2342277664'
  s2_url: null
- name: Ziyue Qiao
  orcid: null
  s2_author_id: '2321832492'
  s2_url: null
- name: Chaoqi Chen
  orcid: null
  s2_author_id: '2335149610'
  s2_url: null
- name: Zhengyi Yang
  orcid: null
  s2_author_id: '150358651'
  s2_url: null
- name: Lun Du
  orcid: null
  s2_author_id: '2343704309'
  s2_url: null
- name: Qingqiang Sun
  orcid: null
  s2_author_id: '49144737'
  s2_url: null
published_date: Jan 24, 2025
published_date_iso: '2025-01-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Homophily, the tendency of similar nodes to connect, is a fundamental phenomenon
  in network science and a critical factor in the performance of graph neural networks
  (GNNs). While existing studies primarily explore homophily in homogeneous graphs,
  where nodes share the same type, real-world networks are often more accurately modeled
  as heterogeneous graphs (HGs) with diverse node types and intricate cross-type interactions.
  This structural diversity complicates the analysis of homophily, as traditional
  homophily metrics fail to account for distinct label spaces across node types. To
  address this limitation, we introduce the Cross-Type Homophily Ratio (CHR), a novel
  metric that quantifies homophily based on the similarity of target information across
  different node types. Additionally, we propose Cross-Type Homophily-guided Graph
  Editing (CTHGE), a novel method for improving heterogeneous graph neural networks
  (HGNNs) performance by optimizing cross-type connectivity using Cross-Type Homophily
  Ratio. Extensive experiments on five HG datasets with nine HGNNs validate the effectiveness
  of CTHGE, which delivers a maximum relative performance improvement of over 25\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CTHGE
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Actor
  is_multi_metric: true
  rows:
  - model: CTHGE
    model_key: cthge
    model_plain: CTHGE
    metric_values:
    - null
    - 0.8258
    - 0.8248
    metric_stds:
    - null
    - 0.0039
    - 0.0092
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.8258
    sort_std: 0.0039
    true_value: 0.8258
    true_std: 0.0039
    paper_value: 0.8258
    paper_std: 0.0039
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: HDHGR
    model_key: hgt hdhgr
    model_plain: HDHGR
    metric_values:
    - 0.7725
    - null
    - null
    metric_stds:
    - 0.0053
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.06299'
    title: Homophily-oriented Heterogeneous Graph Rewiring
    published_venue: ''
    date: Feb 13, 2023
    date_display: Feb 2023
    date_iso: '2023-02-13'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.7725
    sort_std: 0.0053
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
  - model: PSHGCN
    model_key: pshgcn
    model_plain: PSHGCN
    metric_values:
    - null
    - 0.762
    - 0.6716
    metric_stds:
    - null
    - 0.0128
    - 0.0112
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.762
    sort_std: 0.0128
    true_value: 0.762
    true_std: 0.0128
    paper_value: 0.762
    paper_std: 0.0128
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: SHGN
    model_key: shgn
    model_plain: SHGN
    metric_values:
    - null
    - 0.7063
    - 0.7895
    metric_stds:
    - null
    - 0.0093
    - 0.0118
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7063
    sort_std: 0.0093
    true_value: 0.7063
    true_std: 0.0093
    paper_value: 0.7063
    paper_std: 0.0093
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: HAN
    model_key: han
    model_plain: HAN
    metric_values:
    - null
    - 0.6943
    - 0.5654
    metric_stds:
    - null
    - 0.0022
    - 0.0094
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6943
    sort_std: 0.0022
    true_value: 0.6943
    true_std: 0.0022
    paper_value: 0.6943
    paper_std: 0.0022
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    metric_values:
    - null
    - 0.6562
    - 0.7831
    metric_stds:
    - null
    - 0.0134
    - 0.0101
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6562
    sort_std: 0.0134
    true_value: 0.6562
    true_std: 0.0134
    paper_value: 0.6562
    paper_std: 0.0134
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    metric_values:
    - null
    - 0.5142
    - 0.6313
    metric_stds:
    - null
    - 0.0121
    - 0.0134
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5142
    sort_std: 0.0121
    true_value: 0.5142
    true_std: 0.0121
    paper_value: 0.5142
    paper_std: 0.0121
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    metric_values:
    - null
    - 0.506
    - 0.5583
    metric_stds:
    - null
    - 0.0102
    - 0.0112
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.506
    sort_std: 0.0102
    true_value: 0.506
    true_std: 0.0102
    paper_value: 0.506
    paper_std: 0.0102
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.4878
    - 0.6185
    metric_stds:
    - null
    - 0.013
    - 0.0141
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4878
    sort_std: 0.013
    true_value: 0.4878
    true_std: 0.013
    paper_value: 0.4878
    paper_std: 0.013
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
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
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    metric_values:
    - null
    - 0.4772
    - 0.6305
    metric_stds:
    - null
    - 0.0134
    - 0.0059
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.4772
    sort_std: 0.0134
    true_value: 0.4772
    true_std: 0.0134
    paper_value: 0.4772
    paper_std: 0.0134
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - null
    - 0.4565
    - 0.6126
    metric_stds:
    - null
    - 0.0103
    - 0.0102
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4565
    sort_std: 0.0103
    true_value: 0.4565
    true_std: 0.0103
    paper_value: 0.4565
    paper_std: 0.0103
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.14600'
    value_gap_source_title: 'On the Cross-type Homophily of Heterogeneous Graphs:
      Understanding and Unleashing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-24'
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
    date: Jan 24, 2025
    date_display: Jan 2025
    date_iso: '2025-01-24'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 30
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
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
single_proposed_model: CTHGE
main_figure: /figures/2501.14600/main_figure.jpegoptim.jpg
---

