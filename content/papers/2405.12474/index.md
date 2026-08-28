---
title: 'How Universal Polynomial Bases Enhance Spectral Graph Neural Networks: Heterophily,
  Over-smoothing, and Over-squashing'
arxiv_id: '2405.12474'
source_url: ''
authors:
- name: Keke Huang
  orcid: null
  s2_author_id: '2269122908'
  s2_url: null
- name: Yu Guang Wang
  orcid: null
  s2_author_id: '2266362030'
  s2_url: null
- name: Ming Li
  orcid: null
  s2_author_id: '2150654801'
  s2_url: null
- name: Pietro Liò
  orcid: null
  s2_author_id: '2266237603'
  s2_url: null
published_date: May 21, 2024
published_date_iso: '2024-05-21'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: Spectral Graph Neural Networks (GNNs), alternatively known as graph filters,
  have gained increasing prevalence for heterophily graphs. Optimal graph filters
  rely on Laplacian eigendecomposition for Fourier transform. In an attempt to avert
  prohibitive computations, numerous polynomial filters have been proposed. However,
  polynomials in the majority of these filters are predefined and remain fixed across
  different graphs, failing to accommodate the varying degrees of heterophily. Addressing
  this gap, we demystify the intrinsic correlation between the spectral property of
  desired polynomial bases and the heterophily degrees via thorough theoretical analyses.
  Subsequently, we develop a novel adaptive heterophily basis wherein the basis vectors
  mutually form angles reflecting the heterophily degree of the graph. We integrate
  this heterophily basis with the homophily basis to construct a universal polynomial
  basis UniBasis, which devises a polynomial filter based graph neural network - UniFilter.
  It optimizes the convolution and propagation in GNN, thus effectively limiting over-smoothing
  and alleviating over-squashing. Our extensive experiments, conducted on a diverse
  range of real-world and synthetic datasets with varying degrees of heterophily,
  support the superiority of UniFilter. These results not only demonstrate the universality
  of UniBasis but also highlight its proficiency in graph explanation.
codebase_url: https://github.com/kkhuang81/UniFilter
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- UniFilter
mrr: 0.0318
adjusted_mrr: 0.0318
mrr_dataset_count: 4
benchmark_categories:
- Classic
- Heterophilic Graphs
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
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
- &id004
  dataset: Actor
  rows:
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
    global_rank: 1
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 2
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
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
    is_best: true
    is_std_outlier: false
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.4239
    std: 0.0052
    paper_value: 0.4239
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: GuoW23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4239
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2302.12432'
    at_pub_source_title: Graph Neural Networks with Learnable and Optimal Polynomial
      Bases
    at_pub_source_date_iso: '2023-02-24'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4239
    true_std: 0.0052
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4239
    sort_std: 0.0052
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.3628
    std: 0.0109
    paper_value: 0.3628
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: LuanHLZZZCP22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.366
    at_pub_std: 0.01
    at_pub_source_arxiv: '2205.13700'
    at_pub_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    at_pub_source_date_iso: '2022-05-27'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0031999999999999806
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4198
    true_std: 0.0089
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.056999999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.4198
    sort_std: 0.0089
    global_rank: 19
    paper_rank: 206
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.4193
    std: 0.0104
    paper_value: 0.4193
    paper_std: 0.0104
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: BoSWL23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4193
    at_pub_std: 0.0104
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4193
    true_std: 0.0104
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4193
    sort_std: 0.0104
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.4171
    std: 0.0112
    paper_value: 0.4171
    paper_std: 0.0112
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: he2021bernnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4179
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2303.13750'
    at_pub_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    at_pub_source_date_iso: '2023-03-24'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0007999999999999674
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4179
    true_std: 0.0101
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.0007999999999999674
    has_value_note: false
    value_note: ''
    sort_value: 0.4179
    sort_std: 0.0101
    global_rank: 25
    paper_rank: 27
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.4175
    std: 0.0107
    paper_value: 0.4175
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: HeWW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4175
    at_pub_std: 0.0107
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4175
    true_std: 0.0107
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4175
    sort_std: 0.0107
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.4122
    std: 0.0096
    paper_value: 0.4122
    paper_std: 0.0096
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4122
    at_pub_std: 0.0096
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4122
    true_std: 0.0096
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4122
    sort_std: 0.0096
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.4117
    std: 0.0064
    paper_value: 0.4117
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: WangZ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4117
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2302.12432'
    at_pub_source_title: Graph Neural Networks with Learnable and Optimal Polynomial
      Bases
    at_pub_source_date_iso: '2023-02-24'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4117
    true_std: 0.0064
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4117
    sort_std: 0.0064
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
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.4084
    std: 0.0121
    paper_value: 0.4084
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4084
    at_pub_std: 0.0121
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4084
    true_std: 0.0121
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4084
    sort_std: 0.0121
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.3744
    std: 0.013
    paper_value: 0.3744
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: ChenWHDL20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3861
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.011699999999999988
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4082
    true_std: 0.0179
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.0338
    has_value_note: false
    value_note: ''
    sort_value: 0.4082
    sort_std: 0.0179
    global_rank: 47
    paper_rank: 135
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.4036
    std: 0.0065
    paper_value: 0.4036
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: LeiWLDW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4048
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2403.03676'
    at_pub_source_title: Simplified PCNet with Robustness
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0011999999999999789
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4048
    true_std: 0.0062
    value_gap_source_arxiv: '2403.03676'
    value_gap_source_title: Simplified PCNet with Robustness
    value_gap_source_is_current_paper: false
    value_gap: 0.0011999999999999789
    has_value_note: false
    value_note: ''
    sort_value: 0.4048
    sort_std: 0.0062
    global_rank: 51
    paper_rank: 53
    rank_delta: 2
    rank_delta_abs: 2
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
    global_rank: 54
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.3991
    std: 0.0062
    paper_value: 0.3991
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: ChienP0M21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3991
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3992
    true_std: 0.0067
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.3992
    sort_std: 0.0067
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.377
    std: 0.014
    paper_value: 0.377
    paper_std: 0.014
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: LiZCSLLQ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3959
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.018899999999999972
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3959
    true_std: 0.0029
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.018899999999999972
    has_value_note: false
    value_note: ''
    sort_value: 0.3959
    sort_std: 0.0029
    global_rank: 73
    paper_rank: 124
    rank_delta: 51
    rank_delta_abs: 51
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
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
    global_rank: 86
    sort_value: 0.3899
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.3653
    std: 0.0077
    paper_value: 0.3653
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: SureshBNLM21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.386
    at_pub_std: 0.011
    at_pub_source_arxiv: '2205.13700'
    at_pub_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    at_pub_source_date_iso: '2022-05-27'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.020699999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.386
    true_std: 0.011
    value_gap_source_arxiv: '2205.13700'
    value_gap_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    value_gap_source_is_current_paper: false
    value_gap: 0.020699999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.386
    sort_std: 0.011
    global_rank: 93
    paper_rank: 190
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    comparison_source_arxiv: '2205.13700'
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.3742
    std: 0.0058
    paper_value: 0.3742
    paper_std: 0.0058
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: DefferrardBV16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3802
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.3802
    true_std: 0.0023
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.3802
    sort_std: 0.0023
    global_rank: 106
    paper_rank: 136
    rank_delta: 30
    rank_delta_abs: 30
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
    value: 0.2732
    std: 0.011
    paper_value: 0.2732
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: KipfW17
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.369
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.0958
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
    value_gap: 0.0958
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 164
    paper_rank: 463
    rank_delta: 299
    rank_delta_abs: 299
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.3222
    std: 0.0234
    paper_value: 0.3222
    paper_std: 0.0234
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: AbuElHaijaPKA19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3648
    at_pub_std: 0.012
    at_pub_source_arxiv: '2306.02376'
    at_pub_source_title: 'Towards Deep Attention in Graph Neural Networks: Problems
      and Remedies'
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.04260000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3648
    true_std: 0.012
    value_gap_source_arxiv: '2306.02376'
    value_gap_source_title: 'Towards Deep Attention in Graph Neural Networks: Problems
      and Remedies'
    value_gap_source_is_current_paper: false
    value_gap: 0.04260000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3648
    sort_std: 0.012
    global_rank: 194
    paper_rank: 347
    rank_delta: 153
    rank_delta_abs: 153
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Deep Attention in Graph Neural Networks: Problems
      and Remedies'
    comparison_source_arxiv: '2306.02376'
    is_best: false
    is_std_outlier: false
  - model: H_2GCN
    model_key: h_2gcn
    model_plain: H_2GCN
    value: 0.357
    std: 0.01
    paper_value: 0.357
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3622
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.005200000000000038
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3622
    true_std: 0.0033
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.005200000000000038
    has_value_note: false
    value_note: ''
    sort_value: 0.3622
    sort_std: 0.0033
    global_rank: 209
    paper_rank: 237
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.361
    std: 0.0155
    paper_value: 0.361
    paper_std: 0.0155
    metric: Accuracy
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: lim2021large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.361
    at_pub_std: 0.0155
    at_pub_source_arxiv: '2210.00513'
    at_pub_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.361
    true_std: 0.0155
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.361
    sort_std: 0.0155
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.2744
    std: 0.0089
    paper_value: 0.2744
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
    feature_source_evidence: bag-of-words representations
    table_ref: Table 2
    source_ref: VelickovicCCRLB18
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (48/32/20
      for model-optimized methods as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3605
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.08610000000000001
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
    value_gap: 0.08610000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 216
    paper_rank: 461
    rank_delta: 245
    rank_delta_abs: 245
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.3446
    std: 0.0067
    paper_value: 0.3446
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: WuSZFYW19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.349
    at_pub_std: 0.007
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0043999999999999595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.349
    true_std: 0.007
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.0043999999999999595
    has_value_note: false
    value_note: ''
    sort_value: 0.349
    sort_std: 0.007
    global_rank: 279
    paper_rank: 296
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.3341
    std: 0.008
    paper_value: 0.3341
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
    input_feature_source: raw_features
    feature_source_evidence: bag-of-words representations
    table_ref: Table 1
    source_ref: ChanpuriyaM22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Actor dataset using standard split (60/20/20
      for polynomial filters as per text).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3341
    at_pub_std: 0.008
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3341
    true_std: 0.008
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3341
    sort_std: 0.008
    global_rank: 333
    paper_rank: 333
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
- &id005
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
    value: 0.6026
    std: 0.025
    paper_value: 0.6026
    paper_std: 0.025
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.665
    at_pub_std: 0.026
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-06-18'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.06240000000000001
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
    value_gap: 0.25339999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: null
    global_rank: 3
    paper_rank: 165
    rank_delta: 162
    rank_delta_abs: 162
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: true
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.6749
    std: 0.0138
    paper_value: 0.6749
    paper_std: 0.0138
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6978
    at_pub_std: 0.0197
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02289999999999992
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.783
    true_std: 0.006
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.10809999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.783
    sort_std: 0.006
    global_rank: 24
    paper_rank: 96
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.7575
    std: 0.0165
    paper_value: 0.7575
    paper_std: 0.0165
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7575
    at_pub_std: 0.0165
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7575
    true_std: 0.0165
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7575
    sort_std: 0.0165
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.6693
    std: 0.0185
    paper_value: 0.6693
    paper_std: 0.0185
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6693
    at_pub_std: 0.0185
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7476
    true_std: 0.022
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.07830000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7476
    sort_std: 0.022
    global_rank: 30
    paper_rank: 102
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.7472
    std: 0.0129
    paper_value: 0.7472
    paper_std: 0.0129
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7472
    at_pub_std: 0.0129
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7472
    true_std: 0.0129
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7472
    sort_std: 0.0129
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
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.7426
    std: 0.0074
    paper_value: 0.7426
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7426
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7426
    true_std: 0.0074
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7426
    sort_std: 0.0074
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
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.742
    std: 0.0103
    paper_value: 0.742
    paper_std: 0.0103
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.742
    at_pub_std: 0.0103
    at_pub_source_arxiv: '2205.11172'
    at_pub_source_title: How Powerful are Spectral Graph Neural Networks
    at_pub_source_date_iso: '2022-05-23'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.742
    true_std: 0.0103
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.742
    sort_std: 0.0103
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
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.7138
    std: 0.0106
    paper_value: 0.7138
    paper_std: 0.0106
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7138
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7138
    true_std: 0.0106
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7138
    sort_std: 0.0106
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.7137
    std: 0.0101
    paper_value: 0.7137
    paper_std: 0.0101
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7137
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7137
    true_std: 0.0101
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7137
    sort_std: 0.0101
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.7121
    std: 0.0184
    paper_value: 0.7121
    paper_std: 0.0184
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7121
    at_pub_std: 0.018
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7133
    true_std: 0.0242
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.0012000000000000899
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: 0.0242
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6482
    std: 0.0224
    paper_value: 0.6482
    paper_std: 0.0224
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7033
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05510000000000004
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
    value_gap: 0.05510000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7033
    sort_std: null
    global_rank: 69
    paper_rank: 123
    rank_delta: 54
    rank_delta_abs: 54
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.6853
    std: 0.0168
    paper_value: 0.6853
    paper_std: 0.0168
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6853
    at_pub_std: 0.0168
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6853
    true_std: 0.0168
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6853
    sort_std: 0.0168
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.6842
    std: 0.0138
    paper_value: 0.6842
    paper_std: 0.0138
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6842
    at_pub_std: 0.014
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6842
    true_std: 0.0132
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6842
    sort_std: 0.0132
    global_rank: 87
    paper_rank: 87
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4481
    std: 0.012
    paper_value: 0.4481
    paper_std: 0.012
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split (implied by context
      of heterophily benchmark).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.671
    at_pub_std: 0.029
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.22290000000000004
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
    value_gap: 0.22290000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.671
    sort_std: 0.029
    global_rank: 101
    paper_rank: 273
    rank_delta: 172
    rank_delta_abs: 172
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.6702
    std: 0.0177
    paper_value: 0.6702
    paper_std: 0.0177
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6702
    at_pub_std: 0.0177
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6702
    true_std: 0.0177
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6702
    sort_std: 0.0177
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.6524
    std: 0.0087
    paper_value: 0.6524
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6524
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2111.06748'
    at_pub_source_title: Simplifying approach to Node Classification in Graph Neural
      Networks
    at_pub_source_date_iso: '2021-11-12'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6524
    true_std: 0.0087
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6524
    sort_std: 0.0087
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.6386
    std: 0.0304
    paper_value: 0.6386
    paper_std: 0.0304
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6386
    at_pub_std: 0.03
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6386
    true_std: 0.0304
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6386
    sort_std: 0.0304
    global_rank: 132
    paper_rank: 132
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
  - model: H_2GCN
    model_key: h_2gcn
    model_plain: H_2GCN
    value: 0.6011
    std: 0.0215
    paper_value: 0.6011
    paper_std: 0.0215
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.612
    at_pub_std: 0.0095
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.01090000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.612
    true_std: 0.0095
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.01090000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.612
    sort_std: 0.0095
    global_rank: 151
    paper_rank: 168
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.6092
    std: 0.0145
    paper_value: 0.6092
    paper_std: 0.0145
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6092
    at_pub_std: 0.0145
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6092
    true_std: 0.0145
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6092
    sort_std: 0.0145
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.605
    std: 0.0253
    paper_value: 0.605
    paper_std: 0.0253
    metric: Accuracy
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
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.605
    at_pub_std: 0.0253
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.605
    true_std: 0.0253
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.605
    sort_std: 0.0253
    global_rank: 161
    paper_rank: 161
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.5951
    std: 0.0125
    paper_value: 0.5951
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5951
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5951
    true_std: 0.0125
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5951
    sort_std: 0.0125
    global_rank: 172
    paper_rank: 172
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
    value: 0.5429
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 208
    sort_value: 0.5429
    sort_std: null
    comparison_type: global_top
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
    value: 0.765
    std: 0.0136
    paper_value: 0.765
    paper_std: 0.0136
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: KipfW17
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8769
    at_pub_std: 0.004
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1119
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
    value_gap: 0.1119
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 155
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8008
    std: 0.0075
    paper_value: 0.8008
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: he2021bernnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8766
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.07580000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8766
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07580000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8766
    sort_std: 0.0026
    global_rank: 22
    paper_rank: 63
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.8149
    std: 0.0094
    paper_value: 0.8149
    paper_std: 0.0094
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: BoSWL23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8149
    at_pub_std: 0.0094
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8149
    true_std: 0.0094
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8149
    sort_std: 0.0094
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
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.8139
    std: 0.0132
    paper_value: 0.8139
    paper_std: 0.0132
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8139
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8139
    true_std: 0.0132
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8139
    sort_std: 0.0132
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7655
    std: 0.0123
    paper_value: 0.7655
    paper_std: 0.0123
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: VelickovicCCRLB18
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.808
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.04250000000000009
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
    value_gap: 0.04250000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 154
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.8078
    std: 0.0079
    paper_value: 0.8078
    paper_std: 0.0079
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: WangZ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8078
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8078
    true_std: 0.0079
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8078
    sort_std: 0.0079
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
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7733
    std: 0.0148
    paper_value: 0.7733
    paper_std: 0.0148
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: ChenWHDL20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8076
    at_pub_std: 0.003
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.0343
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8076
    true_std: 0.003
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0343
    has_value_note: false
    value_note: ''
    sort_value: 0.8076
    sort_std: 0.003
    global_rank: 48
    paper_rank: 130
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.8058
    std: 0.0082
    paper_value: 0.8058
    paper_std: 0.0082
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: GuoW23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8058
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8058
    true_std: 0.0082
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8058
    sort_std: 0.0082
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
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8053
    std: 0.0079
    paper_value: 0.8053
    paper_std: 0.0079
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: HeWW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8053
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8053
    true_std: 0.0079
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8053
    sort_std: 0.0079
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
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.8014
    std: 0.0087
    paper_value: 0.8014
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8014
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8014
    true_std: 0.0087
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0087
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8013
    std: 0.0084
    paper_value: 0.8013
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: ChienP0M21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8013
    at_pub_std: 0.0084
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8013
    true_std: 0.0084
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8013
    sort_std: 0.0084
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7965
    std: 0.0102
    paper_value: 0.7965
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: WuSZFYW19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (implied by citation network context and standard benchmark usage).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7965
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7965
    true_std: 0.0102
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0102
    global_rank: 68
    paper_rank: 68
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.7933
    std: 0.0057
    paper_value: 0.7933
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: DefferrardBV16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7933
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7933
    true_std: 0.0057
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0057
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.7851
    std: 0.0063
    paper_value: 0.7851
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: LeiWLDW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7851
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7851
    true_std: 0.0063
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7851
    sort_std: 0.0063
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
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.7722
    std: 0.0178
    paper_value: 0.7722
    paper_std: 0.0178
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: LiZCSLLQ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.774
    at_pub_std: 0.017
    at_pub_source_arxiv: '2303.06344'
    at_pub_source_title: Graph Contrastive Learning under Heterophily via Graph Filters
    at_pub_source_date_iso: '2023-03-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0018000000000000238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.774
    true_std: 0.017
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.0018000000000000238
    has_value_note: false
    value_note: ''
    sort_value: 0.774
    sort_std: 0.017
    global_rank: 128
    paper_rank: 134
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.7732
    std: 0.017
    paper_value: 0.7732
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: LuanHLZZZCP22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7732
    at_pub_std: 0.017
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7732
    true_std: 0.017
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7732
    sort_std: 0.017
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.7711
    std: 0.0157
    paper_value: 0.7711
    paper_std: 0.0157
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: ZhuYZHAK20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7711
    at_pub_std: null
    at_pub_source_arxiv: '2206.14418'
    at_pub_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    at_pub_source_date_iso: '2022-06-29'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7711
    true_std: 0.0157
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7711
    sort_std: 0.0157
    global_rank: 142
    paper_rank: 142
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.7681
    std: 0.0189
    paper_value: 0.7681
    paper_std: 0.0189
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: SureshBNLM21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7681
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7681
    true_std: 0.0189
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7681
    sort_std: 0.0189
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
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.7652
    std: 0.0036
    paper_value: 0.7652
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: ChanpuriyaM22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7652
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7652
    true_std: 0.0036
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7652
    sort_std: 0.0036
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.7626
    std: 0.0133
    paper_value: 0.7626
    paper_std: 0.0133
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: AbuElHaijaPKA19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7626
    at_pub_std: 0.0133
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7626
    true_std: 0.0295
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7626
    sort_std: 0.0295
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
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.7319
    std: 0.0099
    paper_value: 0.7319
    paper_std: 0.0099
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: lim2021large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.7319
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7319
    true_std: 0.0099
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7319
    sort_std: 0.0099
    global_rank: 362
    paper_rank: 362
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
    value: 0.7289
    std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 401
    sort_value: 0.7289
    sort_std: 0.001
    comparison_type: global_top
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
    value: 0.8698
    std: 0.0127
    paper_value: 0.8698
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.03059999999999996
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
    value_gap: 0.03059999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 192
    rank_delta: 161
    rank_delta_abs: 161
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8851
    std: 0.0092
    paper_value: 0.8851
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8976
    at_pub_std: 0.016
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.012499999999999956
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8976
    true_std: 0.016
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.012499999999999956
    has_value_note: false
    value_note: ''
    sort_value: 0.8976
    sort_std: 0.016
    global_rank: 37
    paper_rank: 93
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.8791
    std: 0.0095
    paper_value: 0.8791
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8975
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.018399999999999972
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8975
    true_std: 0.0116
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.018399999999999972
    has_value_note: false
    value_note: ''
    sort_value: 0.8975
    sort_std: 0.0116
    global_rank: 38
    paper_rank: 137
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.8949
    std: 0.0135
    paper_value: 0.8949
    paper_std: 0.0135
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8949
    at_pub_std: 0.0135
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8949
    true_std: 0.0135
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8949
    sort_std: 0.0135
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
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8871
    std: 0.0093
    paper_value: 0.8871
    paper_std: 0.0093
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8932
    at_pub_std: 0.011
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8932
    true_std: 0.011
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.006099999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8932
    sort_std: 0.011
    global_rank: 53
    paper_rank: 80
    rank_delta: 27
    rank_delta_abs: 27
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
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.8898
    std: 0.0072
    paper_value: 0.8898
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8898
    at_pub_std: 0.007
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8898
    true_std: 0.0072
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8898
    sort_std: 0.0072
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.873
    std: 0.011
    paper_value: 0.873
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.016700000000000048
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 168
    rank_delta: 101
    rank_delta_abs: 101
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.8837
    std: 0.0125
    paper_value: 0.8837
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8893
    at_pub_std: 0.0137
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.005599999999999938
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8893
    true_std: 0.0137
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.005599999999999938
    has_value_note: false
    value_note: ''
    sort_value: 0.8893
    sort_std: 0.0137
    global_rank: 69
    paper_rank: 101
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.8857
    std: 0.0101
    paper_value: 0.8857
    paper_std: 0.0101
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8857
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8857
    true_std: 0.0101
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8857
    sort_std: 0.0101
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8854
    std: 0.0067
    paper_value: 0.8854
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8854
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8854
    true_std: 0.0067
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8854
    sort_std: 0.0067
    global_rank: 92
    paper_rank: 92
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.8833
    std: 0.0109
    paper_value: 0.8833
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8853
    at_pub_std: 0.012
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8853
    true_std: 0.012
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.8853
    sort_std: 0.012
    global_rank: 93
    paper_rank: 103
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.8732
    std: 0.0092
    paper_value: 0.8732
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8832
    at_pub_std: 0.02
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8832
    true_std: 0.02
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.02
    global_rank: 104
    paper_rank: 168
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.882
    std: 0.0226
    paper_value: 0.882
    paper_std: 0.0226
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.882
    at_pub_std: 0.0226
    at_pub_source_arxiv: '2307.16026'
    at_pub_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.882
    true_std: 0.0226
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.882
    sort_std: 0.0226
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H_2GCN
    model_key: h_2gcn
    model_plain: H_2GCN
    value: 0.8787
    std: 0.012
    paper_value: 0.8787
    paper_std: 0.012
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8787
    true_std: 0.012
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8787
    sort_std: 0.012
    global_rank: 141
    paper_rank: 141
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.8761
    std: 0.0085
    paper_value: 0.8761
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8781
    at_pub_std: 0.017
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8781
    true_std: 0.017
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.8781
    sort_std: 0.017
    global_rank: 144
    paper_rank: 150
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.8777
    std: 0.0067
    paper_value: 0.8777
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8777
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8777
    true_std: 0.0067
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8777
    sort_std: 0.0067
    global_rank: 147
    paper_rank: 147
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.877
    std: 0.0069
    paper_value: 0.877
    paper_std: 0.0069
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.877
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.877
    true_std: 0.0069
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: 0.0069
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.87
    std: 0.0155
    paper_value: 0.87
    paper_std: 0.0155
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.87
    at_pub_std: 0.0155
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.87
    true_std: 0.0155
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.87
    sort_std: 0.0155
    global_rank: 191
    paper_rank: 191
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8683
    std: 0.0128
    paper_value: 0.8683
    paper_std: 0.0128
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8683
    true_std: 0.0128
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8683
    sort_std: 0.0128
    global_rank: 202
    paper_rank: 202
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.8535
    std: 0.0098
    paper_value: 0.8535
    paper_std: 0.0098
    metric: Accuracy
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
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8535
    at_pub_std: 0.0098
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8535
    true_std: 0.0098
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8535
    sort_std: 0.0098
    global_rank: 270
    paper_rank: 270
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.8464
    std: 0.0113
    paper_value: 0.8464
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora node classification using Planetoid split (20-per-class train
      split).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8464
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8464
    true_std: 0.0113
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8464
    sort_std: 0.0113
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7768
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 806
    sort_value: 0.7768
    sort_std: null
    comparison_type: global_top
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
  dataset: Penn94
  rows:
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.8762
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    venue: null
    codebase_url: https://github.com/jianhao2016/GPRGNN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8762
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.8669
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16185'
    title: Differentiable Cluster Graph Neural Network
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8669
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M2M-GNN
    model_key: m2m-gnn
    model_plain: M2M-GNN
    value: 0.8594
    std: 0.004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8594
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8486
    std: 0.0033
    paper_value: 0.8486
    paper_std: 0.0033
    metric: Accuracy
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8522
    at_pub_std: 0.003
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8522
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.0035999999999999366
    has_value_note: false
    value_note: ''
    sort_value: 0.8522
    sort_std: 0.003
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
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.8485
    std: 0.0039
    paper_value: 0.8485
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8485
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2302.12432'
    at_pub_source_title: Graph Neural Networks with Learnable and Optimal Polynomial
      Bases
    at_pub_source_date_iso: '2023-02-24'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-06-03'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8485
    true_std: 0.004
    value_gap_source_arxiv: '2406.01249'
    value_gap_source_title: Equivariant Machine Learning on Graphs with Nonlinear
      Spectral Filters
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8485
    sort_std: 0.004
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
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.8446
    std: 0.0033
    paper_value: 0.8446
    paper_std: 0.0033
    metric: Accuracy
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8446
    true_std: 0.0033
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8446
    sort_std: 0.0033
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8354
    std: 0.0032
    paper_value: 0.8354
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8354
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8354
    true_std: 0.0032
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8354
    sort_std: 0.0032
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8326
    std: 0.0029
    paper_value: 0.8326
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8326
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-06-03'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8326
    true_std: 0.003
    value_gap_source_arxiv: '2406.01249'
    value_gap_source_title: Equivariant Machine Learning on Graphs with Nonlinear
      Spectral Filters
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8326
    sort_std: 0.003
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8247
    std: 0.0027
    paper_value: 0.8247
    paper_std: 0.0027
    metric: Accuracy
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8323
    at_pub_std: 0.002
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007600000000000051
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8323
    true_std: 0.002
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.007600000000000051
    has_value_note: false
    value_note: ''
    sort_value: 0.8323
    sort_std: 0.002
    global_rank: 30
    paper_rank: 37
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8268
    std: 0.0032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_display: Nov 2023
    date_iso: '2023-11-09'
    venue: Accepted for publication in ICLR 2024
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 36
    sort_value: 0.8268
    sort_std: 0.0032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.8259
    std: 0.0031
    paper_value: 0.8259
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8263
    at_pub_std: 0.003
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8263
    true_std: 0.003
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000006697
    has_value_note: false
    value_note: ''
    sort_value: 0.8263
    sort_std: 0.003
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.8213
    std: 0.0028
    paper_value: 0.8213
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8213
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2403.07954'
    at_pub_source_title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov
      Subspace Approach'
    at_pub_source_date_iso: '2024-03-12'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8213
    true_std: 0.0028
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8213
    sort_std: 0.0028
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8144
    std: 0.0015
    paper_value: 0.8144
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
    protocol_note: Accuracy on Penn94 test split
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8144
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2403.07954'
    at_pub_source_title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov
      Subspace Approach'
    at_pub_source_date_iso: '2024-03-12'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8144
    true_std: 0.0015
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8144
    sort_std: 0.0015
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7534
    std: 0.0064
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 60
    sort_value: 0.7534
    sort_std: 0.0064
    comparison_type: global_top
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8949
    std: 0.0038
    paper_value: 0.8949
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: ZhuYZHAK20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8959
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2307.16026'
    at_pub_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9361
    true_std: 0.0013
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.041200000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: 0.0013
    global_rank: 16
    paper_rank: 107
    rank_delta: 91
    rank_delta_abs: 91
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
    value: 0.8842
    std: 0.005
    paper_value: 0.8842
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: KipfW17
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.012800000000000034
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
    value_gap: 0.045399999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 157
    rank_delta: 138
    rank_delta_abs: 138
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
    value: 0.8633
    std: 0.0048
    paper_value: 0.8633
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: VelickovicCCRLB18
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.03370000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: 0.0018
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.06000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 259
    rank_delta: 236
    rank_delta_abs: 236
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.9144
    std: 0.005
    paper_value: 0.9144
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.9144
    at_pub_std: 0.005
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9144
    true_std: 0.005
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9144
    sort_std: 0.005
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
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.9
    std: 0.0052
    paper_value: 0.9
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: LuanHLZZZCP22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.9096
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.009599999999999942
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9096
    true_std: 0.0062
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.009599999999999942
    has_value_note: false
    value_note: ''
    sort_value: 0.9096
    sort_std: 0.0062
    global_rank: 47
    paper_rank: 86
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.9087
    std: 0.0034
    paper_value: 0.9087
    paper_std: 0.0034
    metric: Accuracy
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: LeiWLDW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.9087
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9087
    true_std: 0.0034
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9087
    sort_std: 0.0034
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
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.903
    std: 0.0019
    paper_value: 0.903
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: GuoW23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.903
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.0019
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.0019
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.9015
    std: 0.0043
    paper_value: 0.9015
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: ChenWHDL20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.903
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0015000000000000568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.0043
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: 0.0015000000000000568
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.0043
    global_rank: 68
    paper_rank: 78
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.8531
    std: 0.0061
    paper_value: 0.8531
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: AbuElHaijaPKA19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.9004
    at_pub_std: 0.0141
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04730000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: 0.0141
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.04730000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: 0.0141
    global_rank: 85
    paper_rank: 283
    rank_delta: 198
    rank_delta_abs: 198
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.8962
    std: 0.0041
    paper_value: 0.8962
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: WangZ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8962
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8962
    true_std: 0.0041
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8962
    sort_std: 0.0041
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
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.8924
    std: 0.0039
    paper_value: 0.8924
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: LiZCSLLQ22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.896
    at_pub_std: 0.004
    at_pub_source_arxiv: '2303.06344'
    at_pub_source_title: Graph Contrastive Learning under Heterophily via Graph Filters
    at_pub_source_date_iso: '2023-03-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0036000000000000476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.896
    true_std: 0.004
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.0036000000000000476
    has_value_note: false
    value_note: ''
    sort_value: 0.896
    sort_std: 0.004
    global_rank: 106
    paper_rank: 117
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.8773
    std: 0.0058
    paper_value: 0.8773
    paper_std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: BoSWL23
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8874
    at_pub_std: 0.002
    at_pub_source_arxiv: '2404.15354'
    at_pub_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.010099999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8947
    true_std: 0.0048
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.017400000000000082
    has_value_note: false
    value_note: ''
    sort_value: 0.8947
    sort_std: 0.0048
    global_rank: 109
    paper_rank: 197
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    comparison_source_arxiv: '2404.15354'
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.8909
    std: 0.0043
    paper_value: 0.8909
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8909
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8909
    true_std: 0.0043
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8909
    sort_std: 0.0043
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
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8893
    std: 0.0029
    paper_value: 0.8893
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: HeWW22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8898
    at_pub_std: 0.004
    at_pub_source_arxiv: '2404.15354'
    at_pub_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8898
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: false
    value_gap: 0.000500000000000056
    has_value_note: false
    value_note: ''
    sort_value: 0.8898
    sort_std: 0.004
    global_rank: 130
    paper_rank: 131
    rank_delta: 1
    rank_delta_abs: 1
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
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.8852
    std: 0.0092
    paper_value: 0.8852
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: SureshBNLM21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8852
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8852
    true_std: 0.0092
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8852
    sort_std: 0.0092
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
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8851
    std: 0.0039
    paper_value: 0.8851
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: he2021bernnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8851
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8851
    true_std: 0.0039
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8851
    sort_std: 0.0039
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8846
    std: 0.0031
    paper_value: 0.8846
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: ChienP0M21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8846
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8846
    true_std: 0.0031
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8846
    sort_std: 0.0031
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8714
    std: 0.009
    paper_value: 0.8714
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: WuSZFYW19
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split
      (implied by citation network context).
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8714
    at_pub_std: 0.009
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.0055
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.011800000000000033
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.0055
    global_rank: 164
    paper_rank: 231
    rank_delta: 67
    rank_delta_abs: 67
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.8786
    std: 0.0077
    paper_value: 0.8786
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
    input_feature_source: raw_features
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 2
    source_ref: lim2021large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8786
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8786
    true_std: 0.0077
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8786
    sort_std: 0.0077
    global_rank: 187
    paper_rank: 187
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.8782
    std: 0.0024
    paper_value: 0.8782
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: DefferrardBV16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8782
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8782
    true_std: 0.0024
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8782
    sort_std: 0.0024
    global_rank: 190
    paper_rank: 190
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
    value: 0.869
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 243
    sort_value: 0.869
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.8417
    std: 0.0024
    paper_value: 0.8417
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
    feature_source_evidence: Feature vectors of nodes are bag-of-words representations.
    table_ref: Table 1
    source_ref: ChanpuriyaM22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using the standard Planetoid split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8417
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8417
    true_std: 0.0024
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8417
    sort_std: 0.0024
    global_rank: 314
    paper_rank: 314
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.5043
    std: 0.0189
    paper_value: 0.5043
    paper_std: 0.0189
    metric: Accuracy
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
    source_ref: Chien et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5043
    at_pub_std: 0.0189
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.748
    true_std: 0.005
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.24370000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.748
    sort_std: 0.005
    global_rank: 10
    paper_rank: 102
    rank_delta: 92
    rank_delta_abs: 92
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.5788
    std: 0.0176
    paper_value: 0.5788
    paper_std: 0.0176
    metric: Accuracy
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
    source_ref: Li et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5788
    at_pub_std: 0.018
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7121
    true_std: 0.0184
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7121
    sort_std: 0.0184
    global_rank: 19
    paper_rank: 62
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.674
    std: 0.0125
    paper_value: 0.674
    paper_std: 0.0125
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
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.674
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.674
    true_std: 0.0125
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.674
    sort_std: 0.0125
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
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.544
    std: 0.0188
    paper_value: 0.544
    paper_std: 0.0188
    metric: Accuracy
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
    source_ref: Luan et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.544
    at_pub_std: 0.0188
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.674
    true_std: 0.0221
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.13
    has_value_note: false
    value_note: ''
    sort_value: 0.674
    sort_std: 0.0221
    global_rank: 26
    paper_rank: 85
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.6464
    std: 0.0081
    paper_value: 0.6464
    paper_std: 0.0081
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Bo et al. 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6464
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6464
    true_std: 0.0081
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6464
    sort_std: 0.0081
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OptBasisGNN
    model_key: optbasisgnn
    model_plain: OptBasisGNN
    value: 0.6362
    std: 0.0076
    paper_value: 0.6362
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
    source_ref: Guo et al. 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6362
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6362
    true_std: 0.0076
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6362
    sort_std: 0.0076
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
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.6181
    std: 0.018
    paper_value: 0.6181
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: Lim et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6181
    at_pub_std: 0.018
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6181
    true_std: 0.018
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6181
    sort_std: 0.018
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5343
    std: 0.0201
    paper_value: 0.5343
    paper_std: 0.0201
    metric: Accuracy
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
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.6067
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.07240000000000002
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
    value_gap: 0.07240000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6067
    sort_std: null
    global_rank: 51
    paper_rank: 90
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: ASGC
    model_key: asgc
    model_plain: ASGC
    value: 0.5791
    std: 0.0089
    paper_value: 0.5791
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
    table_ref: Table 1
    source_ref: Chanpuriya et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5791
    at_pub_std: 0.0089
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5791
    true_std: 0.0089
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5791
    sort_std: 0.0089
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.5772
    std: 0.0059
    paper_value: 0.5772
    paper_std: 0.0059
    metric: Accuracy
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
    source_ref: He et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5772
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5772
    true_std: 0.0059
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5772
    sort_std: 0.0059
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
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.5738
    std: 0.0125
    paper_value: 0.5738
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Wang et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5738
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2303.13750'
    at_pub_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    at_pub_source_date_iso: '2023-03-24'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5738
    true_std: 0.0125
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5738
    sort_std: 0.0125
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4072
    std: 0.0155
    paper_value: 0.4072
    paper_std: 0.0155
    metric: Accuracy
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
    source_ref: Veličković et al. 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.563
    at_pub_std: 0.022
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.15579999999999994
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
    value_gap: 0.15579999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.563
    sort_std: 0.022
    global_rank: 77
    paper_rank: 179
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: EvenNet
    model_key: evennet
    model_plain: EvenNet
    value: 0.5271
    std: 0.0085
    paper_value: 0.5271
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
    table_ref: Table 1
    source_ref: Lei et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.5271
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5271
    true_std: 0.0085
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5271
    sort_std: 0.0085
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
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.5139
    std: 0.0092
    paper_value: 0.5139
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
    table_ref: Table 1
    source_ref: He et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.526
    at_pub_std: 0.017
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0121
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.526
    true_std: 0.017
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.0121
    has_value_note: false
    value_note: ''
    sort_value: 0.526
    sort_std: 0.017
    global_rank: 95
    paper_rank: 99
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.2575
    std: 0.0107
    paper_value: 0.2575
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
    source_ref: Wu et al. 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.523
    at_pub_std: 0.023
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2655
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
    value_gap: 0.2655
    has_value_note: false
    value_note: ''
    sort_value: 0.523
    sort_std: 0.023
    global_rank: 96
    paper_rank: 301
    rank_delta: 205
    rank_delta_abs: 205
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.4885
    std: 0.0078
    paper_value: 0.4885
    paper_std: 0.0078
    metric: Accuracy
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
    source_ref: Suresh et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4885
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2111.06748'
    at_pub_source_title: Simplifying approach to Node Classification in Graph Neural
      Networks
    at_pub_source_date_iso: '2021-11-12'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4885
    true_std: 0.0078
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4885
    sort_std: 0.0078
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.4559
    std: 0.014
    paper_value: 0.4559
    paper_std: 0.014
    metric: Accuracy
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
    source_ref: Frasca et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4559
    at_pub_std: 0.014
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4559
    true_std: 0.014
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4559
    sort_std: 0.014
    global_rank: 129
    paper_rank: 129
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
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.4081
    std: 0.0042
    paper_value: 0.4081
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Defferrard et al. 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.4081
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4386
    true_std: 0.0164
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: 0.03049999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4386
    sort_std: 0.0164
    global_rank: 142
    paper_rank: 176
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.438
    std: 0.0148
    paper_value: 0.438
    paper_std: 0.0148
    metric: Accuracy
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
    source_ref: Abu-ElHaija et al. 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.438
    at_pub_std: 0.0148
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.438
    true_std: 0.0148
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.438
    sort_std: 0.0148
    global_rank: 144
    paper_rank: 144
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
    value: 0.393
    std: 0.0079
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 194
    sort_value: 0.393
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.3847
    std: 0.0158
    paper_value: 0.3847
    paper_std: 0.0158
    metric: Accuracy
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
    source_ref: Chen et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3847
    at_pub_std: 0.016
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3881
    true_std: 0.0197
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.003400000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.3881
    sort_std: 0.0197
    global_rank: 198
    paper_rank: 201
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H_2GCN
    model_key: h_2gcn
    model_plain: H_2GCN
    value: 0.3648
    std: 0.0186
    paper_value: 0.3648
    paper_std: 0.0186
    metric: Accuracy
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
    source_ref: Zhu et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Squirrel node classification using standard split.
    date: May 21, 2024
    date_display: May 2024
    date_iso: '2024-05-21'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.379
    at_pub_std: 0.02
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.01419999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.379
    true_std: 0.02
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.01419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.379
    sort_std: 0.02
    global_rank: 208
    paper_rank: 229
    rank_delta: 21
    rank_delta_abs: 21
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: Heterophilic Graphs
  datasets:
  - *id004
  - *id005
  - *id006
- benchmark: LINKX Benchmarks
  datasets:
  - *id007
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
    - dataset: Penn94
      dataset_slug: penn94
single_proposed_model: UniFilter
main_figure: /figures/2405.12474/main_figure.jpegoptim.jpg
---

