---
title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised Graph-Level
  Anomaly Detection'
arxiv_id: '2407.02057'
source_url: ''
authors:
- name: Yali Fu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jindong Li
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jiahong Liu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Qianli Xing
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Qi Wang
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Irwin King
  orcid: null
  s2_author_id: null
  s2_url: null
published_date: Jul 2, 2024
published_date_iso: '2024-07-02'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Unsupervised graph-level anomaly detection (UGAD) has garnered increasing
  attention in recent years due to its significance. Most existing methods that rely
  on traditional GNNs mainly consider pairwise relationships between first-order neighbors,
  which is insufficient to capture the complex high-order dependencies often associated
  with anomalies. This limitation underscores the necessity of exploring high-order
  node interactions in UGAD. In addition, most previous works ignore the underlying
  properties (e.g., hierarchy and power-law structure) which are common in real-world
  graph datasets and therefore are indispensable factors in the UGAD task. In this
  paper, we propose a novel Dual Hyperbolic Contrastive Learning for Unsupervised
  Graph-Level Anomaly Detection (HC-GLAD in short). To exploit high-order node group
  information, we construct hypergraphs based on pre-designed gold motifs and subsequently
  perform hypergraph convolution. Furthermore, to preserve the hierarchy of real-world
  graphs, we introduce hyperbolic geometry into this field and conduct both graph
  and hypergraph embedding learning in hyperbolic space with the hyperboloid model.
  To the best of our knowledge, this is the first work to simultaneously apply hypergraph
  with node group information and hyperbolic geometry in this field. Extensive experiments
  on 13 real-world datasets of different fields demonstrate the superiority of HC-GLAD
  on the UGAD task. The code is available at.
codebase_url: https://github.com/Yali-Fu/HC-GLAD
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HC-GLAD
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ENZYMES
  rows:
  - model: HC-GLAD
    model_key: hc-glad
    model_plain: HC-GLAD
    value: 0.6539
    std: 0.0623
    paper_value: 0.6539
    paper_std: 0.0623
    metric: AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6539
    true_std: 0.0623
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6539
    sort_std: 0.0623
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
  - model: GOOD-D
    model_key: good-d
    model_plain: GOOD-D
    value: 0.639
    std: 0.0369
    paper_value: 0.639
    paper_std: 0.0369
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.639
    true_std: 0.0369
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.639
    sort_std: 0.0369
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
  - model: GlocalKD
    model_key: glocalkd
    model_plain: GlocalKD
    value: 0.6139
    std: 0.0881
    paper_value: 0.6139
    paper_std: 0.0881
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6139
    true_std: 0.0881
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6139
    sort_std: 0.0881
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: OCGIN
    model_key: ocgin
    model_plain: OCGIN
    value: 0.5875
    std: 0.0598
    paper_value: 0.5875
    paper_std: 0.0598
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5875
    true_std: 0.0598
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5875
    sort_std: 0.0598
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL-OCSVM
    model_key: wl-ocsvm
    model_plain: WL-OCSVM
    value: 0.5524
    std: 0.0266
    paper_value: 0.5524
    paper_std: 0.0266
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5524
    true_std: 0.0266
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5524
    sort_std: 0.0266
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
  - model: InfoGraph-iF
    model_key: infograph-if
    model_plain: InfoGraph-iF
    value: 0.538
    std: 0.045
    paper_value: 0.538
    paper_std: 0.045
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.538
    true_std: 0.045
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.538
    sort_std: 0.045
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
  - model: PK-OCSVM
    model_key: pk-ocsvm
    model_plain: PK-OCSVM
    value: 0.5367
    std: 0.0266
    paper_value: 0.5367
    paper_std: 0.0266
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5367
    true_std: 0.0266
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5367
    sort_std: 0.0266
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
  - model: GraphCL-iF
    model_key: graphcl-if
    model_plain: GraphCL-iF
    value: 0.536
    std: 0.0488
    paper_value: 0.536
    paper_std: 0.0488
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.536
    true_std: 0.0488
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.536
    sort_std: 0.0488
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
  - model: WL-iF
    model_key: wl-if
    model_plain: WL-iF
    value: 0.516
    std: 0.0381
    paper_value: 0.516
    paper_std: 0.0381
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.516
    true_std: 0.0381
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.516
    sort_std: 0.0381
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
  - model: PK-iF
    model_key: pk-if
    model_plain: PK-iF
    value: 0.513
    std: 0.0201
    paper_value: 0.513
    paper_std: 0.0201
    metric: AUC
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
    source_ref: 2023_WSDM_GOOD-D
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUC reported in percent in table, converted to [0,1]. Task is graph-level
      anomaly detection.
    date: Jul 2, 2024
    date_display: Jul 2024
    date_iso: '2024-07-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.513
    true_std: 0.0201
    value_gap_source_arxiv: '2407.02057'
    value_gap_source_title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised
      Graph-Level Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.513
    sort_std: 0.0201
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: HC-GLAD
main_figure: /figures/2407.02057/main_figure.jpegoptim.jpg
---

