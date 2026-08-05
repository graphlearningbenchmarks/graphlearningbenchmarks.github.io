---
title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks with Paired Tests
  and Rank Aggregation'
arxiv_id: '2605.09099'
source_url: ''
authors:
- name: K. Costa
  orcid: null
  s2_author_id: '2313569200'
  s2_url: null
- name: Bernardo Modenesi
  orcid: null
  s2_author_id: '2080386633'
  s2_url: null
published_date: May 9, 2026
published_date_iso: '2026-05-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) benchmarks often report single point estimates,
  even when performance differences are small relative to variation across random
  seeds, train/test splits, and datasets. Confidence intervals, paired comparisons,
  multiple-comparison correction, and rank-based aggregation are standard statistical
  tools, but they are rarely the default output of graph-learning benchmark suites.
  We introduce GraphNetz, a benchmarking framework whose default output is a structured
  statistical report rather than a raw accuracy table. GraphNetz currently includes
  63 dataset loaders, four task types, and five canonical GNN architectures, while
  also supporting custom datasets and models. The framework standardizes multi-seed
  evaluation and automatically returns per-cell confidence intervals, Holm-corrected
  paired tests, and Friedman–Nemenyi critical-difference diagrams across tasks. In
  a cross-category benchmark over ten heterogeneous tasks, apparent rank differences
  among four canonical node-level encoders fall within a single Nemenyi clique, indicating
  that none is significantly better than the others at $ = 0.05$. GraphNetz therefore
  provides researchers with a reproducible computational and statistical pipeline
  to benchmark new graph-learning methods against standard architectures, over different
  tasks and a wide set of applications, while reporting principled statistical evidence
  for benchmarking which accounts for seed uncertainty. This framework is set to serve
  the graph-learning community with a reproducible and honest model comparison ready
  to be added to papers.
codebase_url: https://github.com/quant-sci/graphnetz
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: FB15k-237
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.674
    std: 0.009
    paper_value: 0.674
    paper_std: 0.009
    metric: AUC
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 9, 2026
    date_display: May 2026
    date_iso: '2026-05-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-09'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.674
    true_std: 0.009
    value_gap_source_arxiv: '2605.09099'
    value_gap_source_title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks
      with Paired Tests and Rank Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.674
    sort_std: 0.009
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.633
    std: 0.044
    paper_value: 0.633
    paper_std: 0.044
    metric: AUC
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 9, 2026
    date_display: May 2026
    date_iso: '2026-05-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-09'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.633
    true_std: 0.044
    value_gap_source_arxiv: '2605.09099'
    value_gap_source_title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks
      with Paired Tests and Rank Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.633
    sort_std: 0.044
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
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.538
    std: 0.012
    paper_value: 0.538
    paper_std: 0.012
    metric: AUC
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 9, 2026
    date_display: May 2026
    date_iso: '2026-05-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-09'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.538
    true_std: 0.012
    value_gap_source_arxiv: '2605.09099'
    value_gap_source_title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks
      with Paired Tests and Rank Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.538
    sort_std: 0.012
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.528
    std: 0.007
    paper_value: 0.528
    paper_std: 0.007
    metric: AUC
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 9, 2026
    date_display: May 2026
    date_iso: '2026-05-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-09'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.528
    true_std: 0.007
    value_gap_source_arxiv: '2605.09099'
    value_gap_source_title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks
      with Paired Tests and Rank Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.528
    sort_std: 0.007
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: FB15k-237
      dataset_slug: fb15k-237
main_figure: /figures/2605.09099/main_figure.jpegoptim.jpg
---

