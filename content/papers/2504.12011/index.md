---
title: Balancing Graph Embedding Smoothness in Self-Supervised Learning via Information-Theoretic
  Decomposition
arxiv_id: '2504.12011'
source_url: ''
authors:
- name: Heesoo Jung
  orcid: null
  s2_author_id: '123133026'
  s2_url: null
- name: Hogun Park
  orcid: null
  s2_author_id: '2256110317'
  s2_url: null
published_date: Apr 16, 2025
published_date_iso: '2025-04-16'
published_venue: WWW 2025
published_conference: WWW 2025
published_conference_short: WWW
published_conference_slug: www
abstract: 'Self-supervised learning (SSL) in graphs has garnered significant attention,
  particularly in employing Graph Neural Networks (GNNs) with pretext tasks initially
  designed for other domains, such as contrastive learning and feature reconstruction.
  However, it remains uncertain whether these methods effectively reflect essential
  graph properties, precisely representation similarity with its neighbors. We observe
  that existing methods position opposite ends of a spectrum driven by the graph embedding
  smoothness, with each end corresponding to outperformance on specific downstream
  tasks. Decomposing the SSL objective into three terms via an information-theoretic
  framework with a neighbor representation variable reveals that this polarization
  stems from an imbalance among the terms, which existing methods may not effectively
  maintain. Further insights suggest that balancing between the extremes can lead
  to improved performance across a wider range of downstream tasks. A framework, BSG
  (Balancing Smoothness in Graph SSL), introduces novel loss functions designed to
  supplement the representation quality in graph-based SSL by balancing the derived
  three terms: neighbor loss, minimal loss, and divergence loss. We present a theoretical
  analysis of the effects of these loss functions, highlighting their significance
  from both the SSL and graph smoothness perspectives. Extensive experiments on multiple
  real-world datasets across node classification and link prediction consistently
  demonstrate that BSG achieves state-of-the-art performance, outperforming existing
  methods. Our implementation code is available at.'
codebase_url: https://github.com/steve30572/BSG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BSG
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- TU Dortmund
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id003
  dataset: Amazon-Computers
  rows:
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8651
    std: 0.0054
    paper_value: 0.8651
    paper_std: 0.0054
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.916
    at_pub_std: 0.016
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.050900000000000056
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07610000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 317
    rank_delta: 315
    rank_delta_abs: 315
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8693
    std: 0.0029
    paper_value: 0.8693
    paper_std: 0.0029
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.924
    at_pub_std: 0.013
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05470000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07050000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 304
    rank_delta: 301
    rank_delta_abs: 301
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GiGaMAE
    model_key: gigamae
    model_plain: GiGaMAE
    value: 0.902
    std: 0.0045
    paper_value: 0.902
    paper_std: 0.0045
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.897
    at_pub_std: 0.007
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.902
    true_std: 0.0045
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.902
    sort_std: 0.0045
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BSG
    model_key: bsg
    model_plain: BSG
    value: 0.8999
    std: 0.0008
    paper_value: 0.8999
    paper_std: 0.0008
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8999
    true_std: 0.0008
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8999
    sort_std: 0.0008
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE2
    model_key: graphmae2
    model_plain: GraphMAE2
    value: 0.8742
    std: 0.0052
    paper_value: 0.8742
    paper_std: 0.0052
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.896
    at_pub_std: 0.004
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-12-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02180000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.899
    true_std: 0.003
    value_gap_source_arxiv: '2512.13235'
    value_gap_source_title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.024800000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.899
    sort_std: 0.003
    global_rank: 139
    paper_rank: 291
    rank_delta: 152
    rank_delta_abs: 152
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    comparison_source_arxiv: '2410.10241'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.8625
    std: 0.0025
    paper_value: 0.8625
    paper_std: 0.0025
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8953
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-06-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.03279999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8953
    true_std: 0.0035
    value_gap_source_arxiv: '2506.20362'
    value_gap_source_title: Self-Supervised Graph Learning via Spectral Bootstrapping
      and Laplacian-Based Augmentations
    value_gap_source_is_current_paper: false
    value_gap: 0.03279999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8953
    sort_std: 0.0035
    global_rank: 171
    paper_rank: 327
    rank_delta: 156
    rank_delta_abs: 156
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.8936
    std: 0.0018
    paper_value: 0.8936
    paper_std: 0.0018
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.895
    at_pub_std: 0.001
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0014000000000000679
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8936
    true_std: 0.0018
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8936
    sort_std: 0.0018
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Bandana
    model_key: bandana
    model_plain: Bandana
    value: 0.8928
    std: 0.0014
    paper_value: 0.8928
    paper_std: 0.0014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8928
    true_std: 0.0014
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8928
    sort_std: 0.0014
    global_rank: 182
    paper_rank: 182
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.8876
    std: 0.0036
    paper_value: 0.8876
    paper_std: 0.0036
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8874
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2209.13964'
    at_pub_source_title: Graph Soft-Contrastive Learning via Neighborhood Ranking
    at_pub_source_date_iso: '2022-09-28'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8896
    true_std: 0.0013
    value_gap_source_arxiv: '2507.07141'
    value_gap_source_title: 'Str-GCL: Structural Commonsense Driven Graph Contrastive
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.8896
    sort_std: 0.0013
    global_rank: 198
    paper_rank: 213
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.8861
    std: 0.0064
    paper_value: 0.8861
    paper_std: 0.0064
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.879
    at_pub_std: 0.003
    at_pub_source_arxiv: '2412.03864'
    at_pub_source_title: Training MLPs on Graphs without Supervision
    at_pub_source_date_iso: '2024-02-14'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.007099999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8861
    true_std: 0.0064
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8861
    sort_std: 0.0064
    global_rank: 222
    paper_rank: 222
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.8852
    std: 0.0017
    paper_value: 0.8852
    paper_std: 0.0017
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.896
    at_pub_std: 0.005
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.010800000000000032
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8852
    true_std: 0.0017
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8852
    sort_std: 0.0017
    global_rank: 229
    paper_rank: 229
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    comparison_source_arxiv: '2410.10241'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.8745
    std: 0.0047
    paper_value: 0.8745
    paper_std: 0.0047
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8798
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.005299999999999971
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8798
    true_std: 0.0081
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.005299999999999971
    has_value_note: false
    value_note: ''
    sort_value: 0.8798
    sort_std: 0.0081
    global_rank: 256
    paper_rank: 291
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.867
    std: 0.003
    paper_value: 0.867
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8721
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2405.14742'
    at_pub_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    at_pub_source_date_iso: '2024-05-23'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.005099999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8721
    true_std: 0.0026
    value_gap_source_arxiv: '2405.14742'
    value_gap_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.005099999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8721
    sort_std: 0.0026
    global_rank: 297
    paper_rank: 311
    rank_delta: 14
    rank_delta_abs: 14
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
    value: 0.8633
    std: 0.0044
    paper_value: 0.8633
    paper_std: 0.0044
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8666
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0033000000000000806
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8666
    true_std: 0.0007
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0033000000000000806
    has_value_note: false
    value_note: ''
    sort_value: 0.8666
    sort_std: 0.0007
    global_rank: 313
    paper_rank: 321
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.8602
    std: 0.0011
    paper_value: 0.8602
    paper_std: 0.0011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8466
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.013599999999999945
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8602
    true_std: 0.0011
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8602
    sort_std: 0.0011
    global_rank: 332
    paper_rank: 332
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.8586
    std: 0.0011
    paper_value: 0.8586
    paper_std: 0.0011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8439
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.014700000000000046
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8586
    true_std: 0.0011
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8586
    sort_std: 0.0011
    global_rank: 336
    paper_rank: 336
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7758
    std: 0.0082
    paper_value: 0.7758
    paper_std: 0.0082
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Computers dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8463
    at_pub_std: null
    at_pub_source_arxiv: '2407.11907'
    at_pub_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.07050000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8463
    true_std: null
    value_gap_source_arxiv: '2407.11907'
    value_gap_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    value_gap_source_is_current_paper: false
    value_gap: 0.07050000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8463
    sort_std: null
    global_rank: 359
    paper_rank: 477
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphFM: A generalist graph transformer that learns
      transferable representations across diverse domains'
    comparison_source_arxiv: '2407.11907'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Amazon-Photo
  rows:
  - model: C (orthogonal)
    model_key: msh-gnn
    model_plain: C (orthogonal)
    value: 0.9766
    std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: geomancer
    model_plain: C (orthogonal)
    value: 0.9705
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9256
    std: 0.0035
    paper_value: 0.9256
    paper_std: 0.0035
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9498
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0242
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0413
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 5
    paper_rank: 273
    rank_delta: 268
    rank_delta_abs: 268
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9242
    std: 0.0022
    paper_value: 0.9242
    paper_std: 0.0022
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9476
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.023399999999999976
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.038999999999999924
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 16
    paper_rank: 288
    rank_delta: 272
    rank_delta_abs: 272
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: BSG
    model_key: bsg
    model_plain: BSG
    value: 0.9348
    std: 0.0016
    paper_value: 0.9348
    paper_std: 0.0016
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9348
    true_std: 0.0016
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9348
    sort_std: 0.0016
    global_rank: 170
    paper_rank: 170
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.9279
    std: 0.0018
    paper_value: 0.9279
    paper_std: 0.0018
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9342
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.006300000000000083
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9342
    true_std: 0.0026
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.006300000000000083
    has_value_note: false
    value_note: ''
    sort_value: 0.9342
    sort_std: 0.0026
    global_rank: 173
    paper_rank: 244
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: Bandana
    model_key: bandana
    model_plain: Bandana
    value: 0.934
    std: 0.001
    paper_value: 0.934
    paper_std: 0.001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.934
    true_std: 0.001
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.934
    sort_std: 0.001
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.9289
    std: 0.0028
    paper_value: 0.9289
    paper_std: 0.0028
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9325
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2206.12933'
    at_pub_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0036000000000000476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9325
    true_std: 0.0021
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0036000000000000476
    has_value_note: false
    value_note: ''
    sort_value: 0.9325
    sort_std: 0.0021
    global_rank: 192
    paper_rank: 230
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE2
    model_key: graphmae2
    model_plain: GraphMAE2
    value: 0.926
    std: 0.0011
    paper_value: 0.926
    paper_std: 0.0011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.932
    at_pub_std: 0.005
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-12-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.932
    true_std: 0.003
    value_gap_source_arxiv: '2512.13235'
    value_gap_source_title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.003
    global_rank: 197
    paper_rank: 269
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.9264
    std: 0.0024
    paper_value: 0.9264
    paper_std: 0.0024
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.931
    at_pub_std: 0.004
    at_pub_source_arxiv: '2403.01400'
    at_pub_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    at_pub_source_date_iso: '2024-03-03'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0046000000000000485
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.931
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.0046000000000000485
    has_value_note: false
    value_note: ''
    sort_value: 0.931
    sort_std: 0.004
    global_rank: 207
    paper_rank: 265
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9165
    std: 0.0046
    paper_value: 0.9165
    paper_std: 0.0046
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9309
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.014399999999999968
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9309
    true_std: 0.0008
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.014399999999999968
    has_value_note: false
    value_note: ''
    sort_value: 0.9309
    sort_std: 0.0008
    global_rank: 211
    paper_rank: 352
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: GiGaMAE
    model_key: gigamae
    model_plain: GiGaMAE
    value: 0.9301
    std: 0.0046
    paper_value: 0.9301
    paper_std: 0.0046
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.935
    at_pub_std: 0.005
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0049000000000000155
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9301
    true_std: 0.0046
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9301
    sort_std: 0.0046
    global_rank: 217
    paper_rank: 217
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.9282
    std: 0.0017
    paper_value: 0.9282
    paper_std: 0.0017
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.934
    at_pub_std: 0.008
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.005800000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9282
    true_std: 0.0017
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9282
    sort_std: 0.0017
    global_rank: 236
    paper_rank: 236
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.9215
    std: 0.0024
    paper_value: 0.9215
    paper_std: 0.0024
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.928
    at_pub_std: 0.005
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.006500000000000061
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.928
    true_std: 0.005
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.006500000000000061
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.005
    global_rank: 238
    paper_rank: 319
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.9187
    std: 0.0004
    paper_value: 0.9187
    paper_std: 0.0004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9224
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-06-16'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0037000000000000366
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.0011
    value_gap_source_arxiv: '2306.09614'
    value_gap_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0033000000000000806
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.0011
    global_rank: 319
    paper_rank: 338
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9171
    std: 0.0008
    paper_value: 0.9171
    paper_std: 0.0008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9185
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9185
    true_std: 0.0006
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0013999999999999568
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: 0.0006
    global_rank: 339
    paper_rank: 350
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.9182
    std: 0.0008
    paper_value: 0.9182
    paper_std: 0.0008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9268
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.008599999999999941
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9182
    true_std: 0.0008
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9182
    sort_std: 0.0008
    global_rank: 340
    paper_rank: 340
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.9151
    std: 0.0009
    paper_value: 0.9151
    paper_std: 0.0009
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9249
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.009800000000000031
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9151
    true_std: 0.0009
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9151
    sort_std: 0.0009
    global_rank: 358
    paper_rank: 358
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8584
    std: 0.0127
    paper_value: 0.8584
    paper_std: 0.0127
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Photo dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9128
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.05439999999999989
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.05439999999999989
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0063
    global_rank: 378
    paper_rank: 481
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: Coauthor-Physics
  rows:
  - model: SelfGNN LDP
    model_key: geomancer
    model_plain: SelfGNN LDP
    value: 0.9878
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9878
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: lgd
    model_plain: SelfGNN LDP
    value: 0.9855
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9855
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: msh-gnn
    model_plain: SelfGNN LDP
    value: 0.9837
    std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9837
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9538
    std: 0.0002
    paper_value: 0.9538
    paper_std: 0.0002
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9774
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.023600000000000065
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9744
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.020600000000000063
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0014
    global_rank: 9
    paper_rank: 129
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9419
    std: 0.0028
    paper_value: 0.9419
    paper_std: 0.0028
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9782
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0363
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9732
    true_std: 0.0006
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9732
    sort_std: 0.0006
    global_rank: 19
    paper_rank: 166
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9445
    std: 0.0003
    paper_value: 0.9445
    paper_std: 0.0003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9563
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.011800000000000033
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9597
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.015199999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9597
    sort_std: 0.0007
    global_rank: 80
    paper_rank: 159
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: BSG
    model_key: bsg
    model_plain: BSG
    value: 0.9565
    std: 0.0003
    paper_value: 0.9565
    paper_std: 0.0003
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9565
    true_std: 0.0003
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9565
    sort_std: 0.0003
    global_rank: 103
    paper_rank: 103
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.9498
    std: 0.0005
    paper_value: 0.9498
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9563
    at_pub_std: 0.001
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006500000000000061
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9563
    true_std: 0.001
    value_gap_source_arxiv: '2302.08727'
    value_gap_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.006500000000000061
    has_value_note: false
    value_note: ''
    sort_value: 0.9563
    sort_std: 0.001
    global_rank: 104
    paper_rank: 146
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    comparison_source_arxiv: '2302.08727'
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.9562
    std: 0.0012
    paper_value: 0.9562
    paper_std: 0.0012
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9562
    true_std: 0.0012
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9562
    sort_std: 0.0012
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.9531
    std: 0.0007
    paper_value: 0.9531
    paper_std: 0.0007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9559
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2206.12933'
    at_pub_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0028000000000000247
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9559
    true_std: 0.0007
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0028000000000000247
    has_value_note: false
    value_note: ''
    sort_value: 0.9559
    sort_std: 0.0007
    global_rank: 109
    paper_rank: 131
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    comparison_source_arxiv: '2206.12933'
    is_best: false
    is_std_outlier: false
  - model: Bandana
    model_key: bandana
    model_plain: Bandana
    value: 0.9557
    std: 0.0003
    paper_value: 0.9557
    paper_std: 0.0003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9557
    true_std: 0.0003
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9557
    sort_std: 0.0003
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
  - model: GiGaMAE
    model_key: gigamae
    model_plain: GiGaMAE
    value: 0.9553
    std: 0.0003
    paper_value: 0.9553
    paper_std: 0.0003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9553
    true_std: 0.0003
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9553
    sort_std: 0.0003
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
  - model: GraphMAE2
    model_key: graphmae2
    model_plain: GraphMAE2
    value: 0.9525
    std: 0.0005
    paper_value: 0.9525
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.949
    at_pub_std: 0.001
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-12-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0035000000000000586
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.955
    true_std: 0.002
    value_gap_source_arxiv: '2512.13235'
    value_gap_source_title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0024999999999999467
    has_value_note: false
    value_note: ''
    sort_value: 0.955
    sort_std: 0.002
    global_rank: 119
    paper_rank: 134
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    comparison_source_arxiv: '2410.10241'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.951
    std: 0.0004
    paper_value: 0.951
    paper_std: 0.0004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9544
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0034000000000000696
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9544
    true_std: 0.0027
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.0034000000000000696
    has_value_note: false
    value_note: ''
    sort_value: 0.9544
    sort_std: 0.0027
    global_rank: 123
    paper_rank: 145
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    comparison_source_arxiv: '2301.12063'
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.9515
    std: 0.0011
    paper_value: 0.9515
    paper_std: 0.0011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.956
    at_pub_std: 0.002
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0044999999999999485
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9515
    true_std: 0.0011
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9515
    sort_std: 0.0011
    global_rank: 141
    paper_rank: 141
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    comparison_source_arxiv: '2410.10241'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9304
    std: 0.0003
    paper_value: 0.9304
    paper_std: 0.0003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.952
    at_pub_std: 0.001
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.021599999999999953
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9492
    true_std: 0.0007
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.01880000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9492
    sort_std: 0.0007
    global_rank: 147
    paper_rank: 206
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    comparison_source_arxiv: '2410.10241'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9489
    std: 0.0009
    paper_value: 0.9489
    paper_std: 0.0009
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.948
    at_pub_std: 0.002
    at_pub_source_arxiv: '2410.10241'
    at_pub_source_title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    at_pub_source_date_iso: '2024-10-14'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9489
    true_std: 0.0009
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9489
    sort_std: 0.0009
    global_rank: 151
    paper_rank: 151
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.944
    std: 0.0007
    paper_value: 0.944
    paper_std: 0.0007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.9458
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2106.05470'
    at_pub_source_title: Automated Self-Supervised Learning for Graphs
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0018000000000000238
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9452
    true_std: 0.0
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.0012000000000000899
    has_value_note: false
    value_note: ''
    sort_value: 0.9452
    sort_std: 0.0
    global_rank: 156
    paper_rank: 160
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    value: 0.9432
    std: 0.0004
    paper_value: 0.9432
    paper_std: 0.0004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.931
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.012199999999999989
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9432
    true_std: 0.0004
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9432
    sort_std: 0.0004
    global_rank: 162
    paper_rank: 162
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.9364
    std: 0.0008
    paper_value: 0.9364
    paper_std: 0.0008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Physics dataset
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.943
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.006599999999999939
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9364
    true_std: 0.0008
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9364
    sort_std: 0.0008
    global_rank: 181
    paper_rank: 181
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: PROTEINS
  rows:
  - model: Graphormer-SPIS
    model_key: gmn
    model_plain: Graphormer-SPIS
    value: 0.8225
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: ci-gnn
    model_plain: Graphormer-SPIS
    value: 0.82
    std: 0.02
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.01642'
    title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network for Interpretable
      Brain Network-Based Psychiatric Diagnosis'
    date: Jan 4, 2023
    date_display: Jan 2023
    date_iso: '2023-01-04'
    venue: Neural Networks
    codebase_url: https://github.com/ZKZ-Brain/CI-GNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.82
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: diffpool+gpl
    model_plain: Graphormer-SPIS
    value: 0.8196
    std: 0.0286
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Applied intelligence (Boston)
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8196
    sort_std: 0.0286
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.751
    std: 0.035
    paper_value: 0.751
    paper_std: 0.035
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8161
    at_pub_std: 0.0232
    at_pub_source_arxiv: '2407.11361'
    at_pub_source_title: 'Graph Structure Prompt Learning: A Novel Methodology to
      Improve Performance of Graph Neural Networks'
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06510000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8161
    true_std: 0.0232
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.06510000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8161
    sort_std: 0.0232
    global_rank: 4
    paper_rank: 248
    rank_delta: 244
    rank_delta_abs: 244
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    comparison_source_arxiv: '2407.11361'
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.762
    std: 0.028
    paper_value: 0.762
    paper_std: 0.028
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.788
    at_pub_std: 0.041
    at_pub_source_arxiv: '2312.08671'
    at_pub_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    at_pub_source_date_iso: '2023-12-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.026000000000000023
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.041
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.026000000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.041
    global_rank: 27
    paper_rank: 136
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BSG
    model_key: bsg
    model_plain: BSG
    value: 0.7621
    std: 0.004
    paper_value: 0.7621
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7621
    true_std: 0.004
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7621
    sort_std: 0.004
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
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.733
    std: 0.008
    paper_value: 0.733
    paper_std: 0.008
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.7568
    at_pub_std: 0.0255
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.023800000000000043
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7568
    true_std: 0.005
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.023800000000000043
    has_value_note: false
    value_note: ''
    sort_value: 0.7568
    sort_std: 0.005
    global_rank: 187
    paper_rank: 360
    rank_delta: 173
    rank_delta_abs: 173
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
    value: 0.729
    std: 0.006
    paper_value: 0.729
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.756
    at_pub_std: 0.004
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.027000000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.756
    true_std: 0.004
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.027000000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.004
    global_rank: 192
    paper_rank: 380
    rank_delta: 188
    rank_delta_abs: 188
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.7549
    std: 0.004
    paper_value: 0.7549
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.004
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.004
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.753
    std: 0.005
    paper_value: 0.753
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.753
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2309.16014'
    at_pub_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    at_pub_source_date_iso: '2023-09-27'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.753
    true_std: 0.005
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.753
    sort_std: 0.005
    global_rank: 224
    paper_rank: 224
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
    value: 0.75
    std: 0.029
    paper_value: 0.75
    paper_std: 0.029
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.7402
    at_pub_std: 0.003
    at_pub_source_arxiv: '2405.01350'
    at_pub_source_title: Community-Invariant Graph Contrastive Learning
    at_pub_source_date_iso: '2024-05-02'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.009800000000000031
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.75
    true_std: 0.029
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.75
    sort_std: 0.029
    global_rank: 262
    paper_rank: 262
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.744
    std: 0.005
    paper_value: 0.744
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.7489
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0049000000000000155
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7489
    true_std: 0.0065
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0049000000000000155
    has_value_note: false
    value_note: ''
    sort_value: 0.7489
    sort_std: 0.0065
    global_rank: 275
    paper_rank: 306
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.746
    std: 0.004
    paper_value: 0.746
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.746
    at_pub_std: 0.004
    at_pub_source_arxiv: '2401.16011'
    at_pub_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    at_pub_source_date_iso: '2024-01-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.746
    true_std: 0.004
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.004
    global_rank: 291
    paper_rank: 291
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.744
    std: 0.005
    paper_value: 0.744
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.7444
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2202.03104'
    at_pub_source_title: 'SimGRACE: A Simple Framework for Graph Contrastive Learning
      without Data Augmentation'
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7444
    true_std: 0.0031
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.7444
    sort_std: 0.0031
    global_rank: 306
    paper_rank: 306
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.733
    std: 0.021
    paper_value: 0.733
    paper_std: 0.021
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.733
    at_pub_std: 0.0205
    at_pub_source_arxiv: '1707.05005'
    at_pub_source_title: 'graph2vec: Learning Distributed Representations of Graphs'
    at_pub_source_date_iso: '2017-07-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.733
    true_std: 0.0205
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.733
    sort_std: 0.0205
    global_rank: 361
    paper_rank: 361
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGCL
    model_key: infogcl
    model_plain: InfoGCL
    value: 0.7296
    std: 0.03
    paper_value: 0.7296
    paper_std: 0.03
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical task description
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7296
    true_std: 0.03
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7296
    sort_std: 0.03
    global_rank: 379
    paper_rank: 379
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
- &id001
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.79
    std: 0.005
    paper_value: 0.79
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.13959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 611
    rank_delta: 590
    rank_delta_abs: 590
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.79
    std: 0.003
    paper_value: 0.79
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 611
    rank_delta: 588
    rank_delta_abs: 588
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.8081
    std: 0.0038
    paper_value: 0.8081
    paper_std: 0.0038
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.884
    at_pub_std: 0.006
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07589999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.884
    true_std: 0.006
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.07589999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.006
    global_rank: 155
    paper_rank: 403
    rank_delta: 248
    rank_delta_abs: 248
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.82
    std: 0.0019
    paper_value: 0.82
    paper_std: 0.0019
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8748
    at_pub_std: 0.002
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05480000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8748
    true_std: 0.002
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.05480000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8748
    sort_std: 0.002
    global_rank: 212
    paper_rank: 343
    rank_delta: 131
    rank_delta_abs: 131
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.806
    std: 0.004
    paper_value: 0.806
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.873
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06699999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.06699999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 216
    paper_rank: 418
    rank_delta: 202
    rank_delta_abs: 202
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7946
    std: 0.0043
    paper_value: 0.7946
    paper_std: 0.0043
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8725
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07790000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8725
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.07790000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8725
    sort_std: 0.0012
    global_rank: 218
    paper_rank: 542
    rank_delta: 324
    rank_delta_abs: 324
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7883
    std: 0.0077
    paper_value: 0.7883
    paper_std: 0.0077
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8708
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08250000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8708
    true_std: 0.0017
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.08250000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8708
    sort_std: 0.0017
    global_rank: 226
    paper_rank: 641
    rank_delta: 415
    rank_delta_abs: 415
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.684
    std: 0.0049
    paper_value: 0.684
    paper_std: 0.0049
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.18499999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.18499999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 233
    paper_rank: 884
    rank_delta: 651
    rank_delta_abs: 651
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
  - model: SSL
    model_key: ssl
    model_plain: SSL
    value: 0.8413
    std: 0.0023
    paper_value: 0.8413
    paper_std: 0.0023
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8413
    true_std: 0.0023
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8413
    sort_std: 0.0023
    global_rank: 291
    paper_rank: 291
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Bandana
    model_key: bandana
    model_plain: Bandana
    value: 0.8277
    std: 0.0049
    paper_value: 0.8277
    paper_std: 0.0049
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8353
    at_pub_std: 0.0051
    at_pub_source_arxiv: '2408.13471'
    at_pub_source_title: Disentangled Generative Graph Representation Learning
    at_pub_source_date_iso: '2024-08-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.007600000000000051
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8353
    true_std: 0.0051
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.007600000000000051
    has_value_note: false
    value_note: ''
    sort_value: 0.8353
    sort_std: 0.0051
    global_rank: 306
    paper_rank: 323
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.7736
    std: 0.006
    paper_value: 0.7736
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8307
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2410.15355'
    at_pub_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    at_pub_source_date_iso: '2024-10-20'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05710000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8307
    true_std: 0.0029
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.05710000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8307
    sort_std: 0.0029
    global_rank: 314
    paper_rank: 754
    rank_delta: 440
    rank_delta_abs: 440
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    comparison_source_arxiv: '2410.15355'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.7724
    std: 0.011
    paper_value: 0.7724
    paper_std: 0.011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.8294
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2410.15355'
    at_pub_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    at_pub_source_date_iso: '2024-10-20'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05700000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8294
    true_std: 0.0031
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.05700000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8294
    sort_std: 0.0031
    global_rank: 319
    paper_rank: 756
    rank_delta: 437
    rank_delta_abs: 437
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    comparison_source_arxiv: '2410.15355'
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.8151
    std: 0.01
    paper_value: 0.8151
    paper_std: 0.01
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8151
    true_std: 0.01
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8151
    sort_std: 0.01
    global_rank: 361
    paper_rank: 361
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE2
    model_key: graphmae2
    model_plain: GraphMAE2
    value: 0.8123
    std: 0.0057
    paper_value: 0.8123
    paper_std: 0.0057
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: 0.814
    at_pub_std: 0.005
    at_pub_source_arxiv: '2408.13471'
    at_pub_source_title: Disentangled Generative Graph Representation Learning
    at_pub_source_date_iso: '2024-08-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0016999999999999238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.005
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0016999999999999238
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.005
    global_rank: 367
    paper_rank: 378
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.8112
    std: 0.0053
    paper_value: 0.8112
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8112
    true_std: 0.0053
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8112
    sort_std: 0.0053
    global_rank: 384
    paper_rank: 384
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GiGaMAE
    model_key: gigamae
    model_plain: GiGaMAE
    value: 0.8055
    std: 0.0075
    paper_value: 0.8055
    paper_std: 0.0075
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8055
    true_std: 0.0075
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8055
    sort_std: 0.0075
    global_rank: 422
    paper_rank: 422
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
    value: 0.8044
    std: 0.0074
    paper_value: 0.8044
    paper_std: 0.0074
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split
    date: Apr 16, 2025
    date_display: Apr 2025
    date_iso: '2025-04-16'
    published_venue: WWW 2025
    published_conference: WWW 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8044
    true_std: 0.0074
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8044
    sort_std: 0.0074
    global_rank: 431
    paper_rank: 431
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
- benchmark: TU Dortmund
  datasets:
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: PROTEINS
      dataset_slug: proteins
single_proposed_model: BSG
main_figure: /figures/2504.12011/main_figure.jpegoptim.jpg
---

