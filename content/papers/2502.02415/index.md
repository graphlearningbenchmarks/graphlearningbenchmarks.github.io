---
title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
arxiv_id: '2502.02415'
source_url: ''
authors:
- name: Markus Krimmel
  orcid: null
  s2_author_id: '2343749545'
  s2_url: null
- name: Jenna Wiens
  orcid: null
  s2_author_id: '2343749548'
  s2_url: null
- name: Karsten M. Borgwardt
  orcid: null
  s2_author_id: '2268189981'
  s2_url: null
- name: Dexiong Chen
  orcid: null
  s2_author_id: '2322616706'
  s2_url: null
published_date: Feb 4, 2025
published_date_iso: '2025-02-04'
published_venue: TMLR 2025
published_conference: TMLR 2025
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Existing graph generative models often face a critical trade-off between
  sample quality and generation speed. We introduce Autoregressive Noisy Filtration
  Modeling (ANFM), a flexible autoregressive framework that addresses both challenges.
  ANFM leverages filtration, a concept from topological data analysis, to transform
  graphs into short sequences of subgraphs. We identify exposure bias as a potential
  hurdle in autoregressive graph generation and propose noise augmentation and reinforcement
  learning as effective mitigation strategies, which allow ANFM to learn both edge
  addition and deletion operations. This unique capability enables ANFM to correct
  errors during generation by modeling non-monotonic graph sequences. Our results
  show that ANFM matches state-of-the-art diffusion models in quality while offering
  over 100 times faster inference, making it a promising approach for high-throughput
  graph generation. The source code is publicly available at.
codebase_url: https://github.com/BorgwardtLab/anfm
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphRNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 1
  total: 5
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: RB graph
  rows:
  - model: ANFM (DFS)
    model_key: anfm (dfs)
    model_plain: ANFM (DFS)
    value: 65.0
    std: null
    paper_value: 65.0
    paper_std: null
    metric: VUN
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 65.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 65.0
    sort_std: null
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
  - model: DiGress
    model_key: digress
    model_plain: DiGress
    value: 60.0
    std: null
    paper_value: 60.0
    paper_std: null
    metric: VUN
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
    table_ref: Table 1
    source_ref: bergmeister2024efficientscalable
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.0
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SPECTRE
    model_key: spectre
    model_plain: SPECTRE
    value: 52.5
    std: null
    paper_value: 52.5
    paper_std: null
    metric: VUN
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
    table_ref: Table 1
    source_ref: martinkus2022spectre
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 52.5
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 52.5
    sort_std: null
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
  - model: ESGG
    model_key: esgg
    model_plain: ESGG
    value: 45.0
    std: null
    paper_value: 45.0
    paper_std: null
    metric: VUN
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
    table_ref: Table 1
    source_ref: bergmeister2024efficientscalable
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 45.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 45.0
    sort_std: null
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
  - model: GRAN
    model_key: gran
    model_plain: GRAN
    value: 25.0
    std: null
    paper_value: 25.0
    paper_std: null
    metric: VUN
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
    table_ref: Table 1
    source_ref: martinkus2022spectre
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 25.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 25.0
    sort_std: null
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
  - model: GraphRNN
    model_key: graphrnn
    model_plain: GraphRNN
    value: 5.0
    std: null
    paper_value: 5.0
    paper_std: null
    metric: VUN
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: martinkus2022spectre
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 5.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 5.0
    sort_std: null
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
  - model: Edge
    model_key: edge
    model_plain: Edge
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
    metric: VUN
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
    table_ref: Table 1
    source_ref: bergmeister2024efficientscalable
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard evaluation on SBM dataset with N_train=128
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0
    true_std: null
    value_gap_source_arxiv: '2502.02415'
    value_gap_source_title: Fast Graph Generation via Autoregressive Noisy Filtration
      Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0
    sort_std: null
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
  rank_metric: VUN
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - VUN
  metric: VUN
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: GraphBench
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: RB graph
      dataset_slug: rb-graph
single_proposed_model: GraphRNN
---

