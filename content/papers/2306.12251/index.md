---
title: 'GADBench: Revisiting and Benchmarking Supervised Graph Anomaly Detection'
arxiv_id: '2306.12251'
source_url: ''
authors:
- name: Jianheng Tang
  orcid: null
  s2_author_id: '66239746'
  s2_url: null
- name: Fengrui Hua
  orcid: null
  s2_author_id: '2156737826'
  s2_url: null
- name: Zi-Chao Gao
  orcid: null
  s2_author_id: '120267993'
  s2_url: null
- name: P. Zhao
  orcid: null
  s2_author_id: '144259957'
  s2_url: null
- name: Jia Li
  orcid: null
  s2_author_id: '2196671991'
  s2_url: null
published_date: Jun 21, 2023
published_date_iso: '2023-06-21'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: With a long history of traditional Graph Anomaly Detection (GAD) algorithms
  and recently popular Graph Neural Networks (GNNs), it is still not clear (1) how
  they perform under a standard comprehensive setting, (2) whether GNNs can outperform
  traditional algorithms such as tree ensembles, and (3) how about their efficiency
  on large-scale graphs. In response, we introduce GADBench---a benchmark tool dedicated
  to supervised anomalous node detection in static graphs. GADBench facilitates a
  detailed comparison across 29 distinct models on ten real-world GAD datasets, encompassing
  thousands to millions ($ $6M) nodes. Our main finding is that tree ensembles with
  simple neighborhood aggregation can outperform the latest GNNs tailored for the
  GAD task. We shed light on the current progress of GAD, setting a robust groundwork
  for subsequent investigations in this domain. GADBench is open-sourced at.
codebase_url: https://github.com/squareRoot3/GADBench
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Amazon2M
  rows:
  - model: XGB-Graph
    model_key: xgb-graph
    model_plain: XGB-Graph
    value: 0.9333
    std: null
    paper_value: 0.9333
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9333
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9333
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
  - model: XGBOD
    model_key: xgbod
    model_plain: XGBOD
    value: 0.9215
    std: null
    paper_value: 0.9215
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9215
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9215
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
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.9188
    std: null
    paper_value: 0.9188
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9188
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9188
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
  - model: NA
    model_key: na
    model_plain: NA
    value: 0.9156
    std: null
    paper_value: 0.9156
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9156
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9156
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
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.9148
    std: null
    paper_value: 0.9148
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9148
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9148
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
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.9118
    std: null
    paper_value: 0.9118
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9118
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9118
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
  - model: RF-Graph
    model_key: rf-graph
    model_plain: RF-Graph
    value: 0.9053
    std: null
    paper_value: 0.9053
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9053
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9053
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
  - model: GHRN
    model_key: ghrn
    model_plain: GHRN
    value: 0.8952
    std: null
    paper_value: 0.8952
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8952
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8952
    sort_std: null
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
  - model: PCGNN
    model_key: pcgnn
    model_plain: PCGNN
    value: 0.8933
    std: null
    paper_value: 0.8933
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8933
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8933
    sort_std: null
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
  - model: AMNet
    model_key: amnet
    model_plain: AMNet
    value: 0.8836
    std: null
    paper_value: 0.8836
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8836
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8836
    sort_std: null
    global_rank: 10
    paper_rank: 10
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
    value: 0.8794
    std: null
    paper_value: 0.8794
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8794
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8794
    sort_std: null
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8734
    std: null
    paper_value: 0.8734
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8734
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8734
    sort_std: null
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
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.858
    std: null
    paper_value: 0.858
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.858
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.858
    sort_std: null
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCI
    model_key: dci
    model_plain: DCI
    value: 0.8517
    std: null
    paper_value: 0.8517
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8517
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8517
    sort_std: null
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
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.849
    std: null
    paper_value: 0.849
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.849
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.849
    sort_std: null
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8489
    std: null
    paper_value: 0.8489
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8489
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8489
    sort_std: null
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.8472
    std: null
    paper_value: 0.8472
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8472
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8472
    sort_std: null
    global_rank: 17
    paper_rank: 17
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
    value: 0.8461
    std: null
    paper_value: 0.8461
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8461
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8461
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KNN
    model_key: knn
    model_plain: KNN
    value: 0.8441
    std: null
    paper_value: 0.8441
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8441
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8441
    sort_std: null
    global_rank: 19
    paper_rank: 19
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
    value: 0.8245
    std: null
    paper_value: 0.8245
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8245
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8245
    sort_std: null
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAS
    model_key: gas
    model_plain: GAS
    value: 0.8143
    std: null
    paper_value: 0.8143
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8143
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8143
    sort_std: null
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGNN
    model_key: bgnn
    model_plain: BGNN
    value: 0.6792
    std: null
    paper_value: 0.6792
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6792
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6792
    sort_std: null
    global_rank: 22
    paper_rank: 22
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
    value: 0.4565
    std: null
    paper_value: 0.4565
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4565
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4565
    sort_std: null
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4269
    std: null
    paper_value: 0.4269
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4269
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4269
    sort_std: null
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.3524
    std: null
    paper_value: 0.3524
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3524
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3524
    sort_std: null
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
  rank_metric: AUPRC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUPRC
  metric: AUPRC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Reddit
  rows:
  - model: NA
    model_key: na
    model_plain: NA
    value: 0.097
    std: null
    paper_value: 0.097
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.097
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.097
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
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.0832
    std: null
    paper_value: 0.0832
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0832
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0832
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
  - model: XGBOD
    model_key: xgbod
    model_plain: XGBOD
    value: 0.0827
    std: null
    paper_value: 0.0827
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0827
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0827
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
  - model: AMNet
    model_key: amnet
    model_plain: AMNet
    value: 0.0787
    std: null
    paper_value: 0.0787
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0787
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0787
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
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.0782
    std: null
    paper_value: 0.0782
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0782
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0782
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
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.0775
    std: null
    paper_value: 0.0775
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0775
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0775
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
  - model: DCI
    model_key: dci
    model_plain: DCI
    value: 0.0774
    std: null
    paper_value: 0.0774
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0774
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0774
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
  - model: PCGNN
    model_key: pcgnn
    model_plain: PCGNN
    value: 0.0773
    std: null
    paper_value: 0.0773
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0773
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0773
    sort_std: null
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
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.0768
    std: null
    paper_value: 0.0768
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0768
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0768
    sort_std: null
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.072
    std: null
    paper_value: 0.072
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.072
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.072
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.0719
    std: null
    paper_value: 0.0719
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0719
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0719
    sort_std: null
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.0688
    std: null
    paper_value: 0.0688
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0688
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0688
    sort_std: null
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
  - model: BGNN
    model_key: bgnn
    model_plain: BGNN
    value: 0.0687
    std: null
    paper_value: 0.0687
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0687
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0687
    sort_std: null
    global_rank: 13
    paper_rank: 13
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
    value: 0.0641
    std: null
    paper_value: 0.0641
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0641
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0641
    sort_std: null
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
  - model: KNN
    model_key: knn
    model_plain: KNN
    value: 0.0612
    std: null
    paper_value: 0.0612
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0612
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0612
    sort_std: null
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.0604
    std: null
    paper_value: 0.0604
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0604
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0604
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.0591
    std: null
    paper_value: 0.0591
    paper_std: null
    metric: AUPRC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0591
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0591
    sort_std: null
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: XGBoost
    model_key: xgboost
    model_plain: XGBoost
    value: 0.0556
    std: null
    paper_value: 0.0556
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0556
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0556
    sort_std: null
    global_rank: 20
    paper_rank: 20
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
    value: 0.0556
    std: null
    paper_value: 0.0556
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0556
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0556
    sort_std: null
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: XGB-Graph
    model_key: xgb-graph
    model_plain: XGB-Graph
    value: 0.0529
    std: null
    paper_value: 0.0529
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0529
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0529
    sort_std: null
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RF-Graph
    model_key: rf-graph
    model_plain: RF-Graph
    value: 0.0513
    std: null
    paper_value: 0.0513
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0513
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0513
    sort_std: null
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
  - model: GHRN
    model_key: ghrn
    model_plain: GHRN
    value: 0.0466
    std: null
    paper_value: 0.0466
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0466
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0466
    sort_std: null
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: rf
    model_key: rf
    model_plain: rf
    value: 0.0463
    std: null
    paper_value: 0.0463
    paper_std: null
    metric: AUPRC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0463
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0463
    sort_std: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.0463
    std: null
    paper_value: 0.0463
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0463
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0463
    sort_std: null
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAS
    model_key: gas
    model_plain: GAS
    value: 0.0443
    std: null
    paper_value: 0.0443
    paper_std: null
    metric: AUPRC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Hyperparameter tuning via random search
    date: Jun 21, 2023
    date_display: Jun 2023
    date_iso: '2023-06-21'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-21'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0443
    true_std: null
    value_gap_source_arxiv: '2306.12251'
    value_gap_source_title: 'GADBench: Revisiting and Benchmarking Supervised Graph
      Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0443
    sort_std: null
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUPRC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUPRC
  metric: AUPRC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Other Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
main_figure: /figures/2306.12251/main_figure.jpegoptim.jpg
---

