---
title: A Unified Graph Language Model for Multi-Domain Multi-Task Graph Alignment
  Instruction Tuning
arxiv_id: '2605.12197'
source_url: ''
authors:
- name: Haibo Chen
  orcid: null
  s2_author_id: '2319215755'
  s2_url: null
- name: Xin Wang
  orcid: null
  s2_author_id: '2153687490'
  s2_url: null
- name: Jiaheng Chao
  orcid: null
  s2_author_id: '2434929080'
  s2_url: null
- name: Ling Feng
  orcid: null
  s2_author_id: '2152749977'
  s2_url: null
- name: Wenwu Zhu
  orcid: null
  s2_author_id: '2156154955'
  s2_url: null
published_date: May 12, 2026
published_date_iso: '2026-05-12'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Leveraging Graph Neural Networks (GNNs) as graph encoders and aligning
  the resulting representations with Large Language Models (LLMs) through alignment
  instruction tuning has become a mainstream paradigm for constructing Graph Language
  Models (GLMs), combining the generalization ability of LLMs with the structural
  modeling capacity of GNNs. However, existing GLMs that adopt GNNs as graph encoders
  largely overlook the problem of aligning GNN-encoded representations across domains
  and tasks with the LLM token space to obtain unified graph tokens, thereby limiting
  their ability to generalize across diverse graph data. To bridge this gap, we aim
  to incorporate a multi-domain, multi-task GNN encoder into GLMs and align its representations
  with LLMs to enable multi-domain, multi-task graph alignment instruction tuning.
  This alignment problem remains underexplored and poses two key challenges: 1) learning
  GNN-encoded representations that are simultaneously generalizable across domains
  and tasks and well aligned with textual semantics is difficult, due to substantial
  variations in graph structures, feature distributions, and supervision signals,
  together with the lack of textual-semantic alignment guidance in task-specific GNN
  training; 2) diverse graph data and task-specific instructions can exhibit different
  degrees of compatibility with the LLM token space during instruction tuning, leading
  to varying alignment difficulty and rendering a fixed alignment strategy suboptimal.
  To tackle these challenges, we propose UniGraphLM, a Unified Graph Language Model
  that incorporates a multi-domain, multi-task GNN encoder to learn generalizable
  graph representations aligned with textual semantics, and then adaptively aligns
  these representations with the LLM. Specifically, we first develop a graph-text
  pair pretraining strategy with a tailored GNN encoder, trained on large-scale graph-text
  data spanning multiple domains and tasks to obtain generalizable representations
  naturally aligned with textual semantics. We further design a curriculum alignment
  tuning strategy that adaptively adjusts the alignment process by accounting for
  varying alignment difficulty across diverse graph data. Extensive experiments demonstrate
  that UniGraphLM consistently outperforms state-of-the-art baselines across graph
  datasets from different domains and tasks.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LLMs
mrr: 0.0
adjusted_mrr: 0.0
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
  dataset: WN18RR
  is_multi_metric: true
  rows:
  - model: LLMs
    model_key: llms
    model_plain: LLMs
    metric_values:
    - null
    - 0.9352
    - 0.753
    metric_stds:
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
    sort_value: 0.9352
    sort_std: null
    true_value: 0.9352
    true_std: null
    paper_value: 0.9352
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2605.12197'
    value_gap_source_title: A Unified Graph Language Model for Multi-Domain Multi-Task
      Graph Alignment Instruction Tuning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
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
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
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
  - model: TEA-GLM
    model_key: tea-glm
    model_plain: TEA-GLM
    metric_values:
    - null
    - 0.9285
    - 0.7382
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.9285
    sort_std: null
    true_value: 0.9285
    true_std: null
    paper_value: 0.9285
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2605.12197'
    value_gap_source_title: A Unified Graph Language Model for Multi-Domain Multi-Task
      Graph Alignment Instruction Tuning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
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
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
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
  - model: Vicuna-7B
    model_key: vicuna-7b
    model_plain: Vicuna-7B
    metric_values:
    - null
    - 0.3484
    - 0.1214
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.3484
    sort_std: null
    true_value: 0.3484
    true_std: null
    paper_value: 0.3484
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2605.12197'
    value_gap_source_title: A Unified Graph Language Model for Multi-Domain Multi-Task
      Graph Alignment Instruction Tuning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
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
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
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
  - model: LLaMA-2-7B
    model_key: llama-2-7b
    model_plain: LLaMA-2-7B
    metric_values:
    - null
    - 0.2916
    - 0.0754
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.2916
    sort_std: null
    true_value: 0.2916
    true_std: null
    paper_value: 0.2916
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2605.12197'
    value_gap_source_title: A Unified Graph Language Model for Multi-Domain Multi-Task
      Graph Alignment Instruction Tuning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
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
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
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
  - model: GOFA
    model_key: gofa
    model_plain: GOFA
    metric_values:
    - null
    - 0.2195
    - 0.1
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.2195
    sort_std: null
    true_value: 0.2195
    true_std: null
    paper_value: 0.2195
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2605.12197'
    value_gap_source_title: A Unified Graph Language Model for Multi-Domain Multi-Task
      Graph Alignment Instruction Tuning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
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
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
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
  metrics:
  - MRR
  - ACC
  - F1
  primary_metric: MRR
  rank_metric: ACC
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - ACC
  - F1
  metric: ACC
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
    - dataset: WN18RR
      dataset_slug: wn18rr
single_proposed_model: LLMs
---

