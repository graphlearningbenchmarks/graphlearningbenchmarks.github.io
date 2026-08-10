---
title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
arxiv_id: '2204.04874'
source_url: ''
authors:
- name: Haonan Wang
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jieyu Zhang
  orcid: null
  s2_author_id: '47540245'
  s2_url: null
- name: Qi Zhu
  orcid: null
  s2_author_id: '144400492'
  s2_url: null
- name: Wei Huang
  orcid: null
  s2_author_id: '2314536603'
  s2_url: null
published_date: Apr 11, 2022
published_date_iso: '2022-04-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph contrastive learning (GCL) is the most representative and prevalent
  self-supervised learning approach for graph-structured data. Despite its remarkable
  success, existing GCL methods highly rely on an augmentation scheme to learn the
  representations invariant across different augmentation views. In this work, we
  revisit such a convention in GCL through examining the effect of augmentation techniques
  on graph data via the lens of spectral theory. We found that graph augmentations
  preserve the low-frequency components and perturb the middle- and high-frequency
  components of the graph, which contributes to the success of GCL algorithms on homophilic
  graphs but hinder its application on heterophilic graphs, due to the high-frequency
  preference of heterophilic data. Motivated by this, we propose a novel, theoretically-principled,
  and augmentation-free GCL method, named AF-GCL, that (1) leverages the features
  aggregated by Graph Neural Network to construct the self-supervision signal instead
  of augmentations and therefore (2) is less sensitive to the graph homophily degree.
  Theoretically, We present the performance guarantee for AF-GCL\ as well as an analysis
  for understanding the efficacy of AF-GCL. Extensive experiments on 14 benchmark
  datasets with varying degrees of heterophily show that AF-GCL\ presents competitive
  or better performance on homophilic graphs and outperforms all existing state-of-the-art
  GCL methods on heterophilic graphs with significantly less computational overhead.
codebase_url: ''
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- AF-GCL
mrr: 0.0081
adjusted_mrr: 0.0081
mrr_dataset_count: 8
benchmark_categories:
- Classic
- Heterophilic Graphs
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 6
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id005
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
    value: 0.3593
    std: 0.0061
    paper_value: 0.3593
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4018
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-02-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04249999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4026
    true_std: 0.0108
    value_gap_source_arxiv: '2302.03228'
    value_gap_source_title: Heterophily-Aware Graph Attention Network
    value_gap_source_is_current_paper: false
    value_gap: 0.043300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.4026
    sort_std: 0.0108
    global_rank: 55
    paper_rank: 227
    rank_delta: 172
    rank_delta_abs: 172
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2879
    std: 0.0023
    paper_value: 0.2879
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.369
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.0811
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.369
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0811
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 166
    paper_rank: 437
    rank_delta: 271
    rank_delta_abs: 271
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3209
    std: 0.0107
    paper_value: 0.3209
    paper_std: 0.0107
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3464
    true_std: 0.002
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.025499999999999967
    has_value_note: false
    value_note: ''
    sort_value: 0.3464
    sort_std: 0.002
    global_rank: 294
    paper_rank: 352
    rank_delta: 58
    rank_delta_abs: 58
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
    value: 0.2827
    std: 0.0043
    paper_value: 0.2827
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.062299999999999967
    has_value_note: false
    value_note: ''
    sort_value: 0.345
    sort_std: 0.011
    global_rank: 298
    paper_rank: 451
    rank_delta: 153
    rank_delta_abs: 153
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
    value: 0.283
    std: 0.0076
    paper_value: 0.283
    paper_std: 0.0076
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.272
    at_pub_std: null
    at_pub_source_arxiv: '2201.12843'
    at_pub_source_title: Graph Representation Learning via Aggregation Enhancement
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.010999999999999954
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3209
    true_std: 0.0118
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.037900000000000045
    has_value_note: false
    value_note: ''
    sort_value: 0.3209
    sort_std: 0.0118
    global_rank: 353
    paper_rank: 450
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Representation Learning via Aggregation Enhancement
    comparison_source_arxiv: '2201.12843'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.2843
    std: 0.0057
    paper_value: 0.2843
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3157
    true_std: 0.0075
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.031399999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.3157
    sort_std: 0.0075
    global_rank: 363
    paper_rank: 445
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.2728
    std: 0.0087
    paper_value: 0.2728
    paper_std: 0.0087
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2618
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3011
    true_std: 0.0192
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.028299999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.3011
    sort_std: 0.0192
    global_rank: 405
    paper_rank: 467
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.288
    std: 0.0054
    paper_value: 0.288
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.2986
    true_std: 0.0075
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.010599999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.2986
    sort_std: 0.0075
    global_rank: 413
    paper_rank: 436
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.2889
    std: 0.005
    paper_value: 0.2889
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
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
    value_gap: 0.007599999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.2965
    sort_std: 0.0147
    global_rank: 418
    paper_rank: 435
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.2894
    std: 0.0069
    paper_value: 0.2894
    paper_std: 0.0069
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-20'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2894
    true_std: 0.0069
    value_gap_source_arxiv: '2310.13845'
    value_gap_source_title: Spectral-Aware Augmentation for Enhanced Graph Representation
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2894
    sort_std: 0.0069
    global_rank: 435
    paper_rank: 435
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
    value: 0.2536
    std: 0.0023
    paper_value: 0.2536
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2345
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.019100000000000006
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2863
    true_std: 0.0105
    value_gap_source_arxiv: '2308.10077'
    value_gap_source_title: Contrastive Learning for Non-Local Graphs with Multi-Resolution
      Structural Views
    value_gap_source_is_current_paper: false
    value_gap: 0.03270000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2863
    sort_std: 0.0105
    global_rank: 443
    paper_rank: 487
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.2704
    std: 0.0056
    paper_value: 0.2704
    paper_std: 0.0056
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2704
    true_std: 0.0056
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2704
    sort_std: 0.0056
    global_rank: 469
    paper_rank: 469
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.255
    std: 0.0028
    paper_value: 0.255
    paper_std: 0.0028
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using the standard Pei et al. split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.255
    true_std: 0.0028
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.255
    sort_std: 0.0028
    global_rank: 481
    paper_rank: 481
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
- &id006
  dataset: Chameleon
  rows:
  - model: Hetero-S (GAT 8-layer)
    model_key: hetero-s (gat 8-layer)
    model_plain: Hetero-S (GAT 8-layer)
    value: 0.8693
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8693
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.8586
    std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8586
    sort_std: 0.018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.856
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.856
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.5381
    std: 0.0109
    paper_value: 0.5381
    paper_std: 0.0109
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7319
    true_std: 0.0042
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.19379999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7319
    sort_std: 0.0042
    global_rank: 41
    paper_rank: 211
    rank_delta: 170
    rank_delta_abs: 170
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6645
    std: 0.0048
    paper_value: 0.6645
    paper_std: 0.0048
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.676
    at_pub_std: 0.024
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.011500000000000066
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7033
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03880000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7033
    sort_std: null
    global_rank: 69
    paper_rank: 107
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.6094
    std: 0.0081
    paper_value: 0.6094
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
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
    true_value: 0.6554
    true_std: 0.011
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04599999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.6554
    sort_std: 0.011
    global_rank: 110
    paper_rank: 154
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.6528
    std: 0.0053
    paper_value: 0.6528
    paper_std: 0.0053
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
    input_feature_source: raw_features
    feature_source_evidence: AF-GCL constructs positive/negative pairs based on the
      aggregated node features and directly optimizes the distance of representations
      in high-dimensional space.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-20'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6528
    true_std: 0.0053
    value_gap_source_arxiv: '2310.13845'
    value_gap_source_title: Spectral-Aware Augmentation for Enhanced Graph Representation
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6528
    sort_std: 0.0053
    global_rank: 117
    paper_rank: 117
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
    value: 0.6486
    std: 0.0063
    paper_value: 0.6486
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6486
    true_std: 0.0063
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6486
    sort_std: 0.0063
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.634
    std: 0.03
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 136
    sort_value: 0.634
    sort_std: 0.03
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.4265
    std: 0.0127
    paper_value: 0.4265
    paper_std: 0.0127
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6232
    true_std: 0.019
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.19669999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6232
    sort_std: 0.019
    global_rank: 144
    paper_rank: 288
    rank_delta: 144
    rank_delta_abs: 144
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
    value: 0.6124
    std: 0.0053
    paper_value: 0.6124
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6124
    true_std: 0.0053
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6124
    sort_std: 0.0053
    global_rank: 149
    paper_rank: 149
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
    value: 0.6027
    std: 0.007
    paper_value: 0.6027
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6027
    true_std: 0.007
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6027
    sort_std: 0.007
    global_rank: 165
    paper_rank: 165
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
    value: 0.4759
    std: 0.0073
    paper_value: 0.4759
    paper_std: 0.0073
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.482
    at_pub_std: 0.0263
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5429
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06700000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.5429
    sort_std: null
    global_rank: 208
    paper_rank: 258
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.5281
    std: 0.0063
    paper_value: 0.5281
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5281
    true_std: 0.0063
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5281
    sort_std: 0.0063
    global_rank: 214
    paper_rank: 214
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.4399
    std: 0.0067
    paper_value: 0.4399
    paper_std: 0.0067
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4774
    true_std: 0.0205
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.03749999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4774
    sort_std: 0.0205
    global_rank: 256
    paper_rank: 275
    rank_delta: 19
    rank_delta_abs: 19
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
    value: 0.3913
    std: 0.0134
    paper_value: 0.3913
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3913
    true_std: 0.0134
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3913
    sort_std: 0.0134
    global_rank: 308
    paper_rank: 308
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.3149
    std: 0.0117
    paper_value: 0.3149
    paper_std: 0.0117
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the standard Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3149
    true_std: 0.0117
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3149
    sort_std: 0.0117
    global_rank: 321
    paper_rank: 321
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
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8774
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
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7073
    std: 0.0065
    paper_value: 0.7073
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.08699999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.16959999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 638
    rank_delta: 617
    rank_delta_abs: 617
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7183
    std: 0.0054
    paper_value: 0.7183
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7882
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06989999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.789
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.07069999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.002
    global_rank: 83
    paper_rank: 533
    rank_delta: 450
    rank_delta_abs: 450
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.7172
    std: 0.0015
    paper_value: 0.7172
    paper_std: 0.0015
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7869
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0697000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7869
    true_std: 0.0016
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.0697000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7869
    sort_std: 0.0016
    global_rank: 90
    paper_rank: 538
    rank_delta: 448
    rank_delta_abs: 448
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7328
    std: 0.0048
    paper_value: 0.7328
    paper_std: 0.0048
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7808
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04800000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7808
    true_std: 0.0006
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.04800000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0006
    global_rank: 108
    paper_rank: 346
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7182
    std: 0.0048
    paper_value: 0.7182
    paper_std: 0.0048
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.04180000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.002
    global_rank: 171
    paper_rank: 533
    rank_delta: 362
    rank_delta_abs: 362
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.7133
    std: 0.0037
    paper_value: 0.7133
    paper_std: 0.0037
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6752
    at_pub_std: 0.013
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03810000000000002
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7523
    true_std: 0.0119
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.038999999999999924
    has_value_note: false
    value_note: ''
    sort_value: 0.7523
    sort_std: 0.0119
    global_rank: 211
    paper_rank: 587
    rank_delta: 376
    rank_delta_abs: 376
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7121
    std: 0.0064
    paper_value: 0.7121
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.717
    at_pub_std: 0.006
    at_pub_source_arxiv: '2009.07111'
    at_pub_source_title: Contrastive and Generative Graph Convolutional Networks for
      Graph-based Semi-Supervised Learning
    at_pub_source_date_iso: '2020-09-15'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0049000000000000155
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.03290000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 598
    rank_delta: 353
    rank_delta_abs: 353
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4931
    std: 0.0026
    paper_value: 0.4931
    paper_std: 0.0026
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6958
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.2027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7289
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.2358
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 951
    rank_delta: 550
    rank_delta_abs: 550
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.7196
    std: 0.0042
    paper_value: 0.7196
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7196
    true_std: 0.0042
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7196
    sort_std: 0.0042
    global_rank: 520
    paper_rank: 520
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.6741
    std: 0.0024
    paper_value: 0.6741
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.699
    true_std: 0.0057
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.024899999999999922
    has_value_note: false
    value_note: ''
    sort_value: 0.699
    sort_std: 0.0057
    global_rank: 689
    paper_rank: 770
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.5139
    std: 0.0041
    paper_value: 0.5139
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6024
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08850000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6785
    true_std: 0.0079
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.16459999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6785
    sort_std: 0.0079
    global_rank: 759
    paper_rank: 945
    rank_delta: 186
    rank_delta_abs: 186
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6583
    std: 0.004
    paper_value: 0.6583
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6575
    at_pub_std: 0.003
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0008000000000000229
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6639
    true_std: 0.0024
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.005600000000000049
    has_value_note: false
    value_note: ''
    sort_value: 0.6639
    sort_std: 0.0024
    global_rank: 806
    paper_rank: 823
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4734
    std: 0.0084
    paper_value: 0.4734
    paper_std: 0.0084
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using Planetoid fixed split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6552
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.18180000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6552
    true_std: 0.0018
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.18180000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6552
    sort_std: 0.0018
    global_rank: 832
    paper_rank: 954
    rank_delta: 122
    rank_delta_abs: 122
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
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
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8154
    std: 0.0068
    paper_value: 0.8154
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8728
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05740000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 656
    rank_delta: 625
    rank_delta_abs: 625
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
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
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8144
    std: 0.0072
    paper_value: 0.8144
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.058599999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 170
    paper_rank: 662
    rank_delta: 492
    rank_delta_abs: 492
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
    value: 0.8192
    std: 0.0089
    paper_value: 0.8192
    paper_std: 0.0089
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.821
    at_pub_std: 0.016
    at_pub_source_arxiv: '2012.07437'
    at_pub_source_title: Rethinking the Promotion Brought by Contrastive Learning
      to Semi-Supervised Node Classification
    at_pub_source_date_iso: '2020-12-14'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0017999999999999128
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.872
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.05279999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.002
    global_rank: 176
    paper_rank: 618
    rank_delta: 442
    rank_delta_abs: 442
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
    value: 0.8345
    std: 0.0068
    paper_value: 0.8345
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8538
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.019299999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.868
    true_std: 0.005
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.033499999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.005
    global_rank: 205
    paper_rank: 450
    rank_delta: 245
    rank_delta_abs: 245
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
    value: 0.8234
    std: 0.0071
    paper_value: 0.8234
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8508
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.02739999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.863
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.03959999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.002
    global_rank: 227
    paper_rank: 565
    rank_delta: 338
    rank_delta_abs: 338
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.8239
    std: 0.0065
    paper_value: 0.8239
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8526
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02870000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8526
    true_std: 0.0008
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.02870000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8526
    sort_std: 0.0008
    global_rank: 276
    paper_rank: 561
    rank_delta: 285
    rank_delta_abs: 285
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.8207
    std: 0.001
    paper_value: 0.8207
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7822
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03849999999999998
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8409
    true_std: 0.0085
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.020199999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.0085
    global_rank: 363
    paper_rank: 604
    rank_delta: 241
    rank_delta_abs: 241
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.7731
    std: 0.0102
    paper_value: 0.7731
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.836
    true_std: 0.0052
    value_gap_source_arxiv: '2405.14742'
    value_gap_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06289999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0052
    global_rank: 418
    paper_rank: 815
    rank_delta: 397
    rank_delta_abs: 397
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.8316
    std: 0.0013
    paper_value: 0.8316
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8316
    true_std: 0.0013
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8316
    sort_std: 0.0013
    global_rank: 489
    paper_rank: 489
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.7072
    std: 0.0063
    paper_value: 0.7072
    paper_std: 0.0063
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.829
    at_pub_std: null
    at_pub_source_arxiv: '1909.00958'
    at_pub_source_title: 'Graph Representation Learning: A Survey'
    at_pub_source_date_iso: '2019-09-03'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.12179999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.829
    true_std: null
    value_gap_source_arxiv: '1909.00958'
    value_gap_source_title: 'Graph Representation Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.12179999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: null
    global_rank: 508
    paper_rank: 900
    rank_delta: 392
    rank_delta_abs: 392
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Representation Learning: A Survey'
    comparison_source_arxiv: '1909.00958'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.7149
    std: 0.0041
    paper_value: 0.7149
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8011
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08620000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8011
    true_std: 0.0022
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.08620000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8011
    sort_std: 0.0022
    global_rank: 736
    paper_rank: 895
    rank_delta: 159
    rank_delta_abs: 159
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4792
    std: 0.0041
    paper_value: 0.4792
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7414
    at_pub_std: 0.014
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.26219999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.29760000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 996
    rank_delta: 190
    rank_delta_abs: 190
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.7108
    std: 0.0091
    paper_value: 0.7108
    paper_std: 0.0091
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cora using Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7108
    true_std: 0.0091
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7108
    sort_std: 0.0091
    global_rank: 897
    paper_rank: 897
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
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
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
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
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
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
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
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7916
    std: 0.0025
    paper_value: 0.7916
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10540000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: 0.0015
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.138
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 625
    rank_delta: 606
    rank_delta_abs: 606
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8881
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 134
    sort_value: 0.8881
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8018
    std: 0.0063
    paper_value: 0.8018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.883
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08120000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.883
    sort_std: 0.001
    global_rank: 167
    paper_rank: 487
    rank_delta: 320
    rank_delta_abs: 320
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
    value: 0.8054
    std: 0.0036
    paper_value: 0.8054
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.795
    at_pub_std: 0.011
    at_pub_source_arxiv: '2009.07111'
    at_pub_source_title: Contrastive and Generative Graph Convolutional Networks for
      Graph-based Semi-Supervised Learning
    at_pub_source_date_iso: '2020-09-15'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.010399999999999965
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.0676
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 224
    paper_rank: 452
    rank_delta: 228
    rank_delta_abs: 228
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.7934
    std: 0.0104
    paper_value: 0.7934
    paper_std: 0.0104
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8726
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07920000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8726
    true_std: 0.0016
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.07920000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8726
    sort_std: 0.0016
    global_rank: 225
    paper_rank: 594
    rank_delta: 369
    rank_delta_abs: 369
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.8009
    std: 0.0062
    paper_value: 0.8009
    paper_std: 0.0062
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8725
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07160000000000011
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
    value_gap: 0.07160000000000011
    has_value_note: false
    value_note: ''
    sort_value: 0.8725
    sort_std: 0.0012
    global_rank: 226
    paper_rank: 496
    rank_delta: 270
    rank_delta_abs: 270
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
    value: 0.7678
    std: 0.0031
    paper_value: 0.7678
    paper_std: 0.0031
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8703
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10249999999999992
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
    value_gap: 0.10299999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8708
    sort_std: 0.0017
    global_rank: 235
    paper_rank: 821
    rank_delta: 586
    rank_delta_abs: 586
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6914
    std: 0.0034
    paper_value: 0.6914
    paper_std: 0.0034
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8638
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.1724
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
    value_gap: 0.17759999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 929
    rank_delta: 686
    rank_delta_abs: 686
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.7327
    std: 0.0086
    paper_value: 0.7327
    paper_std: 0.0086
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8652
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.13249999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8652
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.13249999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8652
    sort_std: 0.0012
    global_rank: 255
    paper_rank: 897
    rank_delta: 642
    rank_delta_abs: 642
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.8021
    std: 0.0039
    paper_value: 0.8021
    paper_std: 0.0039
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8128
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.010699999999999932
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8512
    true_std: 0.0023
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.04909999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8512
    sort_std: 0.0023
    global_rank: 291
    paper_rank: 479
    rank_delta: 188
    rank_delta_abs: 188
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
    value: 0.7585
    std: 0.0062
    paper_value: 0.7585
    paper_std: 0.0062
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.07220000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8307
    sort_std: 0.0029
    global_rank: 342
    paper_rank: 850
    rank_delta: 508
    rank_delta_abs: 508
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
    value: 0.7223
    std: 0.0071
    paper_value: 0.7223
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.775
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05269999999999997
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
    value_gap: 0.10709999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8294
    sort_std: 0.0031
    global_rank: 347
    paper_rank: 905
    rank_delta: 558
    rank_delta_abs: 558
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.7905
    std: 0.0075
    paper_value: 0.7905
    paper_std: 0.0075
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
    input_feature_source: raw_features
    feature_source_evidence: AF-GCL constructs positive/negative pairs based on the
      aggregated node features and directly optimizes the distance of representations
      in high-dimensional space.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.815
    true_std: 0.007
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.024499999999999966
    has_value_note: false
    value_note: ''
    sort_value: 0.815
    sort_std: 0.007
    global_rank: 393
    paper_rank: 639
    rank_delta: 246
    rank_delta_abs: 246
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.6623
    std: 0.0095
    paper_value: 0.6623
    paper_std: 0.0095
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on PubMed using Planetoid split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6623
    true_std: 0.0095
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6623
    sort_std: 0.0095
    global_rank: 945
    paper_rank: 945
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
- &id007
  dataset: Squirrel
  rows:
  - model: IBG-NN
    model_key: ibg-nn
    model_plain: IBG-NN
    value: 0.7763
    std: 0.0179
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_display: Apr 2025
    date_iso: '2025-04-25'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7763
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.7747
    std: 0.0128
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7747
    sort_std: 0.0128
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DHGNN
    model_key: dhgnn
    model_plain: DHGNN
    value: 0.7684
    std: 0.0161
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7684
    sort_std: 0.0161
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5303
    std: 0.0057
    paper_value: 0.5303
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.549
    at_pub_std: 0.019
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.01870000000000005
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6067
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07640000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6067
    sort_std: null
    global_rank: 51
    paper_rank: 92
    rank_delta: 41
    rank_delta_abs: 41
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
    value: 0.3875
    std: 0.0132
    paper_value: 0.3875
    paper_std: 0.0132
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6009
    true_std: 0.0044
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.21339999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6009
    sort_std: 0.0044
    global_rank: 55
    paper_rank: 199
    rank_delta: 144
    rank_delta_abs: 144
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.521
    std: 0.0067
    paper_value: 0.521
    paper_std: 0.0067
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
    input_feature_source: raw_features
    feature_source_evidence: AF-GCL constructs positive/negative pairs based on the
      aggregated node features and directly optimizes the distance of representations
      in high-dimensional space.
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-20'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.521
    true_std: 0.0067
    value_gap_source_arxiv: '2310.13845'
    value_gap_source_title: Spectral-Aware Augmentation for Enhanced Graph Representation
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.521
    sort_std: 0.0067
    global_rank: 98
    paper_rank: 98
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
    value: 0.4153
    std: 0.0109
    paper_value: 0.4153
    paper_std: 0.0109
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4809
    true_std: 0.0021
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.06559999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.4809
    sort_std: 0.0021
    global_rank: 112
    paper_rank: 171
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.4624
    std: 0.007
    paper_value: 0.4624
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4624
    true_std: 0.007
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4624
    sort_std: 0.007
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.446
    std: 0.013
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 137
    sort_value: 0.446
    sort_std: 0.013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.4109
    std: 0.0085
    paper_value: 0.4109
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
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
    true_value: 0.4268
    true_std: 0.011
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.015900000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.4268
    sort_std: 0.011
    global_rank: 157
    paper_rank: 174
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
    value: 0.3511
    std: 0.0092
    paper_value: 0.3511
    paper_std: 0.0092
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.425
    true_std: 0.0135
    value_gap_source_arxiv: '2604.15699'
    value_gap_source_title: Frequency-Corrupt Based Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.07389999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.425
    sort_std: 0.0135
    global_rank: 161
    paper_rank: 248
    rank_delta: 87
    rank_delta_abs: 87
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
    value: 0.4222
    std: 0.0063
    paper_value: 0.4222
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4222
    true_std: 0.0063
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4222
    sort_std: 0.0063
    global_rank: 164
    paper_rank: 164
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
    value: 0.3167
    std: 0.0061
    paper_value: 0.3167
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3335
    at_pub_std: 0.0124
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.016800000000000037
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.393
    true_std: 0.0079
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07630000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.393
    sort_std: 0.0079
    global_rank: 194
    paper_rank: 273
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.309
    std: 0.0109
    paper_value: 0.309
    paper_std: 0.0109
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3754
    true_std: 0.0219
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.06640000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3754
    sort_std: 0.0219
    global_rank: 217
    paper_rank: 278
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.3525
    std: 0.0121
    paper_value: 0.3525
    paper_std: 0.0121
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3525
    true_std: 0.0121
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3525
    sort_std: 0.0121
    global_rank: 247
    paper_rank: 247
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
    value: 0.3465
    std: 0.0081
    paper_value: 0.3465
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3465
    true_std: 0.0081
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3465
    sort_std: 0.0081
    global_rank: 256
    paper_rank: 256
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.2764
    std: 0.0136
    paper_value: 0.2764
    paper_std: 0.0136
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel using Geom-GCN 10 fixed splits.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2764
    true_std: 0.0136
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2764
    sort_std: 0.0136
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
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9302
    std: 0.0011
    paper_value: 0.9302
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.772
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1582
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
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
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8771
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
    global_rank: 9
    sort_value: 0.8771
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7819
    std: 0.001
    paper_value: 0.7819
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8014
    at_pub_std: 0.48
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.019499999999999962
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8014
    true_std: 0.0048
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.019499999999999962
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0048
    global_rank: 94
    paper_rank: 172
    rank_delta: 78
    rank_delta_abs: 78
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7696
    std: 0.0061
    paper_value: 0.7696
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.030400000000000094
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: 0.001
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.030400000000000094
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.001
    global_rank: 100
    paper_rank: 208
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.7901
    std: 0.0051
    paper_value: 0.7901
    paper_std: 0.0051
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7901
    true_std: 0.0051
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7901
    sort_std: 0.0051
    global_rank: 134
    paper_rank: 134
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
    value: 0.7537
    std: 0.0013
    paper_value: 0.7537
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.754
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-07-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7865
    true_std: 0.069
    value_gap_source_arxiv: '2507.19526'
    value_gap_source_title: Quantizing Text-attributed Graphs for Semantic-Structural
      Integration
    value_gap_source_is_current_paper: false
    value_gap: 0.03279999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7865
    sort_std: 0.069
    global_rank: 152
    paper_rank: 230
    rank_delta: 78
    rank_delta_abs: 78
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.784
    std: 0.0013
    paper_value: 0.784
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.784
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
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
    true_value: 0.784
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.001
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.7397
    std: 0.0016
    paper_value: 0.7397
    paper_std: 0.0016
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.702
    at_pub_std: 0.0
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03770000000000007
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.038999999999999924
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 181
    paper_rank: 243
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.7556
    std: 0.0028
    paper_value: 0.7556
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7563
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0006999999999999229
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0230999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 180
    paper_rank: 226
    rank_delta: 46
    rank_delta_abs: 46
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
    value: 0.7751
    std: 0.0006
    paper_value: 0.7751
    paper_std: 0.0006
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7752
    at_pub_std: 0.08
    at_pub_source_arxiv: '2106.02466'
    at_pub_source_title: 'Graph Barlow Twins: A self-supervised representation learning
      framework for graphs'
    at_pub_source_date_iso: '2021-06-04'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7757
    true_std: 0.0046
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0005999999999999339
    has_value_note: false
    value_note: ''
    sort_value: 0.7757
    sort_std: 0.0046
    global_rank: 190
    paper_rank: 193
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.7442
    std: 0.0013
    paper_value: 0.7442
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7721
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.027900000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7721
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.027900000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: null
    global_rank: 199
    paper_rank: 238
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.7487
    std: 0.0013
    paper_value: 0.7487
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.749
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.001
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7198
    std: 0.0042
    paper_value: 0.7198
    paper_std: 0.0042
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-12'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7469
    true_std: 0.0085
    value_gap_source_arxiv: '2512.11561'
    value_gap_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.027100000000000013
    has_value_note: false
    value_note: ''
    sort_value: 0.7469
    sort_std: 0.0085
    global_rank: 237
    paper_rank: 255
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.7176
    std: 0.0014
    paper_value: 0.7176
    paper_std: 0.0014
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on WikiCS node classification task using standard split.
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7176
    true_std: 0.0014
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7176
    sort_std: 0.0014
    global_rank: 263
    paper_rank: 263
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
- &id008
  dataset: twitch-gamers
  rows:
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.6634
    std: 0.0029
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/benfinkelshtein/ICGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6634
    sort_std: 0.0029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGT
    model_key: dgt
    model_plain: DGT
    value: 0.6609
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6609
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ICG_u-NN
    model_key: icg_u-nn
    model_plain: ICG_u-NN
    value: 0.6608
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/benfinkelshtein/ICGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6608
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6473
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.6473
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6274
    std: 0.0003
    paper_value: 0.6274
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6218
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-08-13'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.005599999999999938
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6456
    true_std: 0.0019
    value_gap_source_arxiv: '2408.07191'
    value_gap_source_title: Joint Graph Rewiring and Feature Denoising via Spectral
      Resonance
    value_gap_source_is_current_paper: false
    value_gap: 0.018199999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6456
    sort_std: 0.0019
    global_rank: 19
    paper_rank: 30
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: AF-GCL
    model_key: af-gcl
    model_plain: AF-GCL
    value: 0.6204
    std: 0.0017
    paper_value: 0.6204
    paper_std: 0.0017
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
    input_feature_source: raw_features
    feature_source_evidence: constructs positive/negative pairs based on the aggregated
      node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6204
    true_std: 0.0017
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6204
    sort_std: 0.0017
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.6171
    std: 0.0041
    paper_value: 0.6171
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6171
    true_std: 0.0041
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6171
    sort_std: 0.0041
    global_rank: 36
    paper_rank: 36
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
    value: 0.6147
    std: 0.0056
    paper_value: 0.6147
    paper_std: 0.0056
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6147
    true_std: 0.0056
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6147
    sort_std: 0.0056
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6071
    std: 0.0018
    paper_value: 0.6071
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6092
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0020999999999999908
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6114
    true_std: 0.0006
    value_gap_source_arxiv: '2206.14337'
    value_gap_source_title: Deformable Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.0043000000000000815
    has_value_note: false
    value_note: ''
    sort_value: 0.6114
    sort_std: 0.0006
    global_rank: 39
    paper_rank: 44
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2cec
    model_key: node2cec
    model_plain: Node2cec
    value: 0.6112
    std: 0.0029
    paper_value: 0.6112
    paper_std: 0.0029
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
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
    true_std: 0.0029
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6112
    sort_std: 0.0029
    global_rank: 40
    paper_rank: 40
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
    value: 0.6093
    std: 0.0032
    paper_value: 0.6093
    paper_std: 0.0032
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6093
    true_std: 0.0032
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6093
    sort_std: 0.0032
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.607
    std: 0.0061
    paper_value: 0.607
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.607
    true_std: 0.0061
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.607
    sort_std: 0.0061
    global_rank: 45
    paper_rank: 45
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
    value: 0.5626
    std: 0.005
    paper_value: 0.5626
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification on Twitch-gamers test split
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5626
    true_std: 0.005
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5626
    sort_std: 0.005
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id005
  - *id006
  - *id007
- benchmark: LINKX Benchmarks
  datasets:
  - *id008
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: twitch-gamers
      dataset_slug: twitch-gamers
single_proposed_model: AF-GCL
main_figure: /figures/2204.04874/main_figure.jpegoptim.jpg
---

