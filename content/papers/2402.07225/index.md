---
title: Rethinking Graph Masked Autoencoders through Alignment and Uniformity
arxiv_id: '2402.07225'
source_url: ''
authors:
- name: Liang Wang
  orcid: null
  s2_author_id: '2258184369'
  s2_url: null
- name: Xiang Tao
  orcid: null
  s2_author_id: '2282967194'
  s2_url: null
- name: Q. Liu
  orcid: null
  s2_author_id: '48873756'
  s2_url: null
- name: Shu Wu
  orcid: null
  s2_author_id: '50425438'
  s2_url: null
published_date: Feb 11, 2024
published_date_iso: '2024-02-11'
published_venue: AAAI 2024
published_conference: AAAI 2024
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Self-supervised learning on graphs can be bifurcated into contrastive and
  generative methods. Contrastive methods, also known as graph contrastive learning
  (GCL), have dominated graph self-supervised learning in the past few years, but
  the recent advent of graph masked autoencoder (GraphMAE) rekindles the momentum
  behind generative methods. Despite the empirical success of GraphMAE, there is still
  a dearth of theoretical understanding regarding its efficacy. Moreover, while both
  generative and contrastive methods have been shown to be effective, their connections
  and differences have yet to be thoroughly investigated. Therefore, we theoretically
  build a bridge between GraphMAE and GCL, and prove that the node-level reconstruction
  objective in GraphMAE implicitly performs context-level GCL. Based on our theoretical
  analysis, we further identify the limitations of the GraphMAE from the perspectives
  of alignment and uniformity, which have been considered as two key properties of
  high-quality representations in GCL. We point out that GraphMAE's alignment performance
  is restricted by the masking strategy, and the uniformity is not strictly guaranteed.
  To remedy the aforementioned limitations, we propose an lignment- niformity enhanced
  raph asked uto ncoder, named AUG-MAE. Specifically, we propose an easy-to-hard adversarial
  masking strategy to provide hard-to-align samples, which improves the alignment
  performance. Meanwhile, we introduce an explicit uniformity regularizer to ensure
  the uniformity of the learned representations. Experimental results on benchmark
  datasets demonstrate the superiority of our model over existing state-of-the-art
  methods. The code is available at:.
codebase_url: https://github.com/AzureLeon1/AUG-MAE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AUG-MAE
mrr: 0.0078
adjusted_mrr: 0.0078
mrr_dataset_count: 8
benchmark_categories:
- Classic
- TU Dortmund
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id005
  dataset: COLLAB
  rows:
  - model: GPM
    model_key: wl-mlp
    model_plain: GPM
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
  - model: GPM
    model_key: msh-gnn
    model_plain: GPM
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
    input_feature_source: null
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
  - model: GPM
    model_key: cocn
    model_plain: GPM
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
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.8032
    std: 0.0042
    paper_value: 0.8032
    paper_std: 0.0042
    metric: Accuracy
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
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8032
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.827
    true_std: 0.01
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.023799999999999932
    has_value_note: false
    value_note: ''
    sort_value: 0.827
    sort_std: 0.01
    global_rank: 27
    paper_rank: 128
    rank_delta: 101
    rank_delta_abs: 101
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCC
    model_key: gcc
    model_plain: GCC
    value: 0.789
    std: null
    paper_value: 0.789
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.811
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-02-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.02200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.811
    true_std: null
    value_gap_source_arxiv: '2103.00111'
    value_gap_source_title: 'Graph Self-Supervised Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: null
    global_rank: 89
    paper_rank: 186
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Self-Supervised Learning: A Survey'
    comparison_source_arxiv: '2103.00111'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7136
    std: 0.0115
    paper_value: 0.7136
    paper_std: 0.0115
    metric: Accuracy
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
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8108
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.09719999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8108
    true_std: 0.0017
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.09719999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8108
    sort_std: 0.0017
    global_rank: 92
    paper_rank: 322
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.8048
    std: 0.005
    paper_value: 0.8048
    paper_std: 0.005
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.005
    value_gap_source_arxiv: '2512.13235'
    value_gap_source_title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.005
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGCL
    model_key: infogcl
    model_plain: InfoGCL
    value: 0.8
    std: 0.013
    paper_value: 0.8
    paper_std: 0.013
    metric: Accuracy
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
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8
    at_pub_std: 0.013
    at_pub_source_arxiv: '2110.15438'
    at_pub_source_title: 'InfoGCL: Information-Aware Graph Contrastive Learning'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-06-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8001
    true_std: 0.0132
    value_gap_source_arxiv: '2506.20362'
    value_gap_source_title: Self-Supervised Graph Learning via Spectral Bootstrapping
      and Laplacian-Based Augmentations
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8001
    sort_std: 0.0132
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7065
    std: 0.0113
    paper_value: 0.7065
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.794
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-03-01'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.08750000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.794
    true_std: null
    value_gap_source_arxiv: '2103.00959'
    value_gap_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08750000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: null
    global_rank: 165
    paper_rank: 328
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    comparison_source_arxiv: '2103.00959'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.695
    std: 0.0036
    paper_value: 0.695
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard data split for graph classification task.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7535
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-04'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.058499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7553
    true_std: 0.0018
    value_gap_source_arxiv: '2406.01899'
    value_gap_source_title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion
      Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.06030000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7553
    sort_std: 0.0018
    global_rank: 268
    paper_rank: 338
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
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
- &id004
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGCL
    model_key: infogcl
    model_plain: InfoGCL
    value: 0.912
    std: 0.013
    paper_value: 0.912
    paper_std: 0.013
    metric: Accuracy
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
    source_ref: InfoGCL [28]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.912
    at_pub_std: 0.013
    at_pub_source_arxiv: '2110.15438'
    at_pub_source_title: 'InfoGCL: Information-Aware Graph Contrastive Learning'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-10-24'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.013
    value_gap_source_arxiv: '2310.15523'
    value_gap_source_title: Generative and Contrastive Paradigms Are Complementary
      for Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.013
    global_rank: 94
    paper_rank: 94
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
    value: 0.897
    std: 0.011
    paper_value: 0.897
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
    source_ref: MVGRL [27]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8993
    at_pub_std: 0.0616
    at_pub_source_arxiv: '2305.19903'
    at_pub_source_title: Improving Expressivity of GNNs with Subgraph-specific Factor
      Embedded Normalization
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0022999999999999687
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8993
    true_std: 0.0616
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0022999999999999687
    has_value_note: false
    value_note: ''
    sort_value: 0.8993
    sort_std: 0.0616
    global_rank: 180
    paper_rank: 194
    rank_delta: 14
    rank_delta_abs: 14
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
    value: 0.8828
    std: 0.0098
    paper_value: 0.8828
    paper_std: 0.0098
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.898
    true_std: 0.013
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.015199999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.898
    sort_std: 0.013
    global_rank: 192
    paper_rank: 301
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.8901
    std: 0.0113
    paper_value: 0.8901
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
    source_ref: InfoGraph [23]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.893
    at_pub_std: 0.0514
    at_pub_source_arxiv: '2305.19903'
    at_pub_source_title: Improving Expressivity of GNNs with Subgraph-specific Factor
      Embedded Normalization
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0029000000000000137
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.0514
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0029000000000000137
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.0514
    global_rank: 236
    paper_rank: 251
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.8819
    std: 0.0126
    paper_value: 0.8819
    paper_std: 0.0126
    metric: Accuracy
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
    source_ref: GraphMAE [29]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8819
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.011
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.011099999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.011
    global_rank: 237
    paper_rank: 305
    rank_delta: 68
    rank_delta_abs: 68
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
    value: 0.868
    std: 0.0134
    paper_value: 0.868
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
    source_ref: GraphCL [24]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8829
    at_pub_std: 0.0131
    at_pub_source_arxiv: '2309.16014'
    at_pub_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    at_pub_source_date_iso: '2023-09-27'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-27'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.014900000000000024
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8829
    true_std: 0.0131
    value_gap_source_arxiv: '2309.16014'
    value_gap_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    value_gap_source_is_current_paper: false
    value_gap: 0.014900000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.8829
    sort_std: 0.0131
    global_rank: 301
    paper_rank: 377
    rank_delta: 76
    rank_delta_abs: 76
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
    value: 0.8735
    std: 0.0102
    paper_value: 0.8735
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
    source_ref: JOAO [25]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-02-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.0034999999999999476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.877
    true_std: null
    value_gap_source_arxiv: '2103.00111'
    value_gap_source_title: 'Graph Self-Supervised Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.0034999999999999476
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: null
    global_rank: 327
    paper_rank: 346
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.8315
    std: 0.0925
    paper_value: 0.8315
    paper_std: 0.0925
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
    source_ref: Graph2vec [22]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MUTAG
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8644
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.03289999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8644
    true_std: 0.0125
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.03289999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8644
    sort_std: 0.0125
    global_rank: 389
    paper_rank: 518
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
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
- &id003
  dataset: PPI
  rows:
  - model: Cluster-GCN
    model_key: gamlp(jk)
    model_plain: Cluster-GCN
    value: 0.9982
    std: 0.01
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9982
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Cluster-GCN
    model_key: graphcon-gcn
    model_plain: Cluster-GCN
    value: 0.996
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.996
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Cluster-GCN
    model_key: gcnii
    model_plain: Cluster-GCN
    value: 0.9956
    std: 0.02
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02133'
    title: Simple and Deep Graph Convolutional Networks
    date: Jul 4, 2020
    date_display: Jul 2020
    date_iso: '2020-07-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/DropEdge/DropEdge
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9956
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.741
    std: 0.004
    paper_value: 0.741
    paper_std: 0.004
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.745
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.0029
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.0029
    global_rank: 104
    paper_rank: 105
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.743
    std: 0.001
    paper_value: 0.743
    paper_std: 0.001
    metric: F1
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.743
    true_std: 0.001
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.001
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
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.739
    std: 0.003
    paper_value: 0.739
    paper_std: 0.003
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: 0.003
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: 0.003
    global_rank: 106
    paper_rank: 106
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
    value: 0.736
    std: 0.002
    paper_value: 0.736
    paper_std: 0.002
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7363
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7363
    true_std: 0.0016
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.7363
    sort_std: 0.0016
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEEGERA
    model_key: seegera
    model_plain: SEEGERA
    value: 0.734
    std: 0.003
    paper_value: 0.734
    paper_std: 0.003
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.003
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.003
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
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.733
    std: 0.002
    paper_value: 0.733
    paper_std: 0.002
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7334
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7334
    true_std: 0.0017
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000006697
    has_value_note: false
    value_note: ''
    sort_value: 0.7334
    sort_std: 0.0017
    global_rank: 109
    paper_rank: 109
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
    value: 0.697
    std: 0.002
    paper_value: 0.697
    paper_std: 0.002
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.6971
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.00010000000000010001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6971
    true_std: 0.0017
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000010001
    has_value_note: false
    value_note: ''
    sort_value: 0.6971
    sort_std: 0.0017
    global_rank: 116
    paper_rank: 117
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.638
    std: 0.002
    paper_value: 0.638
    paper_std: 0.002
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
    protocol_note: Micro-F1 reported for PPI
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.638
    at_pub_std: 0.002
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2021-06-04'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.638
    true_std: 0.002
    value_gap_source_arxiv: '2106.02466'
    value_gap_source_title: 'Graph Barlow Twins: A self-supervised representation
      learning framework for graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.638
    sort_std: 0.002
    global_rank: 137
    paper_rank: 137
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
- &id001
  dataset: Reddit
  rows:
  - model: Cluster-GCN (2019)
    model_key: node sampled soup
    model_plain: Cluster-GCN (2019)
    value: 0.9728
    std: 0.0008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_display: Jun 2023
    date_iso: '2023-06-18'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/VITA-Group/graph_ladling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9728
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Cluster-GCN (2019)
    model_key: engcn
    model_plain: Cluster-GCN (2019)
    value: 0.9714
    std: 0.0003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9714
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cluster-GCN (2019)
    model_key: sagn+sle
    model_plain: Cluster-GCN (2019)
    value: 0.971
    std: 0.0
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.971
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.961
    std: 0.001
    paper_value: 0.961
    paper_std: 0.001
    metric: F1
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.961
    true_std: 0.001
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.961
    sort_std: 0.001
    global_rank: 41
    paper_rank: 41
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
    value: 0.958
    std: 0.004
    paper_value: 0.958
    paper_std: 0.004
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.9601
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.0020999999999999908
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9601
    true_std: 0.0008
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.0020999999999999908
    has_value_note: false
    value_note: ''
    sort_value: 0.9601
    sort_std: 0.0008
    global_rank: 44
    paper_rank: 49
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.954
    std: 0.001
    paper_value: 0.954
    paper_std: 0.001
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.954
    true_std: 0.001
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.954
    sort_std: 0.001
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEEGERA
    model_key: seegera
    model_plain: SEEGERA
    value: 0.952
    std: 0.002
    paper_value: 0.952
    paper_std: 0.002
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.952
    true_std: 0.002
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.002
    global_rank: 71
    paper_rank: 71
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
    value: 0.951
    std: 0.001
    paper_value: 0.951
    paper_std: 0.001
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.9511
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9511
    true_std: 0.0018
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.9511
    sort_std: 0.0018
    global_rank: 75
    paper_rank: 75
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
    value: 0.947
    std: 0.001
    paper_value: 0.947
    paper_std: 0.001
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.9501
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0030999999999999917
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9501
    true_std: 0.0036
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.0030999999999999917
    has_value_note: false
    value_note: ''
    sort_value: 0.9501
    sort_std: 0.0036
    global_rank: 79
    paper_rank: 88
    rank_delta: 9
    rank_delta_abs: 9
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
    value: 0.942
    std: 0.001
    paper_value: 0.942
    paper_std: 0.001
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.949
    at_pub_std: 0.04
    at_pub_source_arxiv: '2208.10493'
    at_pub_source_title: Relational Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-08-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9431
    true_std: 0.0023
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.001100000000000101
    has_value_note: false
    value_note: ''
    sort_value: 0.9431
    sort_std: 0.0023
    global_rank: 94
    paper_rank: 97
    rank_delta: 3
    rank_delta_abs: 3
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
    value: 0.94
    std: 0.001
    paper_value: 0.94
    paper_std: 0.001
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
    protocol_note: Micro-F1 reported for Reddit
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.9414
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2101.11525'
    at_pub_source_title: Calibrating and Improving Graph Contrastive Learning
    at_pub_source_date_iso: '2021-01-27'
    at_pub_source_date_label: TMLR 2021
    value_gap_source_date_iso: '2021-01-27'
    value_gap_source_date_label: TMLR 2021
    gap_vs_at_pub: 0.0014000000000000679
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9414
    true_std: 0.0003
    value_gap_source_arxiv: '2101.11525'
    value_gap_source_title: Calibrating and Improving Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0014000000000000679
    has_value_note: false
    value_note: ''
    sort_value: 0.9414
    sort_std: 0.0003
    global_rank: 100
    paper_rank: 103
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Calibrating and Improving Graph Contrastive Learning
    comparison_source_arxiv: '2101.11525'
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
  dataset: WikiCS
  rows:
  - model: GPM
    model_key: gcn
    model_plain: GPM
    value: 0.9302
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
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9302
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.68
    std: 0.007
    paper_value: 0.68
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8014
    at_pub_std: 0.48
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2025-06-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.12139999999999995
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
    value_gap: 0.12139999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0048
    global_rank: 55
    paper_rank: 226
    rank_delta: 171
    rank_delta_abs: 171
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
    value: 0.655
    std: 0.015
    paper_value: 0.655
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.8
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.14500000000000002
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
    value_gap: 0.14500000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.001
    global_rank: 61
    paper_rank: 247
    rank_delta: 186
    rank_delta_abs: 186
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.706
    std: 0.009
    paper_value: 0.706
    paper_std: 0.009
    metric: Accuracy
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7992
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-05'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.09320000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7992
    true_std: 0.0068
    value_gap_source_arxiv: '2312.02619'
    value_gap_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    value_gap_source_is_current_paper: false
    value_gap: 0.09320000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7992
    sort_std: 0.0068
    global_rank: 65
    paper_rank: 210
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    comparison_source_arxiv: '2312.02619'
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.674
    std: 0.009
    paper_value: 0.674
    paper_std: 0.009
    metric: Accuracy
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7908
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1167999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7908
    true_std: 0.0053
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1167999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7908
    sort_std: 0.0053
    global_rank: 80
    paper_rank: 230
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    comparison_source_arxiv: '2312.02619'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.648
    std: 0.006
    paper_value: 0.648
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.754
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10599999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.13449999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7825
    sort_std: 0.0056
    global_rank: 120
    paper_rank: 249
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.648
    std: 0.007
    paper_value: 0.648
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: 0.7752
    at_pub_std: 0.08
    at_pub_source_arxiv: '2106.02466'
    at_pub_source_title: 'Graph Barlow Twins: A self-supervised representation learning
      framework for graphs'
    at_pub_source_date_iso: '2021-06-04'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12719999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7757
    true_std: 0.0046
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.12769999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.7757
    sort_std: 0.0046
    global_rank: 141
    paper_rank: 249
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Barlow Twins: A self-supervised representation
      learning framework for graphs'
    comparison_source_arxiv: '2106.02466'
    is_best: false
    is_std_outlier: false
  - model: AUG-MAE
    model_key: aug-mae
    model_plain: AUG-MAE
    value: 0.717
    std: 0.006
    paper_value: 0.717
    paper_std: 0.006
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.717
    true_std: 0.006
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.717
    sort_std: 0.006
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
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.66
    std: 0.002
    paper_value: 0.66
    paper_std: 0.002
    metric: Accuracy
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.66
    true_std: 0.002
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.66
    sort_std: 0.002
    global_rank: 243
    paper_rank: 243
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEEGERA
    model_key: seegera
    model_plain: SEEGERA
    value: 0.658
    std: 0.002
    paper_value: 0.658
    paper_std: 0.002
    metric: Accuracy
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
    protocol_note: Accuracy reported for WikiCS as per caption.
    date: Feb 11, 2024
    date_display: Feb 2024
    date_iso: '2024-02-11'
    published_venue: AAAI 2024
    published_conference: AAAI 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-11'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.658
    true_std: 0.002
    value_gap_source_arxiv: '2402.07225'
    value_gap_source_title: Rethinking Graph Masked Autoencoders through Alignment
      and Uniformity
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.658
    sort_std: 0.002
    global_rank: 244
    paper_rank: 244
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
- benchmark: TU Dortmund
  datasets:
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
    - dataset: WikiCS
      dataset_slug: wikics
    - dataset: PPI
      dataset_slug: ppi
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: COLLAB
      dataset_slug: collab
single_proposed_model: AUG-MAE
main_figure: /figures/2402.07225/main_figure.jpegoptim.jpg
---

