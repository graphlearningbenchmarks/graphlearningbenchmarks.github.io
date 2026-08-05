---
title: Rethinking Graph Neural Networks for Anomaly Detection
arxiv_id: '2205.15508'
source_url: ''
authors:
- name: Jianheng Tang
  orcid: null
  s2_author_id: '66239746'
  s2_url: null
- name: Jiajin Li
  orcid: null
  s2_author_id: '1932149570'
  s2_url: null
- name: Zi-Chao Gao
  orcid: null
  s2_author_id: '120267993'
  s2_url: null
- name: Jia Li
  orcid: null
  s2_author_id: '2118372080'
  s2_url: null
published_date: May 31, 2022
published_date_iso: '2022-05-31'
published_venue: ICML 2022
published_conference: ICML 2022
published_conference_short: ICML
published_conference_slug: icml
abstract: Graph Neural Networks (GNNs) are widely applied for graph anomaly detection.
  As one of the key components for GNN design is to select a tailored spectral filter,
  we take the first step towards analyzing anomalies via the lens of the graph spectrum.
  Our crucial observation is the existence of anomalies will lead to the `right-shift'
  phenomenon, that is, the spectral energy distribution concentrates less on low frequencies
  and more on high frequencies. This fact motivates us to propose the Beta Wavelet
  Graph Neural Network (BWGNN). Indeed, BWGNN has spectral and spatial localized band-pass
  filters to better handle the `right-shift' phenomenon in anomalies. We demonstrate
  the effectiveness of BWGNN on four large-scale anomaly detection datasets. Our code
  and data are released at https://github.com/squareRoot3/Rethinking-Anomaly-Detection
codebase_url: https://github.com/squareRoot3/Rethinking-Anomaly-Detection
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BWGNN (Homo)
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon2M
  rows:
  - model: BWGNN (Homo)
    model_key: bwgnn (homo)
    model_plain: BWGNN (Homo)
    value: 0.9229
    std: 0.0044
    paper_value: 0.9229
    paper_std: 0.0044
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9229
    true_std: 0.0044
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0044
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
  - model: ChebyNet
    model_key: chebynet
    model_plain: ChebyNet
    value: 0.9194
    std: 0.0029
    paper_value: 0.9194
    paper_std: 0.0029
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9194
    true_std: 0.0029
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9194
    sort_std: 0.0029
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
  - model: GWNN
    model_key: gwnn
    model_plain: GWNN
    value: 0.91
    std: 0.0027
    paper_value: 0.91
    paper_std: 0.0027
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.91
    true_std: 0.0027
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.91
    sort_std: 0.0027
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
  - model: SVM
    model_key: svm
    model_plain: SVM
    value: 0.9071
    std: 0.0004
    paper_value: 0.9071
    paper_std: 0.0004
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9071
    true_std: 0.0004
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9071
    sort_std: 0.0004
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
  - model: PC-GNN
    model_key: pc-gnn
    model_plain: PC-GNN
    value: 0.8956
    std: 0.0077
    paper_value: 0.8956
    paper_std: 0.0077
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8956
    true_std: 0.0077
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8956
    sort_std: 0.0077
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
  - model: CAREGNN
    model_key: caregnn
    model_plain: CAREGNN
    value: 0.8639
    std: 0.0173
    paper_value: 0.8639
    paper_std: 0.0173
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8639
    true_std: 0.0173
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8639
    sort_std: 0.0173
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8318
    std: 0.0291
    paper_value: 0.8318
    paper_std: 0.0291
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8318
    true_std: 0.0291
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8318
    sort_std: 0.0291
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7917
    std: 0.0126
    paper_value: 0.7917
    paper_std: 0.0126
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7917
    true_std: 0.0126
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7917
    sort_std: 0.0126
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
  - model: GraphConsis
    model_key: graphconsis
    model_plain: GraphConsis
    value: 0.7512
    std: 0.0325
    paper_value: 0.7512
    paper_std: 0.0325
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7512
    true_std: 0.0325
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7512
    sort_std: 0.0325
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7417
    std: 0.0137
    paper_value: 0.7417
    paper_std: 0.0137
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7417
    true_std: 0.0137
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7417
    sort_std: 0.0137
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.6926
    std: 0.0245
    paper_value: 0.6926
    paper_std: 0.0245
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6926
    true_std: 0.0245
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6926
    sort_std: 0.0245
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6793
    std: 0.0142
    paper_value: 0.6793
    paper_std: 0.0142
    metric: F1-macro
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1% training ratio split
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6793
    true_std: 0.0142
    value_gap_source_arxiv: '2205.15508'
    value_gap_source_title: Rethinking Graph Neural Networks for Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6793
    sort_std: 0.0142
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
  rank_metric: F1-macro
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1-macro
  metric: F1-macro
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
single_proposed_model: BWGNN (Homo)
main_figure: /figures/2205.15508/main_figure.jpegoptim.jpg
---

