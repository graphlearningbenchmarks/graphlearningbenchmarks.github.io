---
title: 'Toward General Digraph Contrastive Learning: A Dual Spatial Perspective'
arxiv_id: '2510.16311'
source_url: ''
authors:
- name: Daohan Su
  orcid: null
  s2_author_id: '2271295428'
  s2_url: null
- name: Yang Zhang
  orcid: null
  s2_author_id: '2371136592'
  s2_url: null
- name: Xunkai Li
  orcid: null
  s2_author_id: '2268429288'
  s2_url: null
- name: Ronghua Li
  orcid: null
  s2_author_id: '2312235766'
  s2_url: null
- name: Guoren Wang
  orcid: null
  s2_author_id: '8349792'
  s2_url: null
published_date: Oct 18, 2025
published_date_iso: '2025-10-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Contrastive Learning (GCL) has emerged as a powerful tool for extracting
  consistent representations from graphs, independent of labeled information. However,
  existing methods predominantly focus on undirected graphs, disregarding the pivotal
  directional information that is fundamental and indispensable in real-world networks
  (e.g., social networks and recommendations). In this paper, we introduce S2-DiGCL,
  a novel framework that emphasizes spatial insights from complex and real domain
  perspectives for directed graph (digraph) contrastive learning. From the complex-domain
  perspective, S2-DiGCL introduces personalized perturbations into the magnetic Laplacian
  to adaptively modulate edge phases and directional semantics. From the real-domain
  perspective, it employs a path-based subgraph augmentation strategy to capture fine-grained
  local asymmetries and topological dependencies. By jointly leveraging these two
  complementary spatial views, S2-DiGCL constructs high-quality positive and negative
  samples, leading to more general and robust digraph contrastive learning. Extensive
  experiments on 7 real-world digraph datasets demonstrate the superiority of our
  approach, achieving SOTA performance with 4.41\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DiGCL
- S2-DiGCL
mrr: 0.0046
adjusted_mrr: 0.0031
mrr_dataset_count: 2
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Actor
  rows:
  - model: R-SoftGraphAIN
    model_key: nodeformer
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: diggr
    model_plain: R-SoftGraphAIN
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
    input_feature_source: null
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
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.432
    std: 0.012
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
    global_rank: 3
    sort_value: 0.432
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.312
    std: 0.0051
    paper_value: 0.312
    paper_std: 0.0051
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.369
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.056999999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.362
    true_std: 0.01
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.04999999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.362
    sort_std: 0.01
    global_rank: 184
    paper_rank: 339
    rank_delta: 155
    rank_delta_abs: 155
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.2941
    std: 0.0125
    paper_value: 0.2941
    paper_std: 0.0125
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3605
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.06640000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3605
    true_std: 0.0035
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.06640000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 191
    paper_rank: 376
    rank_delta: 185
    rank_delta_abs: 185
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: S2-DiGCL
    model_key: s2-digcl
    model_plain: S2-DiGCL
    value: 0.3571
    std: 0.0084
    paper_value: 0.3571
    paper_std: 0.0084
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3571
    true_std: 0.0084
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3571
    sort_std: 0.0084
    global_rank: 212
    paper_rank: 212
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RAW-GNN
    model_key: raw-gnn
    model_plain: RAW-GNN
    value: 0.3508
    std: 0.0053
    paper_value: 0.3508
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3508
    true_std: 0.0053
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3508
    sort_std: 0.0053
    global_rank: 251
    paper_rank: 251
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiGCL
    model_key: digcl
    model_plain: DiGCL
    value: 0.3453
    std: 0.0042
    paper_value: 0.3453
    paper_std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3453
    true_std: 0.0042
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3453
    sort_std: 0.0042
    global_rank: 268
    paper_rank: 268
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
    value: 0.3072
    std: 0.0063
    paper_value: 0.3072
    paper_std: 0.0063
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.345
    at_pub_std: 0.011
    at_pub_source_arxiv: '2303.06344'
    at_pub_source_title: Graph Contrastive Learning under Heterophily via Graph Filters
    at_pub_source_date_iso: '2023-03-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0378
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.345
    true_std: 0.011
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.0378
    has_value_note: false
    value_note: ''
    sort_value: 0.345
    sort_std: 0.011
    global_rank: 269
    paper_rank: 347
    rank_delta: 78
    rank_delta_abs: 78
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    comparison_source_arxiv: '2303.06344'
    is_best: false
    is_std_outlier: false
  - model: DiGCN
    model_key: digcn
    model_plain: DiGCN
    value: 0.3391
    std: 0.0102
    paper_value: 0.3391
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3391
    true_std: 0.0102
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3391
    sort_std: 0.0102
    global_rank: 290
    paper_rank: 290
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UGCL
    model_key: ugcl
    model_plain: UGCL
    value: 0.3363
    std: 0.007
    paper_value: 0.3363
    paper_std: 0.007
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3363
    true_std: 0.007
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3363
    sort_std: 0.007
    global_rank: 295
    paper_rank: 295
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
    value: 0.3067
    std: 0.0063
    paper_value: 0.3067
    paper_std: 0.0063
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2982
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.008499999999999952
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3209
    true_std: 0.0118
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.014200000000000046
    has_value_note: false
    value_note: ''
    sort_value: 0.3209
    sort_std: 0.0118
    global_rank: 319
    paper_rank: 348
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.3151
    std: 0.0154
    paper_value: 0.3151
    paper_std: 0.0154
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2864
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2308.10077'
    at_pub_source_title: Contrastive Learning for Non-Local Graphs with Multi-Resolution
      Structural Views
    at_pub_source_date_iso: '2023-08-19'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.028700000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3151
    true_std: 0.0154
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3151
    sort_std: 0.0154
    global_rank: 330
    paper_rank: 330
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Contrastive Learning for Non-Local Graphs with Multi-Resolution
      Structural Views
    comparison_source_arxiv: '2308.10077'
    is_best: false
    is_std_outlier: false
  - model: MagNet
    model_key: magnet
    model_plain: MagNet
    value: 0.3126
    std: 0.0067
    paper_value: 0.3126
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3126
    true_std: 0.0067
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3126
    sort_std: 0.0067
    global_rank: 337
    paper_rank: 337
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.2939
    std: 0.0097
    paper_value: 0.2939
    paper_std: 0.0097
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
    protocol_note: Node classification on standard split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2965
    at_pub_std: 0.0147
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.002599999999999991
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.2965
    true_std: 0.0147
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.002599999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.2965
    sort_std: 0.0147
    global_rank: 375
    paper_rank: 376
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
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
- &id001
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7756
    std: 0.0029
    paper_value: 0.7756
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9302
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15460000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.15460000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 141
    rank_delta: 140
    rank_delta_abs: 140
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rse + rgcn (70b)
    model_plain: GPM
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPM
    model_key: rse + sehgnn (70b)
    model_plain: GPM
    value: 0.8796
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 3
    sort_value: 0.8796
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.77
    std: 0.0083
    paper_value: 0.77
    paper_std: 0.0083
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8533
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2024-05-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08329999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8279
    true_std: 0.0016
    value_gap_source_arxiv: '2405.18581'
    value_gap_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.05789999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8279
    sort_std: 0.0016
    global_rank: 23
    paper_rank: 155
    rank_delta: 132
    rank_delta_abs: 132
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7049
    std: 0.0313
    paper_value: 0.7049
    paper_std: 0.0313
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8014
    at_pub_std: 0.48
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2025-06-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.09650000000000003
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8014
    true_std: 0.0048
    value_gap_source_arxiv: '2506.20362'
    value_gap_source_title: Self-Supervised Graph Learning via Spectral Bootstrapping
      and Laplacian-Based Augmentations
    value_gap_source_is_current_paper: false
    value_gap: 0.09650000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0048
    global_rank: 55
    paper_rank: 210
    rank_delta: 155
    rank_delta_abs: 155
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S2-DiGCL
    model_key: s2-digcl
    model_plain: S2-DiGCL
    value: 0.7842
    std: 0.0113
    paper_value: 0.7842
    paper_std: 0.0113
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7842
    true_std: 0.0113
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7842
    sort_std: 0.0113
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.7282
    std: 0.019
    paper_value: 0.7282
    paper_std: 0.019
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.784
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05580000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.784
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.05580000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.001
    global_rank: 114
    paper_rank: 193
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7837
    std: 0.0077
    paper_value: 0.7837
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.773
    at_pub_std: 0.008
    at_pub_source_arxiv: '2412.21151'
    at_pub_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    at_pub_source_date_iso: '2024-12-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.010699999999999932
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7837
    true_std: 0.0077
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7837
    sort_std: 0.0077
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7419
    std: 0.029
    paper_value: 0.7419
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7865
    at_pub_std: 0.069
    at_pub_source_arxiv: '2507.19526'
    at_pub_source_title: Quantizing Text-attributed Graphs for Semantic-Structural
      Integration
    at_pub_source_date_iso: '2025-07-20'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.04459999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7825
    true_std: 0.0056
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.04059999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7825
    sort_std: 0.0056
    global_rank: 120
    paper_rank: 188
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RAW-GNN
    model_key: raw-gnn
    model_plain: RAW-GNN
    value: 0.7509
    std: 0.0026
    paper_value: 0.7509
    paper_std: 0.0026
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7801
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2501.18739'
    at_pub_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    at_pub_source_date_iso: '2025-01-30'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-01-30'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.029200000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7801
    true_std: 0.0058
    value_gap_source_arxiv: '2501.18739'
    value_gap_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    value_gap_source_is_current_paper: false
    value_gap: 0.029200000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7801
    sort_std: 0.0058
    global_rank: 127
    paper_rank: 179
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    comparison_source_arxiv: '2501.18739'
    is_best: false
    is_std_outlier: false
  - model: DiGCN
    model_key: digcn
    model_plain: DiGCN
    value: 0.7763
    std: 0.0046
    paper_value: 0.7763
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7973
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2401.11772'
    at_pub_source_title: 'LightDiC: A Simple yet Effective Approach for Large-scale
      Digraph Representation Learning'
    at_pub_source_date_iso: '2024-01-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02100000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7763
    true_std: 0.0046
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7763
    sort_std: 0.0046
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LightDiC: A Simple yet Effective Approach for Large-scale
      Digraph Representation Learning'
    comparison_source_arxiv: '2401.11772'
    is_best: false
    is_std_outlier: false
  - model: MagNet
    model_key: magnet
    model_plain: MagNet
    value: 0.7674
    std: 0.007
    paper_value: 0.7674
    paper_std: 0.007
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7959
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2401.11772'
    at_pub_source_title: 'LightDiC: A Simple yet Effective Approach for Large-scale
      Digraph Representation Learning'
    at_pub_source_date_iso: '2024-01-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02850000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7674
    true_std: 0.007
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7674
    sort_std: 0.007
    global_rank: 160
    paper_rank: 160
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LightDiC: A Simple yet Effective Approach for Large-scale
      Digraph Representation Learning'
    comparison_source_arxiv: '2401.11772'
    is_best: false
    is_std_outlier: false
  - model: UGCL
    model_key: ugcl
    model_plain: UGCL
    value: 0.7543
    std: 0.0315
    paper_value: 0.7543
    paper_std: 0.0315
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7543
    true_std: 0.0315
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7543
    sort_std: 0.0315
    global_rank: 175
    paper_rank: 175
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiGCL
    model_key: digcl
    model_plain: DiGCL
    value: 0.7483
    std: 0.0288
    paper_value: 0.7483
    paper_std: 0.0288
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Node classification on standard WikiCS split
    date: Oct 18, 2025
    date_display: Oct 2025
    date_iso: '2025-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7483
    true_std: 0.0288
    value_gap_source_arxiv: '2510.16311'
    value_gap_source_title: 'Toward General Digraph Contrastive Learning: A Dual Spatial
      Perspective'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7483
    sort_std: 0.0288
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
main_figure: /figures/2510.16311/main_figure.jpegoptim.jpg
---

