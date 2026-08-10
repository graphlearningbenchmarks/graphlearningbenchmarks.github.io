---
title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised Learning on Diverse
  Graphs with Heterogeneous Specialization'
arxiv_id: '2510.21207'
source_url: ''
authors:
- name: Yunlong Chu
  orcid: null
  s2_author_id: '2393020088'
  s2_url: null
- name: Minglai Shao
  orcid: null
  s2_author_id: '2343960608'
  s2_url: null
- name: Zengyi Wo
  orcid: null
  s2_author_id: '2300602182'
  s2_url: null
- name: Bing Hao
  orcid: null
  s2_author_id: '2386990047'
  s2_url: null
- name: Yuhang Liu
  orcid: null
  s2_author_id: '2386989768'
  s2_url: null
- name: Ruijie Wang
  orcid: null
  s2_author_id: '2375748651'
  s2_url: null
- name: Jianxin Li
  orcid: null
  s2_author_id: '2386991786'
  s2_url: null
published_date: Oct 24, 2025
published_date_iso: '2025-10-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks (GNNs) face a fundamental adaptability challenge:
  their fixed message-passing architectures struggle with the immense diversity of
  real-world graphs, where optimal computational strategies vary by local structure
  and task. While Mixture-of-Experts (MoE) offers a promising pathway to adaptability,
  existing graph MoE methods remain constrained by their reliance on supervised signals
  and instability when training heterogeneous experts. We introduce ADaMoRE (Adaptive
  Mixture of Residual Experts), a principled framework that enables robust, fully
  unsupervised training of heterogeneous MoE on graphs. ADaMoRE employs a backbone-residual
  expert architecture where foundational encoders provide stability while specialized
  residual experts capture diverse computational patterns. A structurally-aware gating
  network performs fine-grained node routing. The entire architecture is trained end-to-end
  using a unified unsupervised objective, which integrates a primary reconstruction
  task with an information-theoretic diversity regularizer to explicitly enforce functional
  specialization among the experts. Theoretical analysis confirms our design improves
  data efficiency and training stability. Extensive evaluation across 16 benchmarks
  validates ADaMoRE''s state-of-the-art performance in unsupervised node classification
  and few-shot learning, alongside superior generalization, training efficiency, and
  faster convergence on diverse graphs and tasks.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ADaMoRE
mrr: 0.0053
adjusted_mrr: 0.0053
mrr_dataset_count: 5
benchmark_categories:
- TU Dortmund
- Heterophilic Graphs
- Heterophily Benchmark
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 2
  total: 5
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id004
  dataset: Actor
  rows:
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7623
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    sort_value: 0.7623
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiGGR
    model_key: diggr
    model_plain: DiGGR
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TRIGON
    model_key: trigon
    model_plain: TRIGON
    value: 0.4402
    std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.19071'
    title: Dynamic Triangulation-Based Graph Rewiring for Graph Neural Networks
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Hugo-Attali/TRIGON-CIKM-2025
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4026
    std: 0.0108
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 55
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S3GCL
    model_key: s3gcl
    model_plain: S3GCL
    value: 0.2653
    std: 0.005
    paper_value: 0.2653
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4006
    true_std: 0.0158
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.13530000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4006
    sort_std: 0.0158
    global_rank: 63
    paper_rank: 472
    rank_delta: 409
    rank_delta_abs: 409
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3899
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 87
    sort_value: 0.3899
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.2928
    std: 0.008
    paper_value: 0.2928
    paper_std: 0.008
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3655
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.07269999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3712
    true_std: 0.0067
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07839999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.3712
    sort_std: 0.0067
    global_rank: 154
    paper_rank: 423
    rank_delta: 269
    rank_delta_abs: 269
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: HGRL
    model_key: hgrl
    model_plain: HGRL
    value: 0.2979
    std: 0.011
    paper_value: 0.2979
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3697
    at_pub_std: 0.0098
    at_pub_source_arxiv: '2307.16026'
    at_pub_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07179999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3697
    true_std: 0.0098
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.07179999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.3697
    sort_std: 0.0098
    global_rank: 163
    paper_rank: 414
    rank_delta: 251
    rank_delta_abs: 251
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    comparison_source_arxiv: '2307.16026'
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.3121
    std: 0.003
    paper_value: 0.3121
    paper_std: 0.003
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3121
    true_std: 0.003
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3121
    sort_std: 0.003
    global_rank: 375
    paper_rank: 375
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
- &id003
  dataset: Cornell
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.948
    std: 0.038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/AaltoML/heterophily-imp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.948
    sort_std: 0.038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9429
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9136
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2212.03654'
    title: Node-oriented Spectral Filtering for Graph Neural Networks
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 25
    sort_value: 0.9136
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.7
    std: 0.0534
    paper_value: 0.7
    paper_std: 0.0534
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
    source_ref: GREET [29]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8514
    at_pub_std: 0.0487
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1514000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8514
    true_std: 0.0487
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1514000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8514
    sort_std: 0.0487
    global_rank: 109
    paper_rank: 345
    rank_delta: 236
    rank_delta_abs: 236
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8269
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 165
    sort_value: 0.8269
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S3GCL
    model_key: s3gcl
    model_plain: S3GCL
    value: 0.7333
    std: 0.0734
    paper_value: 0.7333
    paper_std: 0.0734
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
    source_ref: S3GCL [30]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8127
    true_std: 0.0367
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07940000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8127
    sort_std: 0.0367
    global_rank: 196
    paper_rank: 308
    rank_delta: 112
    rank_delta_abs: 112
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP-GCL
    model_key: sp-gcl
    model_plain: SP-GCL
    value: 0.7069
    std: 0.0651
    paper_value: 0.7069
    paper_std: 0.0651
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
    source_ref: SP-GCL [28]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7833
    at_pub_std: 0.0426
    at_pub_source_arxiv: '2506.19343'
    at_pub_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    at_pub_source_date_iso: '2025-06-24'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.07640000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7833
    true_std: 0.0426
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.07640000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7833
    sort_std: 0.0426
    global_rank: 238
    paper_rank: 335
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.7737
    std: 0.0421
    paper_value: 0.7737
    paper_std: 0.0421
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7737
    true_std: 0.0421
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7737
    sort_std: 0.0421
    global_rank: 258
    paper_rank: 258
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.5868
    std: 0.0504
    paper_value: 0.5868
    paper_std: 0.0504
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
    source_ref: DGI [20]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6335
    at_pub_std: 0.0461
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.046699999999999964
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7082
    true_std: 0.0271
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.12140000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7082
    sort_std: 0.0271
    global_rank: 334
    paper_rank: 461
    rank_delta: 127
    rank_delta_abs: 127
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSSL
    model_key: dssl
    model_plain: DSSL
    value: 0.6928
    std: 0.0601
    paper_value: 0.6928
    paper_std: 0.0601
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
    source_ref: DSSL [27]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5363
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15649999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6928
    true_std: 0.0601
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6928
    sort_std: 0.0601
    global_rank: 348
    paper_rank: 348
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GDAE
    model_key: gdae
    model_plain: GDAE
    value: 0.6632
    std: 0.0817
    paper_value: 0.6632
    paper_std: 0.0817
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
    source_ref: GDAE [22]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6632
    true_std: 0.0817
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6632
    sort_std: 0.0817
    global_rank: 382
    paper_rank: 382
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
    value: 0.655
    std: 0.0744
    paper_value: 0.655
    paper_std: 0.0744
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
    source_ref: MaskGAE [21]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4324
    at_pub_std: 0.051
    at_pub_source_arxiv: '2506.19343'
    at_pub_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    at_pub_source_date_iso: '2025-06-24'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.22260000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.655
    true_std: 0.0744
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.655
    sort_std: 0.0744
    global_rank: 391
    paper_rank: 391
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    comparison_source_arxiv: '2506.19343'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.6126
    std: 0.0401
    paper_value: 0.6126
    paper_std: 0.0401
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
    source_ref: MVGRL [23]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.643
    at_pub_std: 0.0543
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.030399999999999983
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.643
    true_std: 0.0543
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.030399999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.0543
    global_rank: 407
    paper_rank: 432
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.4585
    std: 0.0551
    paper_value: 0.4585
    paper_std: 0.0551
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
    source_ref: GRACE [24]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.564
    at_pub_std: 0.021
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.10549999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6066
    true_std: 0.0294
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.1481
    has_value_note: false
    value_note: ''
    sort_value: 0.6066
    sort_std: 0.0294
    global_rank: 440
    paper_rank: 600
    rank_delta: 160
    rank_delta_abs: 160
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for
      Graph Message-passing'
    comparison_source_arxiv: '2507.20127'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.5498
    std: 0.0602
    paper_value: 0.5498
    paper_std: 0.0602
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
    source_ref: BGRL [26]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.573
    at_pub_std: 0.0551
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0232
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.573
    true_std: 0.0551
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0232
    has_value_note: false
    value_note: ''
    sort_value: 0.573
    sort_std: 0.0551
    global_rank: 489
    paper_rank: 506
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBT
    model_key: gbt
    model_plain: GBT
    value: 0.4932
    std: 0.0452
    paper_value: 0.4932
    paper_std: 0.0452
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
    source_ref: GBT [25]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4932
    true_std: 0.0452
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4932
    sort_std: 0.0452
    global_rank: 571
    paper_rank: 571
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
- &id001
  dataset: ENZYMES
  rows:
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.7866
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
    sort_value: 0.7866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.755
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
    global_rank: 2
    sort_value: 0.755
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGW SP
    model_key: tfgw sp (l=2)
    model_plain: TFGW SP
    value: 0.751
    std: 0.05
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.751
    sort_std: 0.05
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7
    std: 0.04944
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
    global_rank: 17
    sort_value: 0.7
    sort_std: 0.04944
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.2024
    std: 0.0639
    paper_value: 0.2024
    paper_std: 0.0639
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.685
    at_pub_std: 0.05241
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.48260000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.685
    true_std: 0.05241
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.48260000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.685
    sort_std: 0.05241
    global_rank: 21
    paper_rank: 329
    rank_delta: 308
    rank_delta_abs: 308
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
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
    global_rank: 27
    sort_value: 0.68167
    sort_std: 0.05449
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.193
    std: 0.0636
    paper_value: 0.193
    paper_std: 0.0636
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.665
    at_pub_std: 0.0691
    at_pub_source_arxiv: '2012.08734'
    at_pub_source_title: Hierarchical Graph Capsule Network
    at_pub_source_date_iso: '2020-12-16'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.47200000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.665
    true_std: 0.0691
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: 0.47200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.665
    sort_std: 0.0691
    global_rank: 37
    paper_rank: 333
    rank_delta: 296
    rank_delta_abs: 296
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Capsule Network
    comparison_source_arxiv: '2012.08734'
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
    global_rank: 133
    sort_value: 0.55833
    sort_std: 0.03516
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.1993
    std: 0.0565
    paper_value: 0.1993
    paper_std: 0.0565
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.551
    at_pub_std: 0.016
    at_pub_source_arxiv: '2402.15270'
    at_pub_source_title: Smoothed Graph Contrastive Learning via Seamless Proximity
      Integration
    at_pub_source_date_iso: '2024-02-23'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3517
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.551
    true_std: 0.016
    value_gap_source_arxiv: '2402.15270'
    value_gap_source_title: Smoothed Graph Contrastive Learning via Seamless Proximity
      Integration
    value_gap_source_is_current_paper: false
    value_gap: 0.3517
    has_value_note: false
    value_note: ''
    sort_value: 0.551
    sort_std: 0.016
    global_rank: 140
    paper_rank: 330
    rank_delta: 190
    rank_delta_abs: 190
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Smoothed Graph Contrastive Learning via Seamless Proximity
      Integration
    comparison_source_arxiv: '2402.15270'
    is_best: false
    is_std_outlier: false
  - model: GraphPrompt
    model_key: graphprompt
    model_plain: GraphPrompt
    value: 0.2185
    std: 0.0617
    paper_value: 0.2185
    paper_std: 0.0617
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2567
    at_pub_std: 0.0349
    at_pub_source_arxiv: '2501.15142'
    at_pub_source_title: 'DAGPrompT: Pushing the Limits of Graph Prompting with a
      Distribution-aware Graph Prompt Tuning Approach'
    at_pub_source_date_iso: '2025-01-25'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-01-25'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.038199999999999984
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.2567
    true_std: 0.0349
    value_gap_source_arxiv: '2501.15142'
    value_gap_source_title: 'DAGPrompT: Pushing the Limits of Graph Prompting with
      a Distribution-aware Graph Prompt Tuning Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.038199999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.2567
    sort_std: 0.0349
    global_rank: 286
    paper_rank: 316
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.2523
    std: 0.047
    paper_value: 0.2523
    paper_std: 0.047
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2523
    true_std: 0.047
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2523
    sort_std: 0.047
    global_rank: 289
    paper_rank: 289
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMoE-GIN
    model_key: gmoe-gin
    model_plain: GMoE-GIN
    value: 0.2315
    std: 0.0363
    paper_value: 0.2315
    paper_std: 0.0363
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2315
    true_std: 0.0363
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2315
    sort_std: 0.0363
    global_rank: 299
    paper_rank: 299
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSSL
    model_key: dssl
    model_plain: DSSL
    value: 0.2314
    std: 0.0671
    paper_value: 0.2314
    paper_std: 0.0671
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2314
    true_std: 0.0671
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2314
    sort_std: 0.0671
    global_rank: 300
    paper_rank: 300
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ProNoG
    model_key: pronog
    model_plain: ProNoG
    value: 0.2255
    std: 0.067
    paper_value: 0.2255
    paper_std: 0.067
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2255
    true_std: 0.067
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2255
    sort_std: 0.067
    global_rank: 307
    paper_rank: 307
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMoE-GCN
    model_key: gmoe-gcn
    model_plain: GMoE-GCN
    value: 0.2233
    std: 0.0356
    paper_value: 0.2233
    paper_std: 0.0356
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2233
    true_std: 0.0356
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2233
    sort_std: 0.0356
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.2157
    std: 0.0537
    paper_value: 0.2157
    paper_std: 0.0537
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2157
    true_std: 0.0537
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2157
    sort_std: 0.0537
    global_rank: 318
    paper_rank: 318
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMOE-SAGE
    model_key: gmoe-sage
    model_plain: GMOE-SAGE
    value: 0.213
    std: 0.0329
    paper_value: 0.213
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.213
    true_std: 0.0329
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.213
    sort_std: 0.0329
    global_rank: 322
    paper_rank: 322
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphACL
    model_key: graphacl
    model_plain: GraphACL
    value: 0.2028
    std: 0.056
    paper_value: 0.2028
    paper_std: 0.056
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2028
    true_std: 0.056
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2028
    sort_std: 0.056
    global_rank: 329
    paper_rank: 329
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.1995
    std: 0.0594
    paper_value: 0.1995
    paper_std: 0.0594
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1995
    true_std: 0.0594
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1995
    sort_std: 0.0594
    global_rank: 330
    paper_rank: 330
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.194
    std: 0.0557
    paper_value: 0.194
    paper_std: 0.0557
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.194
    true_std: 0.0557
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.194
    sort_std: 0.0557
    global_rank: 332
    paper_rank: 332
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
- &id006
  dataset: Minesweeper
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9903
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
    global_rank: 1
    sort_value: 0.9903
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9899
    std: 0.0016
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
    global_rank: 2
    sort_value: 0.9899
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.9827
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    sort_value: 0.9827
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9744
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 9
    sort_value: 0.9744
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.8502
    std: 0.0068
    paper_value: 0.8502
    paper_std: 0.0068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8502
    true_std: 0.0068
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8502
    sort_std: 0.0068
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8176
    std: 0.0088
    paper_value: 0.8176
    paper_std: 0.0088
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
    source_ref: GREET [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8176
    true_std: 0.0088
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8176
    sort_std: 0.0088
    global_rank: 42
    paper_rank: 42
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
    value: 0.8083
    std: 0.0085
    paper_value: 0.8083
    paper_std: 0.0085
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
    source_ref: MVGRL [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8083
    true_std: 0.0085
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8083
    sort_std: 0.0085
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S3GCL
    model_key: s3gcl
    model_plain: S3GCL
    value: 0.8037
    std: 0.0081
    paper_value: 0.8037
    paper_std: 0.0081
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
    source_ref: S3GCL [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8037
    true_std: 0.0081
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8037
    sort_std: 0.0081
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
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8007
    std: 0.0065
    paper_value: 0.8007
    paper_std: 0.0065
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
    source_ref: BGRL [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8007
    true_std: 0.0065
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8007
    sort_std: 0.0065
    global_rank: 48
    paper_rank: 48
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
    value: 0.8
    std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    venue: 'Accepted to ICLR 2026. OpenReview: https://openreview.net/forum?id=FmxRzlu0rT'
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 49
    sort_value: 0.8
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7999
    std: 0.0081
    paper_value: 0.7999
    paper_std: 0.0081
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
    source_ref: GRACE [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7999
    true_std: 0.0081
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7999
    sort_std: 0.0081
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7995
    std: 0.0075
    paper_value: 0.7995
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
    source_ref: DGI [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7995
    true_std: 0.0075
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7995
    sort_std: 0.0075
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSSL
    model_key: dssl
    model_plain: DSSL
    value: 0.7979
    std: 0.0073
    paper_value: 0.7979
    paper_std: 0.0073
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
    source_ref: DSSL [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7979
    true_std: 0.0073
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7979
    sort_std: 0.0073
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP-GCL
    model_key: sp-gcl
    model_plain: SP-GCL
    value: 0.7975
    std: 0.0064
    paper_value: 0.7975
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
    source_ref: SP-GCL [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7975
    true_std: 0.0064
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7975
    sort_std: 0.0064
    global_rank: 53
    paper_rank: 53
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
    value: 0.7971
    std: 0.0072
    paper_value: 0.7971
    paper_std: 0.0072
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
    source_ref: MaskGAE [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7971
    true_std: 0.0072
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7971
    sort_std: 0.0072
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDAE
    model_key: gdae
    model_plain: GDAE
    value: 0.7966
    std: 0.0068
    paper_value: 0.7966
    paper_std: 0.0068
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
    source_ref: GDAE [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7966
    true_std: 0.0068
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7966
    sort_std: 0.0068
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBT
    model_key: gbt
    model_plain: GBT
    value: 0.7834
    std: 0.0071
    paper_value: 0.7834
    paper_std: 0.0071
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
    source_ref: GBT [cite]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7834
    true_std: 0.0071
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7834
    sort_std: 0.0071
    global_rank: 56
    paper_rank: 56
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id005
  dataset: Roman-empire
  rows:
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    value: 0.9451
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    sort_value: 0.9451
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D-CDE
    model_key: d-cde
    model_plain: D-CDE
    value: 0.9387
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_display: Nov 2024
    date_iso: '2024-11-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9387
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeScaleNet
    model_key: largescalenet
    model_plain: LargeScaleNet
    value: 0.9358
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_display: Nov 2024
    date_iso: '2024-11-28'
    venue: null
    codebase_url: https://github.com/Qin87/ScaleNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9358
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9106
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.17939'
    title: Directed Semi-Simplicial Learning with Applications to Brain Activity Decoding
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: https://github.com/ManuelLecha/ssn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 24
    sort_value: 0.9106
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.7786
    std: 0.0089
    paper_value: 0.7786
    paper_std: 0.0089
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7786
    true_std: 0.0089
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7786
    sort_std: 0.0089
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6665
    std: 0.0047
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11596'
    title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: https://github.com/Foisunt/HyperAggregation
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 141
    sort_value: 0.6665
    sort_std: 0.0047
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S3GCL
    model_key: s3gcl
    model_plain: S3GCL
    value: 0.6455
    std: 0.0075
    paper_value: 0.6455
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
    source_ref: S3GCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6455
    true_std: 0.0075
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6455
    sort_std: 0.0075
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.6389
    std: 0.0134
    paper_value: 0.6389
    paper_std: 0.0134
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
    source_ref: GREET
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6389
    true_std: 0.0134
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6389
    sort_std: 0.0134
    global_rank: 160
    paper_rank: 160
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDAE
    model_key: gdae
    model_plain: GDAE
    value: 0.629
    std: 0.0067
    paper_value: 0.629
    paper_std: 0.0067
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
    source_ref: GDAE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.629
    true_std: 0.0067
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.629
    sort_std: 0.0067
    global_rank: 163
    paper_rank: 163
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
    value: 0.6221
    std: 0.0084
    paper_value: 0.6221
    paper_std: 0.0084
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
    source_ref: MaskGAE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6221
    true_std: 0.0084
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6221
    sort_std: 0.0084
    global_rank: 166
    paper_rank: 166
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSSL
    model_key: dssl
    model_plain: DSSL
    value: 0.5969
    std: 0.0075
    paper_value: 0.5969
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
    source_ref: DSSL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5969
    true_std: 0.0075
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5969
    sort_std: 0.0075
    global_rank: 174
    paper_rank: 174
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.5079
    std: 0.0113
    paper_value: 0.5079
    paper_std: 0.0113
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
    source_ref: BGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5079
    true_std: 0.0113
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5079
    sort_std: 0.0113
    global_rank: 195
    paper_rank: 195
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP-GCL
    model_key: sp-gcl
    model_plain: SP-GCL
    value: 0.5079
    std: 0.0095
    paper_value: 0.5079
    paper_std: 0.0095
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
    source_ref: SP-GCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5079
    true_std: 0.0095
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5079
    sort_std: 0.0095
    global_rank: 196
    paper_rank: 196
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
    value: 0.5024
    std: 0.0102
    paper_value: 0.5024
    paper_std: 0.0102
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
    source_ref: GRACE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5024
    true_std: 0.0102
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5024
    sort_std: 0.0102
    global_rank: 197
    paper_rank: 197
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
    value: 0.4668
    std: 0.0073
    paper_value: 0.4668
    paper_std: 0.0073
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
    source_ref: MVGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4668
    true_std: 0.0073
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4668
    sort_std: 0.0073
    global_rank: 199
    paper_rank: 199
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.4204
    std: 0.0094
    paper_value: 0.4204
    paper_std: 0.0094
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
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.071
    at_pub_std: null
    at_pub_source_arxiv: '2508.11328'
    at_pub_source_title: 'Aligning the Spectrum: Hybrid Graph Pre-training and Prompt
      Tuning across Homophily and Heterophily'
    at_pub_source_date_iso: '2025-08-15'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.3494
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4204
    true_std: 0.0094
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4204
    sort_std: 0.0094
    global_rank: 201
    paper_rank: 201
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Aligning the Spectrum: Hybrid Graph Pre-training and
      Prompt Tuning across Homophily and Heterophily'
    comparison_source_arxiv: '2508.11328'
    is_best: false
    is_std_outlier: false
  - model: GBT
    model_key: gbt
    model_plain: GBT
    value: 0.3776
    std: 0.0085
    paper_value: 0.3776
    paper_std: 0.0085
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
    source_ref: GBT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3776
    true_std: 0.0085
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3776
    sort_std: 0.0085
    global_rank: 207
    paper_rank: 207
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
- &id002
  dataset: Texas
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.923
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 45
    sort_value: 0.923
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9001
    std: 0.023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 73
    sort_value: 0.9001
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8079
    std: 0.0441
    paper_value: 0.8079
    paper_std: 0.0441
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
    source_ref: GREET
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8703
    at_pub_std: 0.0236
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06240000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8703
    true_std: 0.0236
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.06240000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8703
    sort_std: 0.0236
    global_rank: 128
    paper_rank: 295
    rank_delta: 167
    rank_delta_abs: 167
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S3GCL
    model_key: s3gcl
    model_plain: S3GCL
    value: 0.825
    std: 0.0586
    paper_value: 0.825
    paper_std: 0.0586
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
    source_ref: S3GCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8612
    true_std: 0.0391
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03620000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8612
    sort_std: 0.0391
    global_rank: 149
    paper_rank: 242
    rank_delta: 93
    rank_delta_abs: 93
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADaMoRE
    model_key: adamore
    model_plain: ADaMoRE
    value: 0.8605
    std: 0.0576
    paper_value: 0.8605
    paper_std: 0.0576
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8605
    true_std: 0.0576
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8605
    sort_std: 0.0576
    global_rank: 151
    paper_rank: 151
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7581
    std: 0.0503
    paper_value: 0.7581
    paper_std: 0.0503
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
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6059
    at_pub_std: 0.0756
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1522
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8148
    true_std: 0.0279
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05669999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8148
    sort_std: 0.0279
    global_rank: 271
    paper_rank: 375
    rank_delta: 104
    rank_delta_abs: 104
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: SP-GCL
    model_key: sp-gcl
    model_plain: SP-GCL
    value: 0.7683
    std: 0.0582
    paper_value: 0.7683
    paper_std: 0.0582
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
    source_ref: SP-GCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8036
    at_pub_std: 0.0564
    at_pub_source_arxiv: '2506.19343'
    at_pub_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    at_pub_source_date_iso: '2025-06-24'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.0353
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8036
    true_std: 0.0564
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.0353
    has_value_note: false
    value_note: ''
    sort_value: 0.8036
    sort_std: 0.0564
    global_rank: 301
    paper_rank: 360
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDAE
    model_key: gdae
    model_plain: GDAE
    value: 0.7684
    std: 0.0668
    paper_value: 0.7684
    paper_std: 0.0668
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
    source_ref: GDAE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7684
    true_std: 0.0668
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7684
    sort_std: 0.0668
    global_rank: 360
    paper_rank: 360
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
    value: 0.7604
    std: 0.0642
    paper_value: 0.7604
    paper_std: 0.0642
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
    source_ref: MaskGAE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6486
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2506.19343'
    at_pub_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    at_pub_source_date_iso: '2025-06-24'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.11180000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7604
    true_std: 0.0642
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7604
    sort_std: 0.0642
    global_rank: 374
    paper_rank: 374
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    comparison_source_arxiv: '2506.19343'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7215
    std: 0.0453
    paper_value: 0.7215
    paper_std: 0.0453
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
    source_ref: GRACE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6354
    at_pub_std: 0.0257
    at_pub_source_arxiv: '2406.01899'
    at_pub_source_title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion
      Models'
    at_pub_source_date_iso: '2024-06-04'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08610000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7574
    true_std: 0.0312
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03589999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7574
    sort_std: 0.0312
    global_rank: 377
    paper_rank: 445
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion
      Models'
    comparison_source_arxiv: '2406.01899'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7301
    std: 0.0552
    paper_value: 0.7301
    paper_std: 0.0552
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
    source_ref: MVGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6238
    at_pub_std: 0.0561
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10629999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7301
    true_std: 0.0552
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7301
    sort_std: 0.0552
    global_rank: 428
    paper_rank: 428
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSSL
    model_key: dssl
    model_plain: DSSL
    value: 0.7273
    std: 0.0402
    paper_value: 0.7273
    paper_std: 0.0402
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
    source_ref: DSSL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6211
    at_pub_std: 0.0153
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10619999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7273
    true_std: 0.0402
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7273
    sort_std: 0.0402
    global_rank: 436
    paper_rank: 436
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GBT
    model_key: gbt
    model_plain: GBT
    value: 0.6925
    std: 0.0481
    paper_value: 0.6925
    paper_std: 0.0481
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
    source_ref: GBT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6925
    true_std: 0.0481
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6925
    sort_std: 0.0481
    global_rank: 477
    paper_rank: 477
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.6841
    std: 0.0501
    paper_value: 0.6841
    paper_std: 0.0501
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
    source_ref: BGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.658
    at_pub_std: 0.027
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.026100000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6841
    true_std: 0.0501
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6841
    sort_std: 0.0501
    global_rank: 487
    paper_rank: 487
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
  - *id003
  - *id004
- benchmark: Heterophily Benchmark
  datasets:
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Minesweeper
      dataset_slug: minesweeper
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: ADaMoRE
main_figure: /figures/2510.21207/main_figure.jpegoptim.jpg
---

