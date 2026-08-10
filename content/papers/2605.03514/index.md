---
title: 'Revisiting Graph-Tokenizing Large Language Models: A Systematic Evaluation
  of Graph Token Understanding'
arxiv_id: '2605.03514'
source_url: ''
authors:
- name: Zhongjian Zhang
  orcid: null
  s2_author_id: '2284728816'
  s2_url: null
- name: Yue Yu
  orcid: null
  s2_author_id: '2257366050'
  s2_url: null
- name: Mengmei Zhang
  orcid: null
  s2_author_id: '16003017'
  s2_url: null
- name: Junping Du
  orcid: null
  s2_author_id: '2260277448'
  s2_url: null
- name: Xiao Wang
  orcid: null
  s2_author_id: '2118449003'
  s2_url: null
- name: Chuan Shi
  orcid: null
  s2_author_id: '2151458697'
  s2_url: null
published_date: May 5, 2026
published_date_iso: '2026-05-05'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'The remarkable success of large language models (LLMs) has motivated researchers
  to adapt them as universal predictors for various graph tasks. As a widely recognized
  paradigm, Graph-Tokenizing LLMs (GTokenLLMs) compress complex graph data into graph
  tokens and treat them as prefix tokens for querying LLMs, leading many to believe
  that LLMs can understand graphs more effectively and efficiently. In this paper,
  we challenge this belief: Do GTokenLLMs fully understand graph tokens in the natural-language
  embedding space? Motivated by this question, we formalize a unified framework for
  GTokenLLMs and propose an evaluation pipeline, GTEval, to assess graph-token understanding
  via instruction transformations at the format and content levels. We conduct extensive
  experiments on 6 representative GTokenLLMs with GTEval. The primary findings are
  as follows: (1) Existing GTokenLLMs do not fully understand graph tokens. They exhibit
  over-sensitivity or over-insensitivity to instruction changes, and rely heavily
  on text for reasoning; (2) Although graph tokens preserve task-relevant graph information
  and receive attention across LLM layers, their utilization varies across models
  and instruction variants; (3) Additional instruction tuning can improve performance
  on the original and seen instructions, but it does not fully address the challenge
  of graph-token understanding, calling for further improvement.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: InstructGLM
    model_key: instructglm
    model_plain: InstructGLM
    value: 0.7859
    std: null
    paper_value: 0.7859
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: instructglm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Original instruction accuracy on Cora node classification
    date: May 5, 2026
    date_display: May 2026
    date_iso: '2026-05-05'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9077
    at_pub_std: null
    at_pub_source_arxiv: '2310.16421'
    at_pub_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.12179999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9077
    true_std: null
    value_gap_source_arxiv: '2310.16421'
    value_gap_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.12179999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9077
    sort_std: null
    global_rank: 24
    paper_rank: 787
    rank_delta: 763
    rank_delta_abs: 763
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    comparison_source_arxiv: '2310.16421'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9004
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 31
    sort_value: 0.9004
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.8745
    std: null
    paper_value: 0.8745
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chenllaga
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Original instruction accuracy on Cora node classification
    date: May 5, 2026
    date_display: May 2026
    date_iso: '2026-05-05'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8125
    at_pub_std: null
    at_pub_source_arxiv: '2406.10727'
    at_pub_source_title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks
      and New Insights'
    at_pub_source_date_iso: '2024-06-15'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-05-05'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.062000000000000055
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8745
    true_std: null
    value_gap_source_arxiv: '2605.03514'
    value_gap_source_title: 'Revisiting Graph-Tokenizing Large Language Models: A
      Systematic Evaluation of Graph Token Understanding'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8745
    sort_std: null
    global_rank: 162
    paper_rank: 162
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks
      and New Insights'
    comparison_source_arxiv: '2406.10727'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7768
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 806
    sort_value: 0.7768
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
main_figure: /figures/2605.03514/main_figure.jpegoptim.jpg
---

