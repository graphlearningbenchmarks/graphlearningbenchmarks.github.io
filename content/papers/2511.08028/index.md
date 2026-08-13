---
title: Generalizable Insights for Graph Transformers in Theory and Practice
arxiv_id: '2511.08028'
source_url: ''
authors:
- name: Timo Stoll
  orcid: null
  s2_author_id: '2373023981'
  s2_url: null
- name: Luis Müller
  orcid: null
  s2_author_id: '2282283890'
  s2_url: null
- name: Christopher Morris
  orcid: null
  s2_author_id: '2257004525'
  s2_url: null
published_date: Nov 11, 2025
published_date_iso: '2025-11-11'
published_venue: NeurIPS 2025
published_conference: NeurIPS 2025
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph Transformers (GTs) have shown strong empirical performance, yet current
  architectures vary widely in their use of attention mechanisms, positional embeddings
  (PEs), and expressivity. Existing expressivity results are often tied to specific
  design choices and lack comprehensive empirical validation on large-scale data.
  This leaves a gap between theory and practice, preventing generalizable insights
  that exceed particular application domains. Here, we propose the Generalized-Distance
  Transformer (GDT), a GT architecture using standard attention that incorporates
  many advancements for GTs from recent years, and develop a fine-grained understanding
  of the GDT's representation power in terms of attention and PEs. Through extensive
  experiments, we identify design choices that consistently perform well across various
  applications, tasks, and model scales, demonstrating strong performance in a few-shot
  transfer setting without fine-tuning. Our evaluation covers over eight million graphs
  with roughly 270M tokens across diverse domains, including image-based object detection,
  molecular property prediction, code summarization, and out-of-distribution algorithmic
  reasoning. We distill our theoretical and practical findings into several generalizable
  insights about effective GT design, training, and inference.
codebase_url: https://github.com/GraphPKU/BREC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- GraphBench
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 1
  total: 5
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
  dataset: Flow
  rows:
  - model: RRWP
    model_key: rrwp
    model_plain: RRWP
    value: 1.45
    std: 0.06
    paper_value: 1.45
    paper_std: 0.06
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: RRWP is a relative positional encoding used in the attention
      bias.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on Flow dataset using 16M parameter GDT with RRWP.
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.45
    true_std: 0.06
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.45
    sort_std: 0.06
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
  - model: RWSE
    model_key: rwse
    model_plain: RWSE
    value: 1.49
    std: 0.02
    paper_value: 1.49
    paper_std: 0.02
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: RWSE is an absolute positional encoding added to node
      embeddings.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on Flow dataset using 16M parameter GDT with RWSE.
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.49
    true_std: 0.02
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.49
    sort_std: 0.02
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
  - model: NoPE
    model_key: nope
    model_plain: NoPE
    value: 1.73
    std: 0.09
    paper_value: 1.73
    paper_std: 0.09
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: NoPE (No Positional Encoding) uses only the adjacency/node
      features.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on Flow dataset using 16M parameter GDT with NoPE.
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.73
    true_std: 0.09
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.73
    sort_std: 0.09
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
  - model: LPE
    model_key: lpe
    model_plain: LPE
    value: 1.75
    std: 0.12
    paper_value: 1.75
    paper_std: 0.12
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: LPE is an absolute positional encoding added to node
      embeddings.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on Flow dataset using 16M parameter GDT with LPE.
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.75
    true_std: 0.12
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.75
    sort_std: 0.12
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
  - model: SPE
    model_key: spe
    model_plain: SPE
    value: 1.98
    std: 0.14
    paper_value: 1.98
    paper_std: 0.14
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: SPE is an absolute positional encoding added to node
      embeddings.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on Flow dataset using 16M parameter GDT with SPE.
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.98
    true_std: 0.14
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.98
    sort_std: 0.14
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
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ogbg-code2
  rows:
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.206
    std: 0.002
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_display: Sep 2025
    date_iso: '2025-09-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.206
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DirGraphSSM
    model_key: dirgraphssm
    model_plain: DirGraphSSM
    value: 0.205
    std: 0.0023
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_display: Sep 2025
    date_iso: '2025-09-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.205
    sort_std: 0.0023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graph-Mamba
    model_key: graph-mamba
    model_plain: Graph-Mamba
    value: 0.203
    std: 0.0023
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_display: Sep 2025
    date_iso: '2025-09-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.203
    sort_std: 0.0023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LPE
    model_key: lpe
    model_plain: LPE
    value: 0.1948
    std: 0.0021
    paper_value: 0.1948
    paper_std: 0.0021
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test F1 on Code dataset
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1948
    true_std: 0.0021
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1948
    sort_std: 0.0021
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
  - model: RRWP
    model_key: rrwp
    model_plain: RRWP
    value: 0.1942
    std: 0.001
    paper_value: 0.1942
    paper_std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test F1 on Code dataset
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1942
    true_std: 0.001
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1942
    sort_std: 0.001
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
  - model: RWSE
    model_key: rwse
    model_plain: RWSE
    value: 0.1939
    std: 0.0047
    paper_value: 0.1939
    paper_std: 0.0047
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test F1 on Code dataset
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1939
    true_std: 0.0047
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1939
    sort_std: 0.0047
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SPE
    model_key: spe
    model_plain: SPE
    value: 0.1935
    std: 0.0021
    paper_value: 0.1935
    paper_std: 0.0021
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test F1 on Code dataset
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1935
    true_std: 0.0021
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1935
    sort_std: 0.0021
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
  - model: NoPE
    model_key: nope
    model_plain: NoPE
    value: 0.1927
    std: 0.002
    paper_value: 0.1927
    paper_std: 0.002
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test F1 on Code dataset
    date: Nov 11, 2025
    date_display: Nov 2025
    date_iso: '2025-11-11'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-11'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1927
    true_std: 0.002
    value_gap_source_arxiv: '2511.08028'
    value_gap_source_title: Generalizable Insights for Graph Transformers in Theory
      and Practice
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1927
    sort_std: 0.002
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.151
    std: 0.002
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_display: Sep 2025
    date_iso: '2025-09-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 39
    sort_value: 0.151
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
- benchmark: GraphBench
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-code2
      dataset_slug: ogbg-code2
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: Flow
      dataset_slug: flow
main_figure: /figures/2511.08028/main_figure.jpegoptim.jpg
---

