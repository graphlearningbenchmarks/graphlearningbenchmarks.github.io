---
title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks via Singular Value
  Decomposition'
arxiv_id: '2601.08230'
source_url: ''
authors:
- name: Hao Deng
  orcid: null
  s2_author_id: '2404597790'
  s2_url: null
- name: Bo Liu
  orcid: null
  s2_author_id: '2405124227'
  s2_url: null
published_date: Jan 13, 2026
published_date_iso: '2026-01-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'While Graph Neural Networks (GNNs) excel on graph-structured data, their
  performance is fundamentally limited by the quality of the observed graph, which
  often contains noise, missing links, or structural properties misaligned with GNNs''
  underlying assumptions. To address this, graph structure learning aims to infer
  a more optimal topology. Existing methods, however, often incur high computational
  costs due to complex generative models and iterative joint optimization, limiting
  their practical utility. In this paper, we propose GADPN, a simple yet effective
  graph structure learning framework that adaptively refines graph topology via low-rank
  denoising and generalized structural perturbation. Our approach makes two key contributions:
  (1) we introduce Bayesian optimization to adaptively determine the optimal denoising
  strength, tailoring the process to each graph''s homophily level; and (2) we extend
  the structural perturbation method to arbitrary graphs via Singular Value Decomposition
  (SVD), overcoming its original limitation to symmetric structures. Extensive experiments
  on benchmark datasets demonstrate that GADPN not only achieves state-of-the-art
  performance but does so with significantly improved efficiency. It shows particularly
  strong gains on challenging disassortative graphs, validating its ability to robustly
  learn enhanced graph structures across diverse network types.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphSAGE
- GADPN
mrr: 0.0045
adjusted_mrr: 0.0045
mrr_dataset_count: 5
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.282
    std: null
    paper_value: 0.282
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4046
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.12260000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4046
    true_std: 0.0064
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.12260000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.4046
    sort_std: 0.0064
    global_rank: 46
    paper_rank: 404
    rank_delta: 358
    rank_delta_abs: 358
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.336
    std: null
    paper_value: 0.336
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.397
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.061
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3908
    true_std: 0.0065
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05479999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.3908
    sort_std: 0.0065
    global_rank: 68
    paper_rank: 295
    rank_delta: 227
    rank_delta_abs: 227
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.338
    std: null
    paper_value: 0.338
    paper_std: null
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
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3899
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0519
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3899
    true_std: 0.0085
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0519
    has_value_note: false
    value_note: ''
    sort_value: 0.3899
    sort_std: 0.0085
    global_rank: 70
    paper_rank: 290
    rank_delta: 220
    rank_delta_abs: 220
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: GEN
    model_key: gen
    model_plain: GEN
    value: 0.328
    std: null
    paper_value: 0.328
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.373
    at_pub_std: 0.014
    at_pub_source_arxiv: '2205.13700'
    at_pub_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    at_pub_source_date_iso: '2022-05-27'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.044999999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.373
    true_std: 0.014
    value_gap_source_arxiv: '2205.13700'
    value_gap_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    value_gap_source_is_current_paper: false
    value_gap: 0.044999999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.373
    sort_std: 0.014
    global_rank: 127
    paper_rank: 308
    rank_delta: 181
    rank_delta_abs: 181
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    comparison_source_arxiv: '2205.13700'
    is_best: false
    is_std_outlier: false
  - model: GADPN
    model_key: gadpn
    model_plain: GADPN
    value: 0.364
    std: null
    paper_value: 0.364
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.364
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.364
    sort_std: null
    global_rank: 176
    paper_rank: 176
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
    value: 0.289
    std: null
    paper_value: 0.289
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
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
    gap_vs_at_pub: 0.08000000000000002
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
    value_gap: 0.07300000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.362
    sort_std: 0.01
    global_rank: 184
    paper_rank: 390
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.266
    std: null
    paper_value: 0.266
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.361
    at_pub_std: 0.0155
    at_pub_source_arxiv: '2405.12474'
    at_pub_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph Neural
      Networks: Heterophily, Over-smoothing, and Over-squashing'
    at_pub_source_date_iso: '2024-05-21'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.09499999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.361
    true_std: 0.0155
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.09499999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.361
    sort_std: 0.0155
    global_rank: 189
    paper_rank: 423
    rank_delta: 234
    rank_delta_abs: 234
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    comparison_source_arxiv: '2405.12474'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.285
    std: null
    paper_value: 0.285
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
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
    gap_vs_at_pub: 0.07550000000000001
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
    value_gap: 0.07550000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 191
    paper_rank: 399
    rank_delta: 208
    rank_delta_abs: 208
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.281
    std: null
    paper_value: 0.281
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.351
    at_pub_std: 0.002
    at_pub_source_arxiv: '2505.11346'
    at_pub_source_title: What Can We Learn From MIMO Graph Convolutions?
    at_pub_source_date_iso: '2025-05-16'
    at_pub_source_date_label: IJCAI 2025
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.06999999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.351
    true_std: 0.002
    value_gap_source_arxiv: '2505.11346'
    value_gap_source_title: What Can We Learn From MIMO Graph Convolutions?
    value_gap_source_is_current_paper: false
    value_gap: 0.06999999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.351
    sort_std: 0.002
    global_rank: 248
    paper_rank: 406
    rank_delta: 158
    rank_delta_abs: 158
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: What Can We Learn From MIMO Graph Convolutions?
    comparison_source_arxiv: '2505.11346'
    is_best: false
    is_std_outlier: false
  - model: AGNN
    model_key: agnn
    model_plain: AGNN
    value: 0.322
    std: null
    paper_value: 0.322
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (3648
      train, 2432 val, 1520 test).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.24
    at_pub_std: 0.03
    at_pub_source_arxiv: '2506.13083'
    at_pub_source_title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop Evidence
      Fusion Approach'
    at_pub_source_date_iso: '2025-06-16'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08200000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.322
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.322
    sort_std: null
    global_rank: 317
    paper_rank: 317
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop
      Evidence Fusion Approach'
    comparison_source_arxiv: '2506.13083'
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
  dataset: Chameleon
  rows:
  - model: FE-GNN
    model_key: hetero-s (gat 8-layer)
    model_plain: FE-GNN
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
  - model: FE-GNN
    model_key: trans.conv+cna
    model_plain: FE-GNN
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.856
    at_pub_std: null
    at_pub_source_arxiv: '2406.12539'
    at_pub_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    at_pub_source_date_iso: '2024-06-18'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-06-18'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.415
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.856
    true_std: null
    value_gap_source_arxiv: '2406.12539'
    value_gap_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.415
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: null
    global_rank: 3
    paper_rank: 258
    rank_delta: 255
    rank_delta_abs: 255
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'The Heterophilic Snowflake Hypothesis: Training and
      Empowering GNNs for Heterophilic Graphs'
    comparison_source_arxiv: '2406.12539'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.344
    std: null
    paper_value: 0.344
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7033
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.35930000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.35930000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7033
    sort_std: null
    global_rank: 63
    paper_rank: 301
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.346
    std: null
    paper_value: 0.346
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.671
    at_pub_std: 0.029
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.32500000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.671
    true_std: 0.029
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.32500000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.671
    sort_std: 0.029
    global_rank: 94
    paper_rank: 300
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.393
    std: null
    paper_value: 0.393
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.667
    at_pub_std: 0.027
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.274
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.667
    true_std: 0.027
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.274
    has_value_note: false
    value_note: ''
    sort_value: 0.667
    sort_std: 0.027
    global_rank: 99
    paper_rank: 291
    rank_delta: 192
    rank_delta_abs: 192
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.393
    std: null
    paper_value: 0.393
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6344
    at_pub_std: 0.0205
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.24139999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6344
    true_std: 0.0205
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.24139999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.6344
    sort_std: 0.0205
    global_rank: 128
    paper_rank: 291
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.463
    std: null
    paper_value: 0.463
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6215
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.15850000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6215
    true_std: 0.0042
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.15850000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.6215
    sort_std: 0.0042
    global_rank: 137
    paper_rank: 245
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: GADPN
    model_key: gadpn
    model_plain: GADPN
    value: 0.611
    std: null
    paper_value: 0.611
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.611
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.611
    sort_std: null
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEN
    model_key: gen
    model_plain: GEN
    value: 0.575
    std: null
    paper_value: 0.575
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.575
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.575
    sort_std: null
    global_rank: 178
    paper_rank: 178
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.426
    std: null
    paper_value: 0.426
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.471
    at_pub_std: 0.003
    at_pub_source_arxiv: '2505.11346'
    at_pub_source_title: What Can We Learn From MIMO Graph Convolutions?
    at_pub_source_date_iso: '2025-05-16'
    at_pub_source_date_label: IJCAI 2025
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.044999999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.471
    true_std: 0.003
    value_gap_source_arxiv: '2505.11346'
    value_gap_source_title: What Can We Learn From MIMO Graph Convolutions?
    value_gap_source_is_current_paper: false
    value_gap: 0.044999999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.471
    sort_std: 0.003
    global_rank: 241
    paper_rank: 271
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: What Can We Learn From MIMO Graph Convolutions?
    comparison_source_arxiv: '2505.11346'
    is_best: false
    is_std_outlier: false
  - model: AGNN
    model_key: agnn
    model_plain: AGNN
    value: 0.434
    std: null
    paper_value: 0.434
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Chameleon test split (456 nodes).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.434
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.434
    sort_std: null
    global_rank: 265
    paper_rank: 265
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
  dataset: CiteSeer
  rows:
  - model: SGC+TSC
    model_key: cna
    model_plain: SGC+TSC
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
  - model: SGC+TSC
    model_key: is-gib
    model_plain: SGC+TSC
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
    input_feature_source: null
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
  - model: SGC+TSC
    model_key: eerm
    model_plain: SGC+TSC
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
    input_feature_source: null
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
    value: 0.699
    std: null
    paper_value: 0.699
    paper_std: null
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
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8774
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1784
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8774
    true_std: 0.0041
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1784
    has_value_note: false
    value_note: ''
    sort_value: 0.8774
    sort_std: 0.0041
    global_rank: 20
    paper_rank: 686
    rank_delta: 666
    rank_delta_abs: 666
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.711
    std: null
    paper_value: 0.711
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8769
    at_pub_std: 0.004
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.16590000000000005
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
    value_gap: 0.16590000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 610
    rank_delta: 589
    rank_delta_abs: 589
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.711
    std: null
    paper_value: 0.711
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8142
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.10320000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8142
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10320000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 610
    rank_delta: 581
    rank_delta_abs: 581
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.701
    std: null
    paper_value: 0.701
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.808
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1070000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1070000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 678
    rank_delta: 632
    rank_delta_abs: 632
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.713
    std: null
    paper_value: 0.713
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7965
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-11-30'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08350000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7965
    true_std: 0.0102
    value_gap_source_arxiv: '2311.18177'
    value_gap_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08350000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0102
    global_rank: 68
    paper_rank: 587
    rank_delta: 519
    rank_delta_abs: 519
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.67
    std: null
    paper_value: 0.67
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7928
    at_pub_std: 0.017
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12279999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7928
    true_std: 0.017
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.12279999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.7928
    sort_std: 0.017
    global_rank: 76
    paper_rank: 780
    rank_delta: 704
    rank_delta_abs: 704
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: AGNN
    model_key: agnn
    model_plain: AGNN
    value: 0.694
    std: null
    paper_value: 0.694
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.738
    at_pub_std: 0.007
    at_pub_source_arxiv: '2204.06127'
    at_pub_source_title: 'Reinforcement learning on graphs: A survey'
    at_pub_source_date_iso: '2022-04-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-13'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04400000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.738
    true_std: 0.007
    value_gap_source_arxiv: '2204.06127'
    value_gap_source_title: 'Reinforcement learning on graphs: A survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.04400000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.738
    sort_std: 0.007
    global_rank: 282
    paper_rank: 701
    rank_delta: 419
    rank_delta_abs: 419
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Reinforcement learning on graphs: A survey'
    comparison_source_arxiv: '2204.06127'
    is_best: false
    is_std_outlier: false
  - model: GEN
    model_key: gen
    model_plain: GEN
    value: 0.708
    std: null
    paper_value: 0.708
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7321
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2205.07266'
    at_pub_source_title: Discovering the Representation Bottleneck of Graph Neural
      Networks
    at_pub_source_date_iso: '2022-05-15'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-15'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02410000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7321
    true_std: 0.0062
    value_gap_source_arxiv: '2205.07266'
    value_gap_source_title: Discovering the Representation Bottleneck of Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.02410000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7321
    sort_std: 0.0062
    global_rank: 349
    paper_rank: 633
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Discovering the Representation Bottleneck of Graph Neural
      Networks
    comparison_source_arxiv: '2205.07266'
    is_best: false
    is_std_outlier: false
  - model: GADPN
    model_key: gadpn
    model_plain: GADPN
    value: 0.728
    std: null
    paper_value: 0.728
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.728
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.728
    sort_std: null
    global_rank: 407
    paper_rank: 407
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.706
    std: null
    paper_value: 0.706
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016) using
      Accuracy metric.
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.699
    at_pub_std: null
    at_pub_source_arxiv: '2310.01089'
    at_pub_source_title: 'GraphText: Graph Reasoning in Text Space'
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.706
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.706
    sort_std: null
    global_rank: 647
    paper_rank: 647
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphText: Graph Reasoning in Text Space'
    comparison_source_arxiv: '2310.01089'
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
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.81
    std: null
    paper_value: 0.81
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.09039999999999992
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
    value_gap: 0.09039999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 735
    rank_delta: 702
    rank_delta_abs: 702
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.826
    std: null
    paper_value: 0.826
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8904
    at_pub_std: 0.015
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06440000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8904
    true_std: 0.015
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.06440000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 571
    rank_delta: 502
    rank_delta_abs: 502
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.817
    std: null
    paper_value: 0.817
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8897
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.0727000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0727000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 680
    rank_delta: 608
    rank_delta_abs: 608
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8
    std: null
    paper_value: 0.8
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8777
    at_pub_std: 0.0183
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.07769999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8889
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08889999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8889
    sort_std: null
    global_rank: 79
    paper_rank: 775
    rank_delta: 696
    rank_delta_abs: 696
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    comparison_source_arxiv: '2110.15777'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.82
    std: null
    paper_value: 0.82
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8885
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0685
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8885
    true_std: 0.0136
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.0685
    has_value_note: false
    value_note: ''
    sort_value: 0.8885
    sort_std: 0.0136
    global_rank: 81
    paper_rank: 647
    rank_delta: 566
    rank_delta_abs: 566
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8
    std: null
    paper_value: 0.8
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.06829999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8797
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0797
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: null
    global_rank: 138
    paper_rank: 775
    rank_delta: 637
    rank_delta_abs: 637
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.815
    std: null
    paper_value: 0.815
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8406
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2210.07715'
    at_pub_source_title: 'Not All Neighbors Are Worth Attending to: Graph Selective
      Attention Networks for Semi-supervised Learning'
    at_pub_source_date_iso: '2022-10-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.025600000000000067
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8406
    true_std: 0.0083
    value_gap_source_arxiv: '2210.07715'
    value_gap_source_title: 'Not All Neighbors Are Worth Attending to: Graph Selective
      Attention Networks for Semi-supervised Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.025600000000000067
    has_value_note: false
    value_note: ''
    sort_value: 0.8406
    sort_std: 0.0083
    global_rank: 406
    paper_rank: 695
    rank_delta: 289
    rank_delta_abs: 289
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Not All Neighbors Are Worth Attending to: Graph Selective
      Attention Networks for Semi-supervised Learning'
    comparison_source_arxiv: '2210.07715'
    is_best: false
    is_std_outlier: false
  - model: AGNN
    model_key: agnn
    model_plain: AGNN
    value: 0.812
    std: null
    paper_value: 0.812
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.836
    at_pub_std: 0.003
    at_pub_source_arxiv: '2204.06127'
    at_pub_source_title: 'Reinforcement learning on graphs: A survey'
    at_pub_source_date_iso: '2022-04-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-13'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02399999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.836
    true_std: 0.003
    value_gap_source_arxiv: '2204.06127'
    value_gap_source_title: 'Reinforcement learning on graphs: A survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.02399999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.003
    global_rank: 458
    paper_rank: 713
    rank_delta: 255
    rank_delta_abs: 255
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Reinforcement learning on graphs: A survey'
    comparison_source_arxiv: '2204.06127'
    is_best: false
    is_std_outlier: false
  - model: GADPN
    model_key: gadpn
    model_plain: GADPN
    value: 0.832
    std: null
    paper_value: 0.832
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.832
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: null
    global_rank: 526
    paper_rank: 526
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEN
    model_key: gen
    model_plain: GEN
    value: 0.812
    std: null
    paper_value: 0.812
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Planetoid split (Yang et al. 2016 fixed
      20-per-class train split).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8166
    at_pub_std: 0.0091
    at_pub_source_arxiv: '2205.07266'
    at_pub_source_title: Discovering the Representation Bottleneck of Graph Neural
      Networks
    at_pub_source_date_iso: '2022-05-15'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-15'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0045999999999999375
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8166
    true_std: 0.0091
    value_gap_source_arxiv: '2205.07266'
    value_gap_source_title: Discovering the Representation Bottleneck of Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0045999999999999375
    has_value_note: false
    value_note: ''
    sort_value: 0.8166
    sort_std: 0.0091
    global_rank: 691
    paper_rank: 713
    rank_delta: 22
    rank_delta_abs: 22
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
- &id005
  dataset: Squirrel
  rows:
  - model: FE-GNN
    model_key: ibg-nn
    model_plain: FE-GNN
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
  - model: FE-GNN
    model_key: trans.conv+cna
    model_plain: FE-GNN
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
  - model: FE-GNN
    model_key: dhgnn
    model_plain: FE-GNN
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
    value: 0.277
    std: null
    paper_value: 0.277
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6067
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.3297
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.3297
    has_value_note: false
    value_note: ''
    sort_value: 0.6067
    sort_std: null
    global_rank: 49
    paper_rank: 280
    rank_delta: 231
    rank_delta_abs: 231
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.272
    std: null
    paper_value: 0.272
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.563
    at_pub_std: 0.022
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2909999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.563
    true_std: 0.022
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2909999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.563
    sort_std: 0.022
    global_rank: 73
    paper_rank: 284
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.285
    std: null
    paper_value: 0.285
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.559
    at_pub_std: 0.029
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2740000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.559
    true_std: 0.029
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2740000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.559
    sort_std: 0.029
    global_rank: 74
    paper_rank: 275
    rank_delta: 201
    rank_delta_abs: 201
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.278
    std: null
    paper_value: 0.278
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.523
    at_pub_std: 0.023
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.245
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.523
    true_std: 0.023
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.245
    has_value_note: false
    value_note: ''
    sort_value: 0.523
    sort_std: 0.023
    global_rank: 92
    paper_rank: 280
    rank_delta: 188
    rank_delta_abs: 188
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.314
    std: null
    paper_value: 0.314
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4378
    at_pub_std: 0.019
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12380000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4378
    true_std: 0.019
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.12380000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4378
    sort_std: 0.019
    global_rank: 140
    paper_rank: 261
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.27
    std: null
    paper_value: 0.27
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4259
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2210.00513'
    at_pub_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-02'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.15589999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4259
    true_std: 0.0079
    value_gap_source_arxiv: '2210.00513'
    value_gap_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.15589999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4259
    sort_std: 0.0079
    global_rank: 153
    paper_rank: 284
    rank_delta: 131
    rank_delta_abs: 131
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    comparison_source_arxiv: '2210.00513'
    is_best: false
    is_std_outlier: false
  - model: GADPN
    model_key: gadpn
    model_plain: GADPN
    value: 0.396
    std: null
    paper_value: 0.396
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.396
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.396
    sort_std: null
    global_rank: 184
    paper_rank: 184
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEN
    model_key: gen
    model_plain: GEN
    value: 0.368
    std: null
    paper_value: 0.368
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.368
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.368
    sort_std: null
    global_rank: 217
    paper_rank: 217
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.278
    std: null
    paper_value: 0.278
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.351
    at_pub_std: 0.002
    at_pub_source_arxiv: '2505.11346'
    at_pub_source_title: What Can We Learn From MIMO Graph Convolutions?
    at_pub_source_date_iso: '2025-05-16'
    at_pub_source_date_label: IJCAI 2025
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.07299999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.351
    true_std: 0.002
    value_gap_source_arxiv: '2505.11346'
    value_gap_source_title: What Can We Learn From MIMO Graph Convolutions?
    value_gap_source_is_current_paper: false
    value_gap: 0.07299999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.351
    sort_std: 0.002
    global_rank: 239
    paper_rank: 280
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: What Can We Learn From MIMO Graph Convolutions?
    comparison_source_arxiv: '2505.11346'
    is_best: false
    is_std_outlier: false
  - model: AGNN
    model_key: agnn
    model_plain: AGNN
    value: 0.274
    std: null
    paper_value: 0.274
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using standard split (1664/1041
      val/test as per Table 1).
    date: Jan 13, 2026
    date_display: Jan 2026
    date_iso: '2026-01-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.274
    true_std: null
    value_gap_source_arxiv: '2601.08230'
    value_gap_source_title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks
      via Singular Value Decomposition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.274
    sort_std: null
    global_rank: 284
    paper_rank: 284
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
main_figure: /figures/2601.08230/main_figure.jpegoptim.jpg
---

