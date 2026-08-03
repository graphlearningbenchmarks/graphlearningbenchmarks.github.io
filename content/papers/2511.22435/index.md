---
title: 'PISA: Prioritized Invariant Subgraph Aggregation'
arxiv_id: '2511.22435'
source_url: ''
authors:
- name: Ali Ghasemi
  orcid: null
  s2_author_id: '2055533949'
  s2_url: null
- name: Farooq Ahmad Wani
  orcid: null
  s2_author_id: '94816957'
  s2_url: null
- name: Maria Sofia Bucarelli
  orcid: null
  s2_author_id: '2131012031'
  s2_url: null
- name: Fabrizio Silvestri
  orcid: null
  s2_author_id: '2278436858'
  s2_url: null
published_date: Nov 27, 2025
published_date_iso: '2025-11-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Recent work has extended the invariance principle for out-of-distribution
  (OOD) generalization from Euclidean to graph data, where challenges arise due to
  complex structures and diverse distribution shifts in node attributes and topology.
  To handle these, Chen et al. proposed CIGA, which uses causal modeling and an information-theoretic
  objective to extract a single invariant subgraph capturing causal features. However,
  this single-subgraph focus can miss multiple causal patterns. addressed this with
  SuGAr, which learns and aggregates diverse invariant subgraphs via a sampler and
  diversity regularizer, improving robustness but still relying on simple uniform
  or greedy aggregation. To overcome this, the proposed PISA framework introduces
  a dynamic MLP-based aggregation that prioritizes and combines subgraph representations
  more effectively. Experiments on 15 datasets, including DrugOOD, show that PISA
  achieves up to 5\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PISA
mrr: 0.0092
adjusted_mrr: 0.0031
mrr_dataset_count: 1
benchmark_categories:
- GNNBenchmark
benchmark_coverage:
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MNIST
  rows:
  - model: 3WLGNN
    model_key: graphcon-gat
    model_plain: 3WLGNN
    value: 0.9891
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9891
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 3WLGNN
    model_key: gig-gatedgcn
    model_plain: 3WLGNN
    value: 0.988
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.00696'
    title: Graph in Graph Neural Network
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    venue: International Journal of Computer Vision
    codebase_url: https://github.com/wangjs96/Graph-in-Graph-Neural-Network
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.988
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 3WLGNN
    model_key: pncnn
    model_plain: 3WLGNN
    value: 0.9876
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
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9876
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.1051
    std: 0.0053
    paper_value: 0.1051
    paper_std: 0.0053
    metric: Accuracy
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
    source_ref: gsat
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.947
    true_std: 0.004
    value_gap_source_arxiv: '2601.20815'
    value_gap_source_title: GNN Explanations that do not Explain and How to find Them
    value_gap_source_is_current_paper: false
    value_gap: 0.8419
    has_value_note: false
    value_note: ''
    sort_value: 0.947
    sort_std: 0.004
    global_rank: 90
    paper_rank: 120
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SUGAR
    model_key: sugar
    model_plain: SUGAR
    value: 0.2849
    std: 0.1761
    paper_value: 0.2849
    paper_std: 0.1761
    metric: Accuracy
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
    table_ref: Table 2
    source_ref: sugar
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2849
    true_std: 0.1761
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2849
    sort_std: 0.1761
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PISA
    model_key: pisa
    model_plain: PISA
    value: 0.281
    std: 0.115
    paper_value: 0.281
    paper_std: 0.115
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.281
    true_std: 0.115
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.281
    sort_std: 0.115
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
  - model: V-REx
    model_key: v-rex
    model_plain: V-REx
    value: 0.1712
    std: 0.0568
    paper_value: 0.1712
    paper_std: 0.0568
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: rex
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1712
    true_std: 0.0568
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1712
    sort_std: 0.0568
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
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.1515
    std: 0.0366
    paper_value: 0.1515
    paper_std: 0.0366
    metric: Accuracy
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
    source_ref: irm
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1515
    true_std: 0.0366
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1515
    sort_std: 0.0366
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DisC
    model_key: disc
    model_plain: DisC
    value: 0.1508
    std: 0.0021
    paper_value: 0.1508
    paper_std: 0.0021
    metric: Accuracy
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
    source_ref: disc
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1508
    true_std: 0.0021
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1508
    sort_std: 0.0021
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
  - model: GREA
    model_key: grea
    model_plain: GREA
    value: 0.1392
    std: 0.0343
    paper_value: 0.1392
    paper_std: 0.0343
    metric: Accuracy
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
    source_ref: grea
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1392
    true_std: 0.0343
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1392
    sort_std: 0.0343
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.1319
    std: 0.0225
    paper_value: 0.1319
    paper_std: 0.0225
    metric: Accuracy
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
    source_ref: gil
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1319
    true_std: 0.0225
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1319
    sort_std: 0.0225
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IB-IRM
    model_key: ib-irm
    model_plain: IB-IRM
    value: 0.1306
    std: 0.0197
    paper_value: 0.1306
    paper_std: 0.0197
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: ibirm
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1306
    true_std: 0.0197
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1306
    sort_std: 0.0197
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
  - model: EIIL
    model_key: eiil
    model_plain: EIIL
    value: 0.118
    std: 0.0042
    paper_value: 0.118
    paper_std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: eiil
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.118
    true_std: 0.0042
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.118
    sort_std: 0.0042
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
  - model: Cal
    model_key: cal
    model_plain: Cal
    value: 0.1146
    std: 0.0182
    paper_value: 0.1146
    paper_std: 0.0182
    metric: Accuracy
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
    source_ref: cal
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1146
    true_std: 0.0182
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1146
    sort_std: 0.0182
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
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.1044
    std: 0.0039
    paper_value: 0.1044
    paper_std: 0.0039
    metric: Accuracy
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
    source_ref: ciga
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1044
    true_std: 0.0039
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1044
    sort_std: 0.0039
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.1026
    std: 0.0062
    paper_value: 0.1026
    paper_std: 0.0062
    metric: Accuracy
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
    source_ref: principles
    variant_inference_reason: 'dataset: fuzzy match to mnist (score=91)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OOD generalization performance under realistic graph distribution
      shifts
    date: Nov 27, 2025
    date_display: Nov 2025
    date_iso: '2025-11-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1026
    true_std: 0.0062
    value_gap_source_arxiv: '2511.22435'
    value_gap_source_title: 'PISA: Prioritized Invariant Subgraph Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1026
    sort_std: 0.0062
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: GNNBenchmark
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
single_proposed_model: PISA
---

