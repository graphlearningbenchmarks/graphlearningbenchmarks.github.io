---
title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
arxiv_id: '2509.15024'
source_url: ''
authors:
- name: Xuanting Xie
  orcid: null
  s2_author_id: '2197705751'
  s2_url: null
- name: Bingheng Li
  orcid: null
  s2_author_id: '2276175028'
  s2_url: null
- name: Erlin Pan
  orcid: null
  s2_author_id: '2134536588'
  s2_url: null
- name: Rui Hou
  orcid: null
  s2_author_id: '2265491781'
  s2_url: null
- name: Wenyu Chen
  orcid: null
  s2_author_id: '2290136174'
  s2_url: null
- name: Zhao Kang
  orcid: null
  s2_author_id: '2275599913'
  s2_url: null
published_date: Sep 18, 2025
published_date_iso: '2025-09-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Attention mechanisms have become a cornerstone in modern neural networks,
  driving breakthroughs across diverse domains. However, their application to graph-structured
  data, where capturing topological connections is essential, remains underexplored
  and underperforming compared to Graph Neural Networks (GNNs), particularly in the
  graph clustering task. GNN tends to overemphasize neighborhood aggregation, leading
  to a homogenization of node representations. Conversely, Transformer tends to over-globalize,
  highlighting distant nodes at the expense of meaningful local patterns. This dichotomy
  raises a key question: Is attention inherently redundant for unsupervised graph
  learning? To address this, we conduct a comprehensive empirical analysis, uncovering
  the complementary weaknesses of GNN and Transformer in graph clustering. Motivated
  by these insights, we propose the Attentive Graph Clustering Network (AGCN)—a novel
  architecture that reinterprets the notion that ``graph is attention''''. AGCN directly
  embeds the attention mechanism into the graph structure, enabling effective global
  information extraction while maintaining sensitivity to local topological cues.
  Our framework incorporates theoretical analysis to contrast AGCN behavior with GNN
  and Transformer and introduces two innovations: (1) a KV cache mechanism to improve
  computational efficiency, and (2) a pairwise margin contrastive loss to boost the
  discriminative capacity of the attention space. Extensive experimental results demonstrate
  that AGCN outperforms state-of-the-art methods.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AGCN
mrr: 0.0161
adjusted_mrr: 0.0107
mrr_dataset_count: 2
benchmark_categories:
- Heterophilic Graphs
- Heterophily Benchmark
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 1
  total: 5
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 1
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
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
  - model: DGCN
    model_key: dgcn
    model_plain: DGCN
    value: 0.6229
    std: null
    paper_value: 0.6229
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.779
    at_pub_std: 0.031
    at_pub_source_arxiv: '2312.04111'
    at_pub_source_title: Breaking the Entanglement of Homophily and Heterophily in
      Semi-supervised Node Classification
    at_pub_source_date_iso: '2023-12-07'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.15610000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.779
    true_std: 0.031
    value_gap_source_arxiv: '2312.04111'
    value_gap_source_title: Breaking the Entanglement of Homophily and Heterophily
      in Semi-supervised Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.15610000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.779
    sort_std: 0.031
    global_rank: 248
    paper_rank: 425
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Breaking the Entanglement of Homophily and Heterophily
      in Semi-supervised Node Classification
    comparison_source_arxiv: '2312.04111'
    is_best: false
    is_std_outlier: false
  - model: AGCN
    model_key: agcn
    model_plain: AGCN
    value: 0.6831
    std: null
    paper_value: 0.6831
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6831
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6831
    sort_std: null
    global_rank: 358
    paper_rank: 358
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMM
    model_key: gmm
    model_plain: GMM
    value: 0.5886
    std: null
    paper_value: 0.5886
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5886
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5886
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5886
    sort_std: null
    global_rank: 460
    paper_rank: 460
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RWR
    model_key: rwr
    model_plain: RWR
    value: 0.5829
    std: null
    paper_value: 0.5829
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5829
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5829
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5829
    sort_std: null
    global_rank: 471
    paper_rank: 471
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SELENE
    model_key: selene
    model_plain: SELENE
    value: 0.5796
    std: null
    paper_value: 0.5796
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5796
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5796
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5796
    sort_std: null
    global_rank: 478
    paper_rank: 478
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGSL
    model_key: rgsl
    model_plain: RGSL
    value: 0.5744
    std: null
    paper_value: 0.5744
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5744
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5744
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5744
    sort_std: null
    global_rank: 485
    paper_rank: 485
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.5623
    std: null
    paper_value: 0.5623
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5623
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5623
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5623
    sort_std: null
    global_rank: 501
    paper_rank: 501
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    value: 0.5132
    std: null
    paper_value: 0.5132
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5132
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5132
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5132
    sort_std: null
    global_rank: 549
    paper_rank: 549
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MSGA
    model_key: msga
    model_plain: MSGA
    value: 0.5077
    std: null
    paper_value: 0.5077
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5077
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5077
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5077
    sort_std: null
    global_rank: 558
    paper_rank: 558
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGC
    model_key: cgc
    model_plain: CGC
    value: 0.4462
    std: null
    paper_value: 0.4462
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4462
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4462
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4462
    sort_std: null
    global_rank: 606
    paper_rank: 606
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FGC
    model_key: fgc
    model_plain: FGC
    value: 0.441
    std: null
    paper_value: 0.441
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.441
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.441
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.441
    sort_std: null
    global_rank: 610
    paper_rank: 610
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
    value: 0.4256
    std: null
    paper_value: 0.4256
    paper_std: null
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
    protocol_note: Unsupervised graph clustering task on heterophilic dataset
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4256
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4256
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4256
    sort_std: null
    global_rank: 622
    paper_rank: 622
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
  - model: AGCN
    model_key: agcn
    model_plain: AGCN
    value: 0.894
    std: null
    paper_value: 0.894
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: null
    global_rank: 34
    paper_rank: 34
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
  - model: RGSL
    model_key: rgsl
    model_plain: RGSL
    value: 0.3457
    std: null
    paper_value: 0.3457
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3457
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3457
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3457
    sort_std: null
    global_rank: 213
    paper_rank: 213
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCN
    model_key: dgcn
    model_plain: DGCN
    value: 0.3342
    std: null
    paper_value: 0.3342
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3342
    at_pub_std: null
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3342
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3342
    sort_std: null
    global_rank: 215
    paper_rank: 215
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    value: 0.3257
    std: null
    paper_value: 0.3257
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3257
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3257
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3257
    sort_std: null
    global_rank: 216
    paper_rank: 216
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGC
    model_key: cgc
    model_plain: CGC
    value: 0.3016
    std: null
    paper_value: 0.3016
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3016
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3016
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3016
    sort_std: null
    global_rank: 220
    paper_rank: 220
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARVGA
    model_key: arvga
    model_plain: ARVGA
    value: 0.2289
    std: null
    paper_value: 0.2289
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2289
    at_pub_std: null
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2289
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2289
    sort_std: null
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
  - model: RWR
    model_key: rwr
    model_plain: RWR
    value: 0.2273
    std: null
    paper_value: 0.2273
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2273
    at_pub_std: null
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2273
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2273
    sort_std: null
    global_rank: 225
    paper_rank: 225
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMM
    model_key: gmm
    model_plain: GMM
    value: 0.219
    std: null
    paper_value: 0.219
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.219
    at_pub_std: null
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.219
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.219
    sort_std: null
    global_rank: 226
    paper_rank: 226
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
    value: 0.2123
    std: null
    paper_value: 0.2123
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2123
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2123
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2123
    sort_std: null
    global_rank: 228
    paper_rank: 228
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MSGA
    model_key: msga
    model_plain: MSGA
    value: 0.1931
    std: null
    paper_value: 0.1931
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1931
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1931
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1931
    sort_std: null
    global_rank: 230
    paper_rank: 230
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FGC
    model_key: fgc
    model_plain: FGC
    value: 0.1446
    std: null
    paper_value: 0.1446
    paper_std: null
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
    protocol_note: Clustering task on heterophilic graph
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1446
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1446
    true_std: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1446
    sort_std: null
    global_rank: 232
    paper_rank: 232
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
  dataset: UAT
  is_multi_metric: true
  rows:
  - model: AGCN
    model_key: agcn
    model_plain: AGCN
    metric_values:
    - null
    - 0.6084
    - 0.3074
    metric_stds:
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.6084
    sort_std: null
    true_value: 0.6084
    true_std: null
    paper_value: 0.6084
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: the idea
    model_key: the idea
    model_plain: the idea
    metric_values:
    - 0.584
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2507.20127'
    title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph Message-passing'
    published_venue: ''
    date: Jul 27, 2025
    date_display: Jul 2025
    date_iso: '2025-07-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.584
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: two unsupervised strategies
    model_key: two unsupervised strategies
    model_plain: two unsupervised strategies
    metric_values:
    - 0.5681
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.03666'
    title: Provable Filter for Real-world Graph Clustering
    published_venue: ''
    date: Mar 6, 2024
    date_display: Mar 2024
    date_iso: '2024-03-06'
    codebase_url: https://github.com/XieXuanting/PFGC
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.5681
    sort_std: 0.0034
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    metric_values:
    - null
    - 0.5658
    - 0.2807
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.5658
    sort_std: null
    true_value: 0.5658
    true_std: null
    paper_value: 0.5658
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5658
    at_pub_std: 0.0162
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: CCGC
    model_key: ccgc
    model_plain: CCGC
    metric_values:
    - null
    - 0.5634
    - 0.2815
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5634
    sort_std: null
    true_value: 0.5634
    true_std: null
    paper_value: 0.5634
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5634
    at_pub_std: 0.0111
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: FGC
    model_key: fgc
    model_plain: FGC
    metric_values:
    - null
    - 0.5303
    - 0.2706
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5303
    sort_std: null
    true_value: 0.5303
    true_std: null
    paper_value: 0.5303
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5303
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: DGCN
    model_key: dgcn
    model_plain: DGCN
    metric_values:
    - null
    - 0.5227
    - 0.2354
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5227
    sort_std: null
    true_value: 0.5227
    true_std: null
    paper_value: 0.5227
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5227
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    metric_values:
    - null
    - 0.5225
    - 0.2161
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5225
    sort_std: null
    true_value: 0.5225
    true_std: null
    paper_value: 0.5225
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5225
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  - model: DyFSS
    model_key: dyfss
    model_plain: DyFSS
    metric_values:
    - null
    - 0.5143
    - 0.2552
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5143
    sort_std: null
    true_value: 0.5143
    true_std: null
    paper_value: 0.5143
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.5143
    at_pub_std: null
    at_pub_source_arxiv: '2507.20127'
    at_pub_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    at_pub_source_date_iso: '2025-07-27'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: CGC
    model_key: cgc
    model_plain: CGC
    metric_values:
    - null
    - 0.4958
    - 0.1749
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4958
    sort_std: null
    true_value: 0.4958
    true_std: null
    paper_value: 0.4958
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.4958
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.4416
    - 0.2153
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4416
    sort_std: null
    true_value: 0.4416
    true_std: null
    paper_value: 0.4416
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.4416
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: MCGC
    model_key: mcgc
    model_plain: MCGC
    metric_values:
    - null
    - 0.4193
    - 0.1664
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4193
    sort_std: null
    true_value: 0.4193
    true_std: null
    paper_value: 0.4193
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.4193
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  - model: SSGC
    model_key: ssgc
    model_plain: SSGC
    metric_values:
    - null
    - 0.3674
    - 0.0804
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3674
    sort_std: null
    true_value: 0.3674
    true_std: null
    paper_value: 0.3674
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.3674
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    metric_values:
    - null
    - 0.3361
    - 0.2649
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3361
    sort_std: null
    true_value: 0.3361
    true_std: null
    paper_value: 0.3361
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2509.15024'
    value_gap_source_title: 'Attention Beyond Neighborhoods: Reviving Transformer
      for Graph Clustering'
    value_note: ''
    at_pub_value: 0.3361
    at_pub_std: null
    at_pub_source_arxiv: '2403.03666'
    at_pub_source_title: Provable Filter for Real-world Graph Clustering
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-09-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Sep 18, 2025
    date_display: Sep 2025
    date_iso: '2025-09-18'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  metrics:
  - F1
  - ACC
  - NMI
  primary_metric: F1
  rank_metric: ACC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - ACC
  - NMI
  metric: ACC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: Heterophily Benchmark
  datasets:
  - *id002
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Cornell
      dataset_slug: cornell
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: UAT
      dataset_slug: uat
single_proposed_model: AGCN
main_figure: /figures/2509.15024/main_figure.jpegoptim.jpg
---

