---
title: Contrastive Graph Few-Shot Learning
arxiv_id: '2210.00084'
source_url: ''
authors:
- name: Chunhui Zhang
  orcid: null
  s2_author_id: '50445486'
  s2_url: null
- name: Hongfu Liu
  orcid: null
  s2_author_id: '2754632'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '2040455'
  s2_url: null
- name: Yanfang Ye
  orcid: null
  s2_author_id: '2093920413'
  s2_url: null
- name: Chuxu Zhang
  orcid: null
  s2_author_id: '2117879943'
  s2_url: null
published_date: Sep 30, 2022
published_date_iso: '2022-09-30'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Prevailing deep graph learning models often suffer from label sparsity issue.
  Although many graph few-shot learning (GFL) methods have been developed to avoid
  the performance degradation in face of limited annotated data, they excessively
  rely on labeled data, where the distribution shift in the test phase might result
  in impaired generalization ability. Additionally, they lack a general purpose as
  their designs are coupled with task or data-specific characteristics. To this end,
  we propose a general and effective Contrastive Graph Few-shot Learning framework
  (CGFL). CGFL leverages a self-distilled contrastive learning procedure to boost
  GFL. Specifically, our model firstly pre-trains a graph encoder with contrastive
  learning using unlabeled data. Later, the trained encoder is frozen as a teacher
  model to distill a student model with a contrastive loss. The distilled model is
  finally fed to GFL. CGFL learns data representation in a self-supervised manner,
  thus mitigating the distribution shift impact for better generalization and making
  model task and data-independent for a general graph mining purpose. Furthermore,
  we introduce an information-based method to quantitatively measure the capability
  of CGFL. Comprehensive experiments demonstrate that CGFL outperforms state-of-the-art
  baselines on several graph mining tasks in the few-shot scenario. We also provide
  quantitative measurement of CGFL's success.
codebase_url: https://github.com/SongW-SW/TENT
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CGFL-I
- CGFL-T
mrr: 0.0103
adjusted_mrr: 0.0034
mrr_dataset_count: 1
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
  - model: BGNN(m)-CS
    model_key: bgnn(m)-cs
    model_plain: BGNN(m)-CS
    value: 0.8068
    std: 0.0149
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8068
    sort_std: 0.0149
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BGNN
    model_key: bgnn
    model_plain: BGNN
    value: 0.7936
    std: 0.0281
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7936
    sort_std: 0.0281
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BGNN(m)-SC
    model_key: bgnn(m)-sc
    model_plain: BGNN(m)-SC
    value: 0.7889
    std: 0.0079
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7889
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.5883
    std: 0.0532
    paper_value: 0.5883
    paper_std: 0.0532
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
    table_ref: Table 1
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.622
    at_pub_std: 0.036
    at_pub_source_arxiv: '2205.15733'
    at_pub_source_title: Template based Graph Neural Network with Optimal Transport
      Distances
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.03369999999999995
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.762
    true_std: 0.028
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.17369999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.028
    global_rank: 8
    paper_rank: 128
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.5847
    std: 0.0384
    paper_value: 0.5847
    paper_std: 0.0384
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
    table_ref: Table 1
    source_ref: shervashidze2011weisfeiler
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.695
    at_pub_std: 0.032
    at_pub_source_arxiv: '2205.15733'
    at_pub_source_title: Template based Graph Neural Network with Optimal Transport
      Distances
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.11029999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.695
    true_std: 0.032
    value_gap_source_arxiv: '2205.15733'
    value_gap_source_title: Template based Graph Neural Network with Optimal Transport
      Distances
    value_gap_source_is_current_paper: false
    value_gap: 0.11029999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.695
    sort_std: 0.032
    global_rank: 30
    paper_rank: 128
    rank_delta: 98
    rank_delta_abs: 98
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Template based Graph Neural Network with Optimal Transport
      Distances
    comparison_source_arxiv: '2205.15733'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.68167
    std: 0.05449
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 38
    sort_value: 0.68167
    sort_std: 0.05449
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGFL-T
    model_key: cgfl-t
    model_plain: CGFL-T
    value: 0.6297
    std: 0.0292
    paper_value: 0.6297
    paper_std: 0.0292
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot transductive setting
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6297
    true_std: 0.0292
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6297
    sort_std: 0.0292
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.4964
    std: 0.0423
    paper_value: 0.4964
    paper_std: 0.0423
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
    table_ref: Table 1
    source_ref: lee2019self
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6253
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.12889999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6253
    true_std: null
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.12889999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6253
    sort_std: null
    global_rank: 88
    paper_rank: 182
    rank_delta: 94
    rank_delta_abs: 94
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis
      for Graph Representation and Learning'
    comparison_source_arxiv: '2007.11202'
    is_best: false
    is_std_outlier: false
  - model: Teacher-T
    model_key: teacher-t
    model_plain: Teacher-T
    value: 0.623
    std: 0.0329
    paper_value: 0.623
    paper_std: 0.0329
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot transductive setting
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.623
    true_std: 0.0329
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.623
    sort_std: 0.0329
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGFL-I
    model_key: cgfl-i
    model_plain: CGFL-I
    value: 0.6166
    std: 0.0461
    paper_value: 0.6166
    paper_std: 0.0461
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot inductive setting
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6166
    true_std: 0.0461
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6166
    sort_std: 0.0461
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Teacher-I
    model_key: teacher-i
    model_plain: Teacher-I
    value: 0.6112
    std: 0.048
    paper_value: 0.6112
    paper_std: 0.048
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot inductive setting
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6112
    true_std: 0.048
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6112
    sort_std: 0.048
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AS-MAML
    model_key: as-maml
    model_plain: AS-MAML
    value: 0.6079
    std: 0.0274
    paper_value: 0.6079
    paper_std: 0.0274
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
    table_ref: Table 1
    source_ref: ma2020adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6079
    true_std: 0.0274
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6079
    sort_std: 0.0274
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
  - model: GSM-GAT
    model_key: gsm-gat
    model_plain: GSM-GAT
    value: 0.6064
    std: 0.0384
    paper_value: 0.6064
    paper_std: 0.0384
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
    table_ref: Table 1
    source_ref: chauhan2020few
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6064
    true_std: 0.0384
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6064
    sort_std: 0.0384
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-KNN
    model_key: gin-knn
    model_plain: GIN-KNN
    value: 0.5934
    std: 0.0524
    paper_value: 0.5934
    paper_std: 0.0524
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
    table_ref: Table 1
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5934
    true_std: 0.0524
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5934
    sort_std: 0.0524
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.5822
    std: 0.043
    paper_value: 0.5822
    paper_std: 0.043
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: narayanan2017graph2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5822
    true_std: 0.043
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5822
    sort_std: 0.043
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSM-GCN
    model_key: gsm-gcn
    model_plain: GSM-GCN
    value: 0.5816
    std: 0.0439
    paper_value: 0.5816
    paper_std: 0.0439
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
    table_ref: Table 1
    source_ref: chauhan2020few
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5816
    true_std: 0.0439
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5816
    sort_std: 0.0439
    global_rank: 136
    paper_rank: 136
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
    value: 0.55833
    std: 0.03516
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 145
    sort_value: 0.55833
    sort_std: 0.03516
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CapsGNN
    model_key: capsgnn
    model_plain: CapsGNN
    value: 0.5531
    std: 0.0423
    paper_value: 0.5531
    paper_std: 0.0423
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
    table_ref: Table 1
    source_ref: xinyi2018capsule
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.547
    at_pub_std: 0.057
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5531
    true_std: 0.0423
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5531
    sort_std: 0.0423
    global_rank: 148
    paper_rank: 148
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.553
    std: 0.0378
    paper_value: 0.553
    paper_std: 0.0378
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
    table_ref: Table 1
    source_ref: shervashidze2009efficient
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.414
    at_pub_std: 0.052
    at_pub_source_arxiv: '2009.10564'
    at_pub_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    at_pub_source_date_iso: '2020-09-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.13900000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.553
    true_std: 0.0378
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.553
    sort_std: 0.0378
    global_rank: 149
    paper_rank: 149
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    comparison_source_arxiv: '2009.10564'
    is_best: false
    is_std_outlier: false
  - model: AWE
    model_key: awe
    model_plain: AWE
    value: 0.4558
    std: 0.0211
    paper_value: 0.4558
    paper_std: 0.0211
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ivanov2018anonymous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-shot few-shot graph classification
    date: Sep 30, 2022
    date_display: Sep 2022
    date_iso: '2022-09-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.358
    at_pub_std: 0.059
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0978
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4558
    true_std: 0.0211
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4558
    sort_std: 0.0211
    global_rank: 200
    paper_rank: 200
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Wasserstein Embedding for Graph Learning
    comparison_source_arxiv: '2006.09430'
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
main_figure: /figures/2210.00084/main_figure.jpegoptim.jpg
---

