---
title: Memorization in Graph Neural Networks
arxiv_id: '2508.19352'
source_url: ''
authors:
- name: Adarsh Jamadandi
  orcid: null
  s2_author_id: '151430731'
  s2_url: null
- name: Jing Xu
  orcid: null
  s2_author_id: '2348358296'
  s2_url: null
- name: Adam Dziedzic
  orcid: null
  s2_author_id: '2257345598'
  s2_url: null
- name: Franziska Boenisch
  orcid: null
  s2_author_id: '1389731564'
  s2_url: null
published_date: Aug 26, 2025
published_date_iso: '2025-08-26'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Deep neural networks (DNNs) have been shown to memorize their training data,
  yet similar analyses for graph neural networks (GNNs) remain largely under-explored.
  We introduce NCMemo (Node Classification Memorization), the first framework to quantify
  label memorization in semi-supervised node classification. We first establish an
  inverse relationship between memorization and graph homophily, the property that
  connected nodes share similar labels/features. We find that lower homophily significantly
  increases memorization, indicating that GNNs rely on memorization to learn less
  homophilic graphs. Secondly, we analyze GNN training dynamics. We find that the
  increased memorization in low homophily graphs is tightly coupled to the GNNs' implicit
  bias on using graph structure during learning. In low homophily regimes, this structure
  is less informative, hence inducing memorization of the node labels to minimize
  training loss. Finally, we show that nodes with higher label inconsistency in their
  feature-space neighborhood are significantly more prone to memorization. Building
  on our insights into the link between graph homophily and memorization, we investigate
  graph rewiring as a means to mitigate memorization. Our results demonstrate that
  this approach effectively reduces memorization without compromising model performance.
  Moreover, we show that it lowers the privacy risk for previously memorized data
  points in practice. Thus, our work not only advances understanding of GNN learning
  but also supports more privacy-preserving GNN deployment.
codebase_url: https://github.com/AdarshMJ/MemorizationinGNNs
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 13
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: Actor
  is_multi_metric: true
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.3821
    - 0.383
    metric_stds:
    - null
    - 0.0087
    - 0.006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3821
    sort_std: 0.0087
    true_value: 0.3821
    true_std: 0.0087
    paper_value: 0.3821
    paper_std: 0.0087
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - null
    - 0.3715
    - 0.37
    metric_stds:
    - null
    - 0.0071
    - 0.005
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3715
    sort_std: 0.0071
    true_value: 0.3715
    true_std: 0.0071
    paper_value: 0.3715
    paper_std: 0.0071
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    metric_values:
    - null
    - 0.3599
    - 0.359
    metric_stds:
    - null
    - 0.0113
    - 0.01
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3599
    sort_std: 0.0113
    true_value: 0.3599
    true_std: 0.0113
    paper_value: 0.3599
    paper_std: 0.0113
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  metrics:
  - Accuracy
  - Avg MemScore
  - MR
  primary_metric: Accuracy
  rank_metric: Avg MemScore
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Avg MemScore
  - MR
  metric: Avg MemScore
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: Cornell
  is_multi_metric: true
  rows:
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    metric_values:
    - null
    - 0.4102
    - 0.39
    metric_stds:
    - null
    - 0.0089
    - 0.01
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4102
    sort_std: 0.0089
    true_value: 0.4102
    true_std: 0.0089
    paper_value: 0.4102
    paper_std: 0.0089
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.3695
    - 0.365
    metric_stds:
    - null
    - 0.0153
    - 0.017
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3695
    sort_std: 0.0153
    true_value: 0.3695
    true_std: 0.0153
    paper_value: 0.3695
    paper_std: 0.0153
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - null
    - 0.3542
    - 0.35
    metric_stds:
    - null
    - 0.013
    - 0.016
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3542
    sort_std: 0.013
    true_value: 0.3542
    true_std: 0.013
    paper_value: 0.3542
    paper_std: 0.013
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  metrics:
  - Accuracy
  - Avg MemScore
  - MR
  primary_metric: Accuracy
  rank_metric: Avg MemScore
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Avg MemScore
  - MR
  metric: Avg MemScore
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Texas
  is_multi_metric: true
  rows:
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    metric_values:
    - null
    - 0.3701
    - 0.354
    - 0.6343
    metric_stds:
    - null
    - 0.0111
    - 0.014
    - 0.0122
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3701
    sort_std: 0.0111
    true_value: 0.3701
    true_std: 0.0111
    paper_value: 0.3701
    paper_std: 0.0111
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - null
    - 0.3312
    - 0.33
    - 0.9048
    metric_stds:
    - null
    - 0.0087
    - 0.011
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3312
    sort_std: 0.0087
    true_value: 0.3312
    true_std: 0.0087
    paper_value: 0.3312
    paper_std: 0.0087
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.3257
    - 0.311
    - 0.73
    metric_stds:
    - null
    - 0.0107
    - 0.012
    - 0.0221
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3257
    sort_std: 0.0107
    true_value: 0.3257
    true_std: 0.0107
    paper_value: 0.3257
    paper_std: 0.0107
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.19352'
    value_gap_source_title: Memorization in Graph Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-26'
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
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
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
  metrics:
  - Accuracy
  - Avg MemScore
  - MR
  - MemNodes LDS
  primary_metric: Accuracy
  rank_metric: Avg MemScore
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Avg MemScore
  - MR
  - MemNodes LDS
  metric: Avg MemScore
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
---

