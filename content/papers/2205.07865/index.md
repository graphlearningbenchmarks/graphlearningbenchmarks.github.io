---
title: Simple Contrastive Graph Clustering
arxiv_id: '2205.07865'
source_url: ''
authors:
- name: Yue Liu
  orcid: null
  s2_author_id: '2119033665'
  s2_url: null
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
- name: Siwei Wang
  orcid: null
  s2_author_id: '103307910'
  s2_url: null
- name: K. Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Wenxuan Tu
  orcid: null
  s2_author_id: '1381761887'
  s2_url: null
- name: Liangjun Li
  orcid: null
  s2_author_id: '2145729091'
  s2_url: null
published_date: May 11, 2022
published_date_iso: '2022-05-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Contrastive learning has recently attracted plenty of attention in deep
  graph clustering for its promising performance. However, complicated data augmentations
  and time-consuming graph convolutional operation undermine the efficiency of these
  methods. To solve this problem, we propose a Simple Contrastive Graph Clustering
  (SCGC) algorithm to improve the existing methods from the perspectives of network
  architecture, data augmentation, and objective function. As to the architecture,
  our network includes two main parts, i.e., pre-processing and network backbone.
  A simple low-pass denoising operation conducts neighbor information aggregation
  as an independent pre-processing, and only two multilayer perceptrons (MLPs) are
  included as the backbone. For data augmentation, instead of introducing complex
  operations over graphs, we construct two augmented views of the same vertex by designing
  parameter un-shared siamese encoders and perturbing the node embeddings directly.
  Finally, as to the objective function, to further improve the clustering performance,
  a novel cross-view structural consistency objective function is designed to enhance
  the discriminative capability of the learned network. Extensive experimental results
  on seven benchmark datasets validate our proposed algorithm's effectiveness and
  superiority. Significantly, our algorithm outperforms the recent contrastive deep
  clustering competitors with at least seven times speedup on average.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SCGC
mrr: 0.248
adjusted_mrr: 0.248
mrr_dataset_count: 4
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 4
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: AMAP
  rows:
  - model: GANN
    model_key: gann
    model_plain: GANN
    value: 0.9405
    std: 0.0037
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9405
    sort_std: 0.0037
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.9308
    std: 0.0026
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9308
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9238
    std: 0.0014
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9238
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8115
    std: 0.0105
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 14
    sort_value: 0.8115
    sort_std: 0.0105
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.7125
    std: 0.0031
    paper_value: 0.7125
    paper_std: 0.0031
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76
    at_pub_std: 0.008
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04749999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.008
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04749999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.008
    global_rank: 16
    paper_rank: 22
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: SCAGC
    model_key: scagc
    model_plain: SCAGC
    value: 0.7277
    std: 0.0016
    paper_value: 0.7277
    paper_std: 0.0016
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7277
    true_std: 0.0016
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7277
    sort_std: 0.0016
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
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    value: 0.7222
    std: 0.0097
    paper_value: 0.7222
    paper_std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7222
    true_std: 0.0097
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7222
    sort_std: 0.0097
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
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7174
    std: 0.0093
    paper_value: 0.7174
    paper_std: 0.0093
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
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
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6987
    std: 0.0054
    paper_value: 0.6987
    paper_std: 0.0054
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6205
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07819999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6808
    std: 0.0176
    paper_value: 0.6808
    paper_std: 0.0176
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6121
    at_pub_std: 0.0122
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06869999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.5066
    std: 0.0149
    paper_value: 0.5066
    paper_std: 0.0149
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6805
    at_pub_std: 0.0181
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.17389999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6805
    true_std: 0.0181
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17389999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6805
    sort_std: 0.0181
    global_rank: 31
    paper_rank: 49
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.643
    std: 0.0195
    paper_value: 0.643
    paper_std: 0.0195
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6483
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.005299999999999971
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6483
    true_std: 0.0059
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.005299999999999971
    has_value_note: false
    value_note: ''
    sort_value: 0.6483
    sort_std: 0.0059
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3288
    std: 0.055
    paper_value: 0.3288
    paper_std: 0.055
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4273
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.09850000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6283
    true_std: 0.0159
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.2995
    has_value_note: false
    value_note: ''
    sort_value: 0.6283
    sort_std: 0.0159
    global_rank: 40
    paper_rank: 53
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: DEC
    model_key: dec
    model_plain: DEC
    value: 0.4671
    std: 0.0012
    paper_value: 0.4671
    paper_std: 0.0012
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5816
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.11449999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5816
    true_std: 0.0056
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.11449999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.5816
    sort_std: 0.0056
    global_rank: 44
    paper_rank: 52
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: SSGC
    model_key: ssgc
    model_plain: SSGC
    value: 0.5279
    std: 0.0001
    paper_value: 0.5279
    paper_std: 0.0001
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5279
    true_std: 0.0001
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5279
    sort_std: 0.0001
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AE
    model_key: ae
    model_plain: AE
    value: 0.4787
    std: 0.002
    paper_value: 0.4787
    paper_std: 0.002
    metric: F1
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5143
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.035599999999999965
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5143
    true_std: 0.0035
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.035599999999999965
    has_value_note: false
    value_note: ''
    sort_value: 0.5143
    sort_std: 0.0035
    global_rank: 48
    paper_rank: 51
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: K-means
    model_key: k-means
    model_plain: K-means
    value: 0.2396
    std: 0.0051
    paper_value: 0.2396
    paper_std: 0.0051
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3192
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2202.12533'
    at_pub_source_title: Improved Dual Correlation Reduction Network
    at_pub_source_date_iso: '2022-02-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07959999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3192
    true_std: 0.0027
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.07959999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3192
    sort_std: 0.0027
    global_rank: 54
    paper_rank: 55
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: BAT
  rows:
  - model: GraphLearner
    model_key: graphlearner
    model_plain: GraphLearner
    value: 0.754
    std: 0.0088
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    venue: ACM Multimedia
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.754
    sort_std: 0.0088
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SCGDN
    model_key: scgdn
    model_plain: SCGDN
    value: 0.7449
    std: 0.0026
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    venue: ACM Multimedia
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7449
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    value: 0.7222
    std: 0.0097
    paper_value: 0.7222
    paper_std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7222
    true_std: 0.0097
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7222
    sort_std: 0.0097
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.7174
    std: 0.0093
    paper_value: 0.7174
    paper_std: 0.0093
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
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
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7125
    std: 0.0031
    paper_value: 0.7125
    paper_std: 0.0031
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7125
    true_std: 0.0031
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7125
    sort_std: 0.0031
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.7125
    std: 0.0031
    paper_value: 0.7125
    paper_std: 0.0031
    metric: F1
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
    protocol_note: 'Note: The table row for SDCN in BAT F1 seems to match AGE''s value
      in the provided text snippet, but I am extracting the value from the table cell
      provided.'
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7125
    true_std: 0.0031
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7125
    sort_std: 0.0031
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7047
    std: 0.037
    paper_value: 0.7047
    paper_std: 0.037
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7047
    true_std: 0.037
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7047
    sort_std: 0.037
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
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6987
    std: 0.0054
    paper_value: 0.6987
    paper_std: 0.0054
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6808
    std: 0.0176
    paper_value: 0.6808
    paper_std: 0.0176
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
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
  - model: AE
    model_key: ae
    model_plain: AE
    value: 0.4787
    std: 0.002
    paper_value: 0.4787
    paper_std: 0.002
    metric: F1
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4787
    true_std: 0.002
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4787
    sort_std: 0.002
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
  - model: DEC
    model_key: dec
    model_plain: DEC
    value: 0.4671
    std: 0.0012
    paper_value: 0.4671
    paper_std: 0.0012
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4671
    true_std: 0.0012
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4671
    sort_std: 0.0012
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
  - model: K-means
    model_key: k-means
    model_plain: K-means
    value: 0.2396
    std: 0.0051
    paper_value: 0.2396
    paper_std: 0.0051
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2396
    true_std: 0.0051
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2396
    sort_std: 0.0051
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: EAT
  rows:
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.7702
    std: 0.0033
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/yueliu1999/HSAN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7702
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HSAN
    model_key: hsan
    model_plain: HSAN
    value: 0.7702
    std: 0.0033
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/yueliu1999/HSAN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7702
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.7125
    std: 0.0031
    paper_value: 0.7125
    paper_std: 0.0031
    metric: F1
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
    source_ref: DFCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7682
    true_std: 0.0023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.05569999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7682
    sort_std: 0.0023
    global_rank: 3
    paper_rank: 10
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7174
    std: 0.0093
    paper_value: 0.7174
    paper_std: 0.0093
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7598
    true_std: 0.0068
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.04239999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7598
    sort_std: 0.0068
    global_rank: 5
    paper_rank: 9
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6987
    std: 0.0054
    paper_value: 0.6987
    paper_std: 0.0054
    metric: F1
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
    source_ref: DAEGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7596
    true_std: 0.0023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.060900000000000065
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.0023
    global_rank: 6
    paper_rank: 10
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCAGC
    model_key: scagc
    model_plain: SCAGC
    value: 0.7277
    std: 0.0016
    paper_value: 0.7277
    paper_std: 0.0016
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7277
    true_std: 0.0016
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7277
    sort_std: 0.0016
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
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    value: 0.7222
    std: 0.0097
    paper_value: 0.7222
    paper_std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7222
    true_std: 0.0097
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7222
    sort_std: 0.0097
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.643
    std: 0.0195
    paper_value: 0.643
    paper_std: 0.0195
    metric: F1
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
    source_ref: ARGA_conf
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6928
    true_std: 0.023
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.049799999999999955
    has_value_note: false
    value_note: ''
    sort_value: 0.6928
    sort_std: 0.023
    global_rank: 11
    paper_rank: 12
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6808
    std: 0.0176
    paper_value: 0.6808
    paper_std: 0.0176
    metric: F1
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
    source_ref: GAE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.5066
    std: 0.0149
    paper_value: 0.5066
    paper_std: 0.0149
    metric: F1
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
    source_ref: SDCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5344
    true_std: 0.0081
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_gap_source_is_current_paper: false
    value_gap: 0.027799999999999936
    has_value_note: false
    value_note: ''
    sort_value: 0.5344
    sort_std: 0.0081
    global_rank: 16
    paper_rank: 18
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SSGC
    model_key: ssgc
    model_plain: SSGC
    value: 0.5279
    std: 0.0001
    paper_value: 0.5279
    paper_std: 0.0001
    metric: F1
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
    source_ref: SSGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5279
    true_std: 0.0001
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5279
    sort_std: 0.0001
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
  - model: AE
    model_key: ae
    model_plain: AE
    value: 0.4787
    std: 0.002
    paper_value: 0.4787
    paper_std: 0.002
    metric: F1
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
    source_ref: AE_K_MEANS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4787
    true_std: 0.002
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4787
    sort_std: 0.002
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3288
    std: 0.055
    paper_value: 0.3288
    paper_std: 0.055
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.47
    true_std: 0.06
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.1412
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.06
    global_rank: 22
    paper_rank: 30
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: DEC
    model_key: dec
    model_plain: DEC
    value: 0.4671
    std: 0.0012
    paper_value: 0.4671
    paper_std: 0.0012
    metric: F1
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
    source_ref: DEC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4671
    true_std: 0.0012
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4671
    sort_std: 0.0012
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
  - model: K-means
    model_key: k-means
    model_plain: K-means
    value: 0.2396
    std: 0.0051
    paper_value: 0.2396
    paper_std: 0.0051
    metric: F1
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
    source_ref: K-means
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2396
    true_std: 0.0051
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2396
    sort_std: 0.0051
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: UAT
  rows:
  - model: SCAGC
    model_key: scagc
    model_plain: SCAGC
    value: 0.7277
    std: 0.0016
    paper_value: 0.7277
    paper_std: 0.0016
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7277
    true_std: 0.0016
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7277
    sort_std: 0.0016
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
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    value: 0.7222
    std: 0.0097
    paper_value: 0.7222
    paper_std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7222
    true_std: 0.0097
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7222
    sort_std: 0.0097
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
  - model: AGE
    model_key: age
    model_plain: AGE
    value: 0.7174
    std: 0.0093
    paper_value: 0.7174
    paper_std: 0.0093
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7174
    true_std: 0.0093
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0093
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
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.6987
    std: 0.0054
    paper_value: 0.6987
    paper_std: 0.0054
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6808
    std: 0.0176
    paper_value: 0.6808
    paper_std: 0.0176
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
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
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.6718
    std: 0.0013
    paper_value: 0.6718
    paper_std: 0.0013
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6718
    true_std: 0.0013
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6718
    sort_std: 0.0013
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.643
    std: 0.0195
    paper_value: 0.643
    paper_std: 0.0195
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: 0.0195
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.0195
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
  - model: SSGC
    model_key: ssgc
    model_plain: SSGC
    value: 0.5279
    std: 0.0001
    paper_value: 0.5279
    paper_std: 0.0001
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5279
    true_std: 0.0001
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5279
    sort_std: 0.0001
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.5066
    std: 0.0149
    paper_value: 0.5066
    paper_std: 0.0149
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5066
    true_std: 0.0149
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5066
    sort_std: 0.0149
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3288
    std: 0.055
    paper_value: 0.3288
    paper_std: 0.055
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.49
    true_std: 0.04
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.1612
    has_value_note: false
    value_note: ''
    sort_value: 0.49
    sort_std: 0.04
    global_rank: 24
    paper_rank: 34
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AE
    model_key: ae
    model_plain: AE
    value: 0.4787
    std: 0.002
    paper_value: 0.4787
    paper_std: 0.002
    metric: F1
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4787
    true_std: 0.002
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4787
    sort_std: 0.002
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DEC
    model_key: dec
    model_plain: DEC
    value: 0.4671
    std: 0.0012
    paper_value: 0.4671
    paper_std: 0.0012
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4671
    true_std: 0.0012
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4671
    sort_std: 0.0012
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
  - model: K-means
    model_key: k-means
    model_plain: K-means
    value: 0.2396
    std: 0.0051
    paper_value: 0.2396
    paper_std: 0.0051
    metric: F1
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
    protocol_note: Clustering performance reported as mean±std under ten runs.
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2396
    true_std: 0.0051
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2396
    sort_std: 0.0051
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: UAT
      dataset_slug: uat
    - dataset: BAT
      dataset_slug: bat
    - dataset: EAT
      dataset_slug: eat
single_proposed_model: SCGC
main_figure: /figures/2205.07865/main_figure.jpegoptim.jpg
---

