---
title: Self-Contrastive Graph Diffusion Network
arxiv_id: '2307.14613'
source_url: ''
authors:
- name: Yixuan Ma
  orcid: null
  s2_author_id: '2287012483'
  s2_url: null
- name: Kun Zhan
  orcid: null
  s2_author_id: '1918754'
  s2_url: null
published_date: Jul 27, 2023
published_date_iso: '2023-07-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Contrastive learning has been proven to be a successful approach in graph
  self-supervised learning. Augmentation techniques and sampling strategies are crucial
  in contrastive learning, but in most existing works, augmentation techniques require
  careful design, and their sampling strategies can only capture a small amount of
  intrinsic supervision information. Additionally, the existing methods require complex
  designs to obtain two different representations of the data. To overcome these limitations,
  we propose a novel framework called the Self-Contrastive Graph Diffusion Network
  (SCGDN). Our framework consists of two main components: the Attentional Module (AttM)
  and the Diffusion Module (DiFM). AttM aggregates higher-order structure and feature
  information to get an excellent embedding, while DiFM balances the state of each
  node in the graph through Laplacian diffusion learning and allows the cooperative
  evolution of adjacency and feature information in the graph. Unlike existing methodologies,
  SCGDN is an augmentation-free approach that avoids "sampling bias" and semantic
  drift, without the need for pre-training. We conduct a high-quality sampling of
  samples based on structure and feature information. If two nodes are neighbors,
  they are considered positive samples of each other. If two disconnected nodes are
  also unrelated on $k$NN graph, they are considered negative samples for each other.
  The contrastive objective reasonably uses our proposed sampling strategies, and
  the redundancy reduction term minimizes redundant information in the embedding and
  can well retain more discriminative information. In this novel framework, the graph
  self-contrastive learning paradigm gives expression to a powerful force. SCGDN effectively
  balances between preserving high-order structure information and avoiding overfitting.
  The results manifest that SCGDN can consistently generate outperformance over both
  the contrastive methods and the classical methods.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SCGDN
mrr: 0.2315
adjusted_mrr: 0.2315
mrr_dataset_count: 3
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 3
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: AMAP
  rows:
  - model: SCGDN
    model_key: idcrn
    model_plain: SCGDN
    value: 0.8208
    std: 0.0018
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_display: Feb 2022
    date_iso: '2022-02-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8208
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SCGDN
    model_key: dcrn
    model_plain: SCGDN
    value: 0.7966
    std: 0.0025
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_display: Feb 2022
    date_iso: '2022-02-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7966
    sort_std: 0.0025
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
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
    global_rank: 3
    paper_rank: 10
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improved Dual Correlation Reduction Network
    comparison_source_arxiv: '2202.12533'
    is_best: false
    is_std_outlier: false
  - model: SCGDN
    model_key: scgdn
    model_plain: SCGDN
    value: 0.7527
    std: 0.0018
    paper_value: 0.7527
    paper_std: 0.0018
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7527
    true_std: 0.0018
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7527
    sort_std: 0.0018
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
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.7103
    std: 0.0064
    paper_value: 0.7103
    paper_std: 0.0064
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7103
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7103
    true_std: 0.0064
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7103
    sort_std: 0.0064
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
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.6999
    std: 0.0034
    paper_value: 0.6999
    paper_std: 0.0034
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6999
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6999
    true_std: 0.0034
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6999
    sort_std: 0.0034
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
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
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
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
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6135
    at_pub_std: 0.008
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06729999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6808
    true_std: 0.0176
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0176
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.5447
    std: 0.0083
    paper_value: 0.5447
    paper_std: 0.0083
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6676
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.12290000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5447
    true_std: 0.0083
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5447
    sort_std: 0.0083
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6283
    at_pub_std: 0.0159
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-02-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4273
    true_std: 0.0102
    value_gap_source_arxiv: '2202.12533'
    value_gap_source_title: Improved Dual Correlation Reduction Network
    value_gap_source_is_current_paper: false
    value_gap: 0.09850000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4273
    sort_std: 0.0102
    global_rank: 35
    paper_rank: 37
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    value: 0.3837
    std: 0.0029
    paper_value: 0.3837
    paper_std: 0.0029
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6639
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.28020000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3837
    true_std: 0.0029
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3837
    sort_std: 0.0029
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.3197
    std: 0.0044
    paper_value: 0.3197
    paper_std: 0.0044
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
    protocol_note: Standard clustering task on AMAP dataset
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6592
    at_pub_std: 0.008
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.3395
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3197
    true_std: 0.0044
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3197
    sort_std: 0.0044
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
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
  dataset: BAT
  rows:
  - model: K-means
    model_key: convert
    model_plain: K-means
    value: 0.7777
    std: 0.0148
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.08963'
    title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    date: Aug 17, 2023
    date_display: Aug 2023
    date_iso: '2023-08-17'
    venue: ACM Multimedia
    codebase_url: https://github.com/xihongyang1999/CONVERT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7777
    sort_std: 0.0148
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: K-means
    model_key: graphlearner
    model_plain: K-means
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
    global_rank: 2
    sort_value: 0.754
    sort_std: 0.0088
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCGDN
    model_key: scgdn
    model_plain: SCGDN
    value: 0.7449
    std: 0.0026
    paper_value: 0.7449
    paper_std: 0.0026
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7449
    true_std: 0.0026
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7449
    sort_std: 0.0026
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.2964
    std: 0.0049
    paper_value: 0.2964
    paper_std: 0.0049
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7047
    at_pub_std: 0.037
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.4083
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7047
    true_std: 0.037
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.4083
    has_value_note: false
    value_note: ''
    sort_value: 0.7047
    sort_std: 0.037
    global_rank: 8
    paper_rank: 30
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.5223
    std: 0.0003
    paper_value: 0.5223
    paper_std: 0.0003
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1764
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.1764
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 9
    paper_rank: 15
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.5608
    std: 0.0089
    paper_value: 0.5608
    paper_std: 0.0089
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5608
    true_std: 0.0089
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5608
    sort_std: 0.0089
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
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.509
    std: 0.0012
    paper_value: 0.509
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.509
    true_std: 0.0012
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.509
    sort_std: 0.0012
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
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    value: 0.5083
    std: 0.0323
    paper_value: 0.5083
    paper_std: 0.0323
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5083
    true_std: 0.0323
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5083
    sort_std: 0.0323
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
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.4653
    std: 0.0057
    paper_value: 0.4653
    paper_std: 0.0057
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4653
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4653
    true_std: 0.0057
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4653
    sort_std: 0.0057
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
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.4233
    std: 0.0051
    paper_value: 0.4233
    paper_std: 0.0051
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4233
    at_pub_std: 0.0051
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4233
    true_std: 0.0051
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4233
    sort_std: 0.0051
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
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    value: 0.3994
    std: 0.0057
    paper_value: 0.3994
    paper_std: 0.0057
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3994
    true_std: 0.0057
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3994
    sort_std: 0.0057
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
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.3484
    std: 0.0015
    paper_value: 0.3484
    paper_std: 0.0015
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
    protocol_note: Clustering task on BAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3484
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3484
    true_std: 0.0015
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3484
    sort_std: 0.0015
    global_rank: 30
    paper_rank: 30
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
- &id003
  dataset: EAT
  rows:
  - model: DFCN
    model_key: scagc
    model_plain: DFCN
    value: 0.7277
    std: 0.0016
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7277
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DFCN
    model_key: scgc
    model_plain: DFCN
    value: 0.7222
    std: 0.0097
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7222
    sort_std: 0.0097
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DFCN
    model_key: age
    model_plain: DFCN
    value: 0.7174
    std: 0.0093
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7174
    sort_std: 0.0093
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.4295
    std: 0.0004
    paper_value: 0.4295
    paper_std: 0.0004
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7682
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.3387
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7125
    true_std: 0.0031
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.28300000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7125
    sort_std: 0.0031
    global_rank: 4
    paper_rank: 21
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    value: 0.3472
    std: 0.0016
    paper_value: 0.3472
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7596
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.41240000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6987
    true_std: 0.0054
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.3515
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.0054
    global_rank: 5
    paper_rank: 25
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: SCGDN
    model_key: scgdn
    model_plain: SCGDN
    value: 0.5763
    std: 0.001
    paper_value: 0.5763
    paper_std: 0.001
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5763
    true_std: 0.001
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5763
    sort_std: 0.001
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.2535
    std: 0.0075
    paper_value: 0.2535
    paper_std: 0.0075
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4107
    at_pub_std: 0.0312
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1572
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.21649999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.06
    global_rank: 17
    paper_rank: 29
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: true
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    value: 0.4308
    std: 0.0326
    paper_value: 0.4308
    paper_std: 0.0326
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7157
    at_pub_std: 0.0248
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2849
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4308
    true_std: 0.0326
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4308
    sort_std: 0.0326
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.4254
    std: 0.0045
    paper_value: 0.4254
    paper_std: 0.0045
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7702
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.3448
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4254
    true_std: 0.0045
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4254
    sort_std: 0.0045
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    value: 0.352
    std: 0.0017
    paper_value: 0.352
    paper_std: 0.0017
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7681
    at_pub_std: 0.0145
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.4161
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.352
    true_std: 0.0017
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.352
    sort_std: 0.0017
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.3053
    std: 0.0147
    paper_value: 0.3053
    paper_std: 0.0147
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4375
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.13219999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3053
    true_std: 0.0147
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3053
    sort_std: 0.0147
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    value: 0.2502
    std: 0.0021
    paper_value: 0.2502
    paper_std: 0.0021
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5153
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2651
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2502
    true_std: 0.0021
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2502
    sort_std: 0.0021
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    value: 0.2182
    std: 0.0098
    paper_value: 0.2182
    paper_std: 0.0098
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
    protocol_note: Clustering task on EAT dataset using standard split
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5455
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-08-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.3273
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2182
    true_std: 0.0098
    value_gap_source_arxiv: '2308.08963'
    value_gap_source_title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2182
    sort_std: 0.0098
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: BAT
      dataset_slug: bat
    - dataset: EAT
      dataset_slug: eat
single_proposed_model: SCGDN
main_figure: /figures/2307.14613/main_figure.jpegoptim.jpg
---

