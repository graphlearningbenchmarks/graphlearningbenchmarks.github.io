---
title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks with Graph Kernels'
arxiv_id: '1905.13192'
source_url: ''
authors:
- name: Simon S. Du
  orcid: null
  s2_author_id: '145697585'
  s2_url: null
- name: Kangcheng Hou
  orcid: null
  s2_author_id: '51151695'
  s2_url: null
- name: Barnab\'as P\'oczos
  orcid: null
  s2_author_id: '1719347'
  s2_url: null
- name: Ruslan Salakhutdinov
  orcid: null
  s2_author_id: '145124475'
  s2_url: null
- name: Ruosong Wang
  orcid: null
  s2_author_id: '2108693711'
  s2_url: null
- name: Keyulu Xu
  orcid: null
  s2_author_id: '3360632'
  s2_url: null
published_date: May 30, 2019
published_date_iso: '2019-05-30'
published_venue: NeurIPS 2019
published_conference: NeurIPS 2019
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: While graph kernels (GKs) are easy to train and enjoy provable theoretical
  guarantees, their practical performances are limited by their expressive power,
  as the kernel function often depends on hand-crafted combinatorial features of graphs.
  Compared to graph kernels, graph neural networks (GNNs) usually achieve better practical
  performance, as GNNs use multi-layer architectures and non-linear activation functions
  to extract high-order information of graphs as features. However, due to the large
  number of hyper-parameters and the non-convex nature of the training procedure,
  GNNs are harder to train. Theoretical guarantees of GNNs are also not well-understood.
  Furthermore, the expressive power of GNNs scales with the number of parameters,
  and thus it is hard to exploit the full power of GNNs when computing resources are
  limited. The current paper presents a new class of graph kernels, Graph Neural Tangent
  Kernels (GNTKs), which correspond to infinitely wide multi-layer GNNs trained by
  gradient descent. GNTKs enjoy the full expressive power of GNNs and inherit advantages
  of GKs. Theoretically, we show GNTKs provably learn a class of smooth functions
  on graphs. Empirically, we test GNTKs on graph classification datasets and show
  they achieve strong performance.
codebase_url: https://github.com/KangchengHou/gntk
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GNTK
mrr: 0.0281
adjusted_mrr: 0.0281
mrr_dataset_count: 4
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id003
  dataset: COLLAB
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9792
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.964
    std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoCN
    model_key: cocn
    model_plain: CoCN
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNTK
    model_key: gntk
    model_plain: GNTK
    value: 0.836
    std: 0.01
    paper_value: 0.836
    paper_std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.01
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.01
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.79
    std: 0.018
    paper_value: 0.79
    paper_std: 0.018
    metric: Accuracy
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.806
    at_pub_std: 0.021
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.826
    true_std: 0.022
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.03599999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.022
    global_rank: 23
    paper_rank: 164
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.802
    std: 0.019
    paper_value: 0.802
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
    source_ref: xu2018how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.802
    at_pub_std: 0.019
    at_pub_source_arxiv: '1905.12560'
    at_pub_source_title: On the Equivalence between Graph Isomorphism Testing and
      Function Approximation with GNNs
    at_pub_source_date_iso: '2019-05-29'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.021
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.019999999999999907
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.021
    global_rank: 30
    paper_rank: 115
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RetGK
    model_key: retgk
    model_plain: RetGK
    value: 0.81
    std: 0.003
    paper_value: 0.81
    paper_std: 0.003
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
    source_ref: Zhang2018RetGKGK
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: 0.003
    value_gap_source_arxiv: '2502.16233'
    value_gap_source_title: Graph Self-Supervised Learning with Learnable Structural
      and Positional Encodings
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: 0.003
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.797
    std: 0.017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 142
    sort_value: 0.797
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.792
    std: 0.024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 157
    sort_value: 0.792
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL subtree
    model_key: wl subtree
    model_plain: WL subtree
    value: 0.789
    std: 0.019
    paper_value: 0.789
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
    source_ref: shervashidze2011weisfeiler
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.789
    at_pub_std: 0.019
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.789
    true_std: 0.019
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.019
    global_rank: 171
    paper_rank: 171
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.737
    std: null
    paper_value: 0.737
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
    source_ref: zhang2018end
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.7376
    at_pub_std: 0.0049
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2025-09-01'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.0006000000000000449
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7759
    true_std: 0.0224
    value_gap_source_arxiv: '2512.04530'
    value_gap_source_title: Explainable Graph Representation Learning via Graph Pattern
      Analysis
    value_gap_source_is_current_paper: false
    value_gap: 0.038900000000000046
    has_value_note: false
    value_note: ''
    sort_value: 0.7759
    sort_std: 0.0224
    global_rank: 202
    paper_rank: 293
    rank_delta: 91
    rank_delta_abs: 91
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AWL
    model_key: awl
    model_plain: AWL
    value: 0.739
    std: 0.019
    paper_value: 0.739
    paper_std: 0.019
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
    source_ref: Ivanov2018AnonymousWE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.739
    at_pub_std: 0.019
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: 0.019
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: 0.019
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
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.726
    std: 0.022
    paper_value: 0.726
    paper_std: 0.022
    metric: Accuracy
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on COLLAB
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.726
    at_pub_std: 0.022
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.042
    global_rank: 304
    paper_rank: 304
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
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
    std: 0.003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.894
    std: 0.056
    paper_value: 0.894
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
    table_ref: Table 1
    source_ref: xu2018how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.894
    at_pub_std: 0.056
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 254
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.926
    std: 0.042
    paper_value: 0.926
    paper_std: 0.042
    metric: Accuracy
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.926
    at_pub_std: 0.042
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.926
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.926
    sort_std: 0.042
    global_rank: 61
    paper_rank: 61
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
    value: 0.856
    std: 0.058
    paper_value: 0.856
    paper_std: 0.058
    metric: Accuracy
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.857
    at_pub_std: 0.066
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2025-03-03'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.044
    value_gap_source_arxiv: '2503.01079'
    value_gap_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.06600000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.044
    global_rank: 71
    paper_rank: 465
    rank_delta: 394
    rank_delta_abs: 394
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
    value: 0.851
    std: 0.076
    paper_value: 0.851
    paper_std: 0.076
    metric: Accuracy
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.857
    at_pub_std: 0.047
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-05-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.078
    value_gap_source_arxiv: '2205.12245'
    value_gap_source_title: Asynchronous Neural Networks for Learning in Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.05300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.078
    global_rank: 170
    paper_rank: 483
    rank_delta: 313
    rank_delta_abs: 313
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL subtree
    model_key: wl subtree
    model_plain: WL subtree
    value: 0.904
    std: 0.057
    paper_value: 0.904
    paper_std: 0.057
    metric: Accuracy
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
    source_ref: shervashidze2011weisfeiler
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RetGK
    model_key: retgk
    model_plain: RetGK
    value: 0.903
    std: 0.011
    paper_value: 0.903
    paper_std: 0.011
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
    source_ref: Zhang2018RetGK
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.011
    value_gap_source_arxiv: '2502.16233'
    value_gap_source_title: Graph Self-Supervised Learning with Learnable Structural
      and Positional Encodings
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.011
    global_rank: 188
    paper_rank: 188
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNTK
    model_key: gntk
    model_plain: GNTK
    value: 0.9
    std: 0.085
    paper_value: 0.9
    paper_std: 0.085
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: 0.085
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.085
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
  - model: AWL
    model_key: awl
    model_plain: AWL
    value: 0.879
    std: 0.098
    paper_value: 0.879
    paper_std: 0.098
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
    source_ref: Ivanov2018AnonymousWE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.879
    at_pub_std: 0.098
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.879
    true_std: 0.098
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.098
    global_rank: 356
    paper_rank: 356
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
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.858
    std: null
    paper_value: 0.858
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
    source_ref: zhang2018end
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.8583
    at_pub_std: null
    at_pub_source_arxiv: '1901.08296'
    at_pub_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    at_pub_source_date_iso: '2018-12-14'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8583
    true_std: 0.0116
    value_gap_source_arxiv: '2412.17856'
    value_gap_source_title: Graph Structure Refinement with Energy-based Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.8583
    sort_std: 0.0116
    global_rank: 455
    paper_rank: 455
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    comparison_source_arxiv: '1901.08296'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7518
    std: 0.047
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_display: Jun 2024
    date_iso: '2024-06-03'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 785
    sort_value: 0.7518
    sort_std: 0.047
    comparison_type: global_top
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
- &id002
  dataset: NCI1
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.827
    std: 0.017
    paper_value: 0.827
    paper_std: 0.017
    metric: Accuracy
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
    source_ref: xu2018how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.827
    at_pub_std: 0.017
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9934
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.1664
    has_value_note: false
    value_note: ''
    sort_value: 0.9934
    sort_std: null
    global_rank: 2
    paper_rank: 101
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.802
    std: 0.02
    paper_value: 0.802
    paper_std: 0.02
    metric: Accuracy
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.725
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07700000000000007
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9727
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.17069999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9727
    sort_std: null
    global_rank: 3
    paper_rank: 233
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
    is_best: false
    is_std_outlier: false
  - model: WL subtree
    model_key: wl subtree
    model_plain: WL subtree
    value: 0.86
    std: 0.018
    paper_value: 0.86
    paper_std: 0.018
    metric: Accuracy
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
    source_ref: shervashidze2011weisfeiler
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.8219
    at_pub_std: null
    at_pub_source_arxiv: '1603.05629'
    at_pub_source_title: Discriminative Embeddings of Latent Variable Models for Structured
      Data
    at_pub_source_date_iso: '2016-03-17'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2020-09-07'
    value_gap_source_date_label: ICML 2020
    gap_vs_at_pub: 0.03810000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2009.03294'
    value_gap_source_title: 'GraphNorm: A Principled Approach to Accelerating Graph
      Neural Network Training'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Discriminative Embeddings of Latent Variable Models for
      Structured Data
    comparison_source_arxiv: '1603.05629'
    is_best: false
    is_std_outlier: false
  - model: RetGK
    model_key: retgk
    model_plain: RetGK
    value: 0.845
    std: 0.002
    paper_value: 0.845
    paper_std: 0.002
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
    source_ref: Zhang2018RetGK
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.002
    value_gap_source_arxiv: '2502.16233'
    value_gap_source_title: Graph Self-Supervised Learning with Learnable Structural
      and Positional Encodings
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.002
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNTK
    model_key: gntk
    model_plain: GNTK
    value: 0.842
    std: 0.015
    paper_value: 0.842
    paper_std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.842
    true_std: 0.015
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.842
    sort_std: 0.015
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.777
    std: 0.015
    paper_value: 0.777
    paper_std: 0.015
    metric: Accuracy
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.732
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.04500000000000004
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8303
    true_std: 0.0137
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_gap_source_is_current_paper: false
    value_gap: 0.053300000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.8303
    sort_std: 0.0137
    global_rank: 82
    paper_rank: 365
    rank_delta: 283
    rank_delta_abs: 283
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.786
    std: 0.019
    paper_value: 0.786
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-01'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.786
    true_std: 0.019
    value_gap_source_arxiv: '2202.00529'
    value_gap_source_title: Molecular Representation Learning via Heterogeneous Motif
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.786
    sort_std: 0.019
    global_rank: 319
    paper_rank: 319
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.744
    std: null
    paper_value: 0.744
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
    source_ref: zhang2018end
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on NCI1
    date: May 30, 2019
    date_display: May 2019
    date_iso: '2019-05-30'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.7444
    at_pub_std: 0.0047
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.765
    true_std: 0.019
    value_gap_source_arxiv: '2009.10564'
    value_gap_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.02100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.765
    sort_std: 0.019
    global_rank: 411
    paper_rank: 471
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.749
    std: 0.017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_display: Jun 2024
    date_iso: '2024-06-03'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 462
    sort_value: 0.749
    sort_std: 0.017
    comparison_type: global_top
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: COLLAB
      dataset_slug: collab
single_proposed_model: GNTK
main_figure: /figures/1905.13192/main_figure.jpegoptim.jpg
---

