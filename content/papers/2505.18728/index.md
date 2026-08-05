---
title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern Sequence
  Modeling'
arxiv_id: '2505.18728'
source_url: ''
authors:
- name: Andrea Ceni
  orcid: null
  s2_author_id: '51152603'
  s2_url: null
- name: Alessio Gravina
  orcid: null
  s2_author_id: '2042289369'
  s2_url: null
- name: C. Gallicchio
  orcid: null
  s2_author_id: '2158038'
  s2_url: null
- name: Davide Bacciu
  orcid: null
  s2_author_id: '2294893543'
  s2_url: null
- name: C. Schönlieb
  orcid: null
  s2_author_id: '1711104'
  s2_url: null
- name: Moshe Eliasof
  orcid: null
  s2_author_id: '104172497'
  s2_url: null
published_date: May 24, 2025
published_date_iso: '2025-05-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: The recent success of State-Space Models (SSMs) in sequence modeling has
  motivated their adaptation to graph learning, giving rise to Graph State-Space Models
  (GSSMs). However, existing GSSMs operate by applying SSM modules to sequences extracted
  from graphs, often compromising core properties such as permutation equivariance,
  message-passing compatibility, and computational efficiency. In this paper, we introduce
  a new perspective by embedding the key principles of modern SSM computation directly
  into the Message-Passing Neural Network framework, resulting in a unified methodology
  for both static and temporal graphs. Our approach, MP-SSM, enables efficient, permutation-equivariant,
  and long-range information propagation while preserving the architectural simplicity
  of message passing. Crucially, MP-SSM enables an exact sensitivity analysis, which
  we use to theoretically characterize information flow and evaluate issues like vanishing
  gradients and over-squashing in the deep regime. Furthermore, our design choices
  allow for a highly optimized parallel implementation akin to modern SSMs. We validate
  MP-SSM across a wide range of tasks, including node classification, graph property
  prediction, long-range benchmarks, and spatiotemporal forecasting, demonstrating
  both its versatility and strong empirical performance.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MP-SSM
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Algorithmic Graph Tasks
benchmark_coverage:
- benchmark: Algorithmic Graph Tasks
  benchmark_slug: algorithmic-graph-tasks
  evaluated: 2
  total: 2
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
  dataset: Eccentricity
  rows:
  - model: MP-SSM
    model_key: mp-ssm
    model_plain: MP-SSM
    value: -2.9724
    std: 0.0271
    paper_value: -2.9724
    paper_std: 0.0271
    metric: MSE
    higher_is_better: false
    is_baseline: false
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -2.9724
    sort_std: 0.0271
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: A-DGN
    model_key: odes
    model_plain: A-DGN
    value: 0.3046
    std: 0.1181
    metric: MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_display: Oct 2022
    date_iso: '2022-10-18'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.3046
    sort_std: 0.1181
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.6077
    std: 0.0282
    paper_value: 0.6077
    paper_std: 0.0282
    metric: MSE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6077
    sort_std: 0.0282
    global_rank: 2
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.6602
    std: 0.1393
    paper_value: 0.6602
    paper_std: 0.1393
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6602
    at_pub_std: 0.1393
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6602
    true_std: 0.1393
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6602
    sort_std: 0.1393
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
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.6833
    std: 0.0074
    paper_value: 0.6833
    paper_std: 0.0074
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6833
    sort_std: 0.0074
    global_rank: 3
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-DGN
    model_key: a-dgn
    model_plain: A-DGN
    value: 0.4296
    std: 0.1003
    paper_value: 0.4296
    paper_std: 0.1003
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7177
    at_pub_std: 0.0345
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.2881
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7177
    true_std: 0.0345
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.2881
    has_value_note: false
    value_note: ''
    sort_value: 0.7177
    sort_std: 0.0345
    global_rank: 3
    paper_rank: 2
    rank_delta: -1
    rank_delta_abs: 1
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    comparison_source_arxiv: '2210.09789'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.764
    std: 0.0355
    paper_value: 0.764
    paper_std: 0.0355
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.764
    at_pub_std: 0.0355
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.764
    true_std: 0.0355
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.764
    sort_std: 0.0355
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7863
    std: 0.0207
    paper_value: 0.7863
    paper_std: 0.0207
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7863
    at_pub_std: 0.0207
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7863
    true_std: 0.0207
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7863
    sort_std: 0.0207
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7909
    std: 0.0222
    paper_value: 0.7909
    paper_std: 0.0222
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7909
    at_pub_std: 0.0222
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7909
    true_std: 0.0222
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7909
    sort_std: 0.0222
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
  - model: DGC
    model_key: dgc
    model_plain: DGC
    value: 0.8261
    std: 0.0032
    paper_value: 0.8261
    paper_std: 0.0032
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8261
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8261
    true_std: 0.0032
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8261
    sort_std: 0.0032
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8468
    std: 0.0028
    paper_value: 0.8468
    paper_std: 0.0028
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8468
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8468
    true_std: 0.0028
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8468
    sort_std: 0.0028
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.9504
    std: 0.0007
    paper_value: 0.9504
    paper_std: 0.0007
    metric: MSE
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9504
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-18'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9504
    true_std: 0.0007
    value_gap_source_arxiv: '2210.09789'
    value_gap_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9504
    sort_std: 0.0007
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
  rank_metric: MSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MSE
  paper_metrics:
  - MSE
  metric: MSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: SSSP
  rows:
  - model: MP-SSM
    model_key: mp-ssm
    model_plain: MP-SSM
    value: -4.6321
    std: 0.0779
    paper_value: -4.6321
    paper_std: 0.0779
    metric: log10(MSE)
    higher_is_better: false
    is_baseline: false
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -4.6321
    sort_std: 0.0779
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: -3.599
    std: 0.1949
    paper_value: -3.599
    paper_std: 0.1949
    metric: log10(MSE)
    higher_is_better: false
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -3.599
    sort_std: 0.1949
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-DGN
    model_key: a-dgn
    model_plain: A-DGN
    value: -3.2417
    std: 0.0751
    paper_value: -3.2417
    paper_std: 0.0751
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -3.2417
    sort_std: 0.0751
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: -1.3836
    std: 0.0092
    paper_value: -1.3836
    paper_std: 0.0092
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -1.3836
    sort_std: 0.0092
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: -1.1329
    std: 0.0135
    paper_value: -1.1329
    paper_std: 0.0135
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -1.1329
    sort_std: 0.0135
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: -0.5408
    std: 0.4193
    paper_value: -0.5408
    paper_std: 0.4193
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -0.5408
    sort_std: 0.4193
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGC
    model_key: dgc
    model_plain: DGC
    value: -0.1483
    std: 0.0231
    paper_value: -0.1483
    paper_std: 0.0231
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -0.1483
    sort_std: 0.0231
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: -0.0942
    std: 0.3897
    paper_value: -0.0942
    paper_std: 0.3897
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: -0.0942
    sort_std: 0.3897
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.2863
    std: 0.1843
    paper_value: 0.2863
    paper_std: 0.1843
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2863
    true_std: 0.1843
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2863
    sort_std: 0.1843
    global_rank: 1
    paper_rank: 1
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
    value: 0.6951
    std: 0.1499
    paper_value: 0.6951
    paper_std: 0.1499
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6951
    true_std: 0.1499
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6951
    sort_std: 0.1499
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9499
    std: 0.0001
    paper_value: 0.9499
    paper_std: 0.0001
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 24, 2025
    date_display: May 2025
    date_iso: '2025-05-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9499
    true_std: 0.0001
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9499
    sort_std: 0.0001
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
  rank_metric: log10(MSE)
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MSE
  paper_metrics:
  - log10(MSE)
  metric: log10(MSE)
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Algorithmic Graph Tasks
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Algorithmic Graph Tasks
    benchmark_slug: algorithmic-graph-tasks
    datasets:
    - dataset: SSSP
      dataset_slug: sssp
    - dataset: Eccentricity
      dataset_slug: eccentricity
single_proposed_model: MP-SSM
main_figure: /figures/2505.18728/main_figure.jpegoptim.jpg
---

