---
title: 'Beyond Smoothing: Unsupervised Graph Representation Learning with Edge Heterophily
  Discriminating'
arxiv_id: '2211.14065'
source_url: ''
authors:
- name: Yixin Liu
  orcid: null
  s2_author_id: '2116018493'
  s2_url: null
- name: Yizhen Zheng
  orcid: null
  s2_author_id: '26956796'
  s2_url: null
- name: Daokun Zhang
  orcid: null
  s2_author_id: '2589584'
  s2_url: null
- name: Vincent Lee
  orcid: null
  s2_author_id: '2187919914'
  s2_url: null
- name: Shirui Pan
  orcid: null
  s2_author_id: '2585415'
  s2_url: null
published_date: Nov 25, 2022
published_date_iso: '2022-11-25'
published_venue: AAAI 2022
published_conference: AAAI 2022
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Unsupervised graph representation learning (UGRL) has drawn increasing research
  attention and achieved promising results in several graph analytic tasks. Relying
  on the homophily assumption, existing UGRL methods tend to smooth the learned node
  representations along all edges, ignoring the existence of heterophilic edges that
  connect nodes with distinct attributes. As a result, current methods are hard to
  generalize to heterophilic graphs where dissimilar nodes are widely connected, and
  also vulnerable to adversarial attacks. To address this issue, we propose a novel
  unsupervised raph epresentation learning method with dge h terophily discrimina
  ing (GREET) which learns representations by discriminating and leveraging homophilic
  edges and heterophilic edges. To distinguish two types of edges, we build an edge
  discriminator that infers edge homophily/heterophily from feature and structure
  information. We train the edge discriminator in an unsupervised way through minimizing
  the crafted pivot-anchored ranking loss, with randomly sampled node pairs acting
  as pivots. Node representations are learned through contrasting the dual-channel
  encodings obtained from the discriminated homophilic and heterophilic edges. With
  an effective interplaying scheme, edge discriminating and representation learning
  can mutually boost each other during the training phase. We conducted extensive
  experiments on 14 benchmark datasets and multiple learning scenarios to demonstrate
  the superiority of GREET.
codebase_url: https://github.com/yixinliu233/GREET
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GREET
mrr: 0.0119
adjusted_mrr: 0.0119
mrr_dataset_count: 12
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 6
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 6
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id009
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.3566
    std: 0.0094
    paper_value: 0.3566
    paper_std: 0.0094
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4018
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-02-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04520000000000002
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
    value_gap: 0.04600000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.4026
    sort_std: 0.0108
    global_rank: 54
    paper_rank: 238
    rank_delta: 184
    rank_delta_abs: 184
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.3527
    std: 0.0104
    paper_value: 0.3527
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3991
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0464
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3992
    true_std: 0.0067
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: 0.046499999999999986
    has_value_note: false
    value_note: ''
    sort_value: 0.3992
    sort_std: 0.0067
    global_rank: 67
    paper_rank: 263
    rank_delta: 196
    rank_delta_abs: 196
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.3574
    std: 0.0062
    paper_value: 0.3574
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.397
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.039600000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.397
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.039600000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.397
    sort_std: null
    global_rank: 70
    paper_rank: 236
    rank_delta: 166
    rank_delta_abs: 166
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.3586
    std: 0.0103
    paper_value: 0.3586
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: zhu2020beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.384
    at_pub_std: 0.01
    at_pub_source_arxiv: '2205.13700'
    at_pub_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    at_pub_source_date_iso: '2022-05-27'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.025400000000000034
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3885
    true_std: 0.0117
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.029900000000000038
    has_value_note: false
    value_note: ''
    sort_value: 0.3885
    sort_std: 0.0117
    global_rank: 89
    paper_rank: 229
    rank_delta: 140
    rank_delta_abs: 140
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    comparison_source_arxiv: '2205.13700'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.3163
    std: null
    paper_value: 0.3163
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
    table_ref: Table 2
    source_ref: geom_pei2020geom
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.381
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.06469999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.381
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06469999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.381
    sort_std: null
    global_rank: 105
    paper_rank: 356
    rank_delta: 251
    rank_delta_abs: 251
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.3655
    std: 0.0101
    paper_value: 0.3655
    paper_std: 0.0101
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.3712
    true_std: 0.0067
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.005699999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.3712
    sort_std: 0.0067
    global_rank: 152
    paper_rank: 190
    rank_delta: 38
    rank_delta_abs: 38
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
    value: 0.3083
    std: 0.0077
    paper_value: 0.3083
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.369
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.060699999999999976
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
    value_gap: 0.060699999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 164
    paper_rank: 381
    rank_delta: 217
    rank_delta_abs: 217
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
    value: 0.2806
    std: 0.0148
    paper_value: 0.2806
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3605
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07989999999999997
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
    value_gap: 0.07989999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 216
    paper_rank: 452
    rank_delta: 236
    rank_delta_abs: 236
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3002
    std: 0.007
    paper_value: 0.3002
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
    table_ref: Table 2
    source_ref: hassani2020contrastive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3209
    at_pub_std: 0.0107
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.020699999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.04619999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.3464
    sort_std: 0.002
    global_rank: 291
    paper_rank: 405
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.2901
    std: 0.0078
    paper_value: 0.2901
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2827
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007400000000000018
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.345
    true_std: 0.011
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.05489999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.345
    sort_std: 0.011
    global_rank: 295
    paper_rank: 428
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.3255
    std: 0.0128
    paper_value: 0.3255
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3255
    true_std: 0.0128
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3255
    sort_std: 0.0128
    global_rank: 344
    paper_rank: 344
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
    value: 0.2982
    std: 0.0069
    paper_value: 0.2982
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: velivckovic2019deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.283
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.015200000000000047
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
    value_gap: 0.022699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3209
    sort_std: 0.0118
    global_rank: 350
    paper_rank: 410
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.2699
    std: 0.0156
    paper_value: 0.2699
    paper_std: 0.0156
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2843
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.014400000000000024
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
    value_gap: 0.04580000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3157
    sort_std: 0.0075
    global_rank: 360
    paper_rank: 466
    rank_delta: 106
    rank_delta_abs: 106
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
    value: 0.2782
    std: 0.009
    paper_value: 0.2782
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
    table_ref: Table 2
    source_ref: peng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2728
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.005400000000000016
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3011
    true_std: 0.0192
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.022899999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.3011
    sort_std: 0.0192
    global_rank: 402
    paper_rank: 455
    rank_delta: 53
    rank_delta_abs: 53
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
    value: 0.2986
    std: 0.0075
    paper_value: 0.2986
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
    table_ref: Table 2
    source_ref: thakoor2021large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.288
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.010599999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2986
    true_std: 0.0075
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2986
    sort_std: 0.0075
    global_rank: 410
    paper_rank: 410
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.2965
    std: 0.0147
    paper_value: 0.2965
    paper_std: 0.0147
    metric: Accuracy
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
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2889
    at_pub_std: 0.005
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.007599999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2965
    true_std: 0.0147
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2965
    sort_std: 0.0147
    global_rank: 415
    paper_rank: 415
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.2803
    std: 0.0118
    paper_value: 0.2803
    paper_std: 0.0118
    metric: Accuracy
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
    source_ref: kipf2016variational
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2536
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0267
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2863
    true_std: 0.0105
    value_gap_source_arxiv: '2308.10077'
    value_gap_source_title: Contrastive Learning for Non-Local Graphs with Multi-Resolution
      Structural Views
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.2863
    sort_std: 0.0105
    global_rank: 440
    paper_rank: 452
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.2828
    std: 0.0127
    paper_value: 0.2828
    paper_std: 0.0127
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
    table_ref: Table 2
    source_ref: grover2016node2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2828
    true_std: 0.0127
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2828
    sort_std: 0.0127
    global_rank: 448
    paper_rank: 448
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
    value: 0.2278
    std: 0.0064
    paper_value: 0.2278
    paper_std: 0.0064
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
    table_ref: Table 2
    source_ref: perozzi2014deepwalk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Actor heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.255
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.027200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.255
    true_std: 0.0028
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.027200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.255
    sort_std: 0.0028
    global_rank: 478
    paper_rank: 519
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
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
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
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
    global_rank: 1
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
    value: 0.9264
    std: 0.0042
    paper_value: 0.9264
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.926
    at_pub_std: 0.004
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04049999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 296
    rank_delta: 294
    rank_delta_abs: 294
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
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
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9235
    std: 0.0025
    paper_value: 0.9235
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9242
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0007000000000000339
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.03969999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 337
    rank_delta: 328
    rank_delta_abs: 328
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.9285
    std: 0.0031
    paper_value: 0.9285
    paper_std: 0.0031
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9361
    true_std: 0.0035
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.007600000000000051
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: 0.0035
    global_rank: 159
    paper_rank: 261
    rank_delta: 102
    rank_delta_abs: 102
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
    value: 0.9324
    std: 0.0029
    paper_value: 0.9324
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9337
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2206.12933'
    at_pub_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0012999999999999678
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9337
    true_std: 0.0021
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0012999999999999678
    has_value_note: false
    value_note: ''
    sort_value: 0.9337
    sort_std: 0.0021
    global_rank: 198
    paper_rank: 214
    rank_delta: 16
    rank_delta_abs: 16
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
    value: 0.9278
    std: 0.0017
    paper_value: 0.9278
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.932
    at_pub_std: 0.003
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0042000000000000925
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.932
    true_std: 0.006
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.0042000000000000925
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.006
    global_rank: 217
    paper_rank: 273
    rank_delta: 56
    rank_delta_abs: 56
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
    value: 0.9265
    std: 0.0032
    paper_value: 0.9265
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.928
    at_pub_std: 0.005
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0015000000000000568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9313
    true_std: 0.0017
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0048000000000000265
    has_value_note: false
    value_note: ''
    sort_value: 0.9313
    sort_std: 0.0017
    global_rank: 229
    paper_rank: 294
    rank_delta: 65
    rank_delta_abs: 65
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
    value: 0.9201
    std: 0.0013
    paper_value: 0.9201
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9174
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0027000000000000357
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.931
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.01090000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.931
    sort_std: 0.004
    global_rank: 232
    paper_rank: 371
    rank_delta: 139
    rank_delta_abs: 139
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9149
    std: 0.0025
    paper_value: 0.9149
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9161
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0011999999999999789
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.015999999999999903
    has_value_note: false
    value_note: ''
    sort_value: 0.9309
    sort_std: 0.0008
    global_rank: 239
    paper_rank: 410
    rank_delta: 171
    rank_delta_abs: 171
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
    value: 0.922
    std: 0.0011
    paper_value: 0.922
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9224
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9224
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9224
    sort_std: null
    global_rank: 349
    paper_rank: 356
    rank_delta: 7
    rank_delta_abs: 7
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
    value: 0.9162
    std: 0.0013
    paper_value: 0.9162
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9185
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0022999999999999687
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9185
    true_std: 0.0006
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0022999999999999687
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: 0.0006
    global_rank: 385
    paper_rank: 400
    rank_delta: 15
    rank_delta_abs: 15
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
    value: 0.7854
    std: 0.0005
    paper_value: 0.7854
    paper_std: 0.0005
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.785
    at_pub_std: 0.002
    at_pub_source_arxiv: '2202.08480'
    at_pub_source_title: Eliciting Structural and Semantic Global Knowledge in Unsupervised
      Graph Contrastive Learning
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.12739999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0063
    global_rank: 426
    paper_rank: 588
    rank_delta: 162
    rank_delta_abs: 162
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
    value: 0.9072
    std: 0.0033
    paper_value: 0.9072
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.907
    at_pub_std: 0.002
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-12-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9081
    true_std: 0.0015
    value_gap_source_arxiv: '2512.24062'
    value_gap_source_title: Energy-Balanced Hyperspherical Graph Representation Learning
      via Structural Binding and Entropic Dispersion
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.9081
    sort_std: 0.0015
    global_rank: 447
    paper_rank: 452
    rank_delta: 5
    rank_delta_abs: 5
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
    value: 0.8944
    std: 0.0011
    paper_value: 0.8944
    paper_std: 0.0011
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9005
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9005
    true_std: 0.0008
    value_gap_source_arxiv: '2307.01053'
    value_gap_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.006099999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0008
    global_rank: 487
    paper_rank: 508
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.8967
    std: 0.0012
    paper_value: 0.8967
    paper_std: 0.0012
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Homophilic benchmark split
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.897
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-09-12'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.897
    true_std: 0.001
    value_gap_source_arxiv: '2409.08010'
    value_gap_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: 0.001
    global_rank: 501
    paper_rank: 502
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
- &id010
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
    value: 0.5638
    std: 0.0219
    paper_value: 0.5638
    paper_std: 0.0219
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.665
    at_pub_std: 0.026
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-06-18'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.10120000000000007
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
    value_gap: 0.2922
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: null
    global_rank: 3
    paper_rank: 196
    rank_delta: 193
    rank_delta_abs: 193
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
    value: 0.6158
    std: 0.0224
    paper_value: 0.6158
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6978
    at_pub_std: 0.0197
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.08199999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.16720000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.783
    sort_std: 0.006
    global_rank: 24
    paper_rank: 148
    rank_delta: 124
    rank_delta_abs: 124
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.5107
    std: 0.0268
    paper_value: 0.5107
    paper_std: 0.0268
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5381
    at_pub_std: 0.0109
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.02739999999999998
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
    value_gap: 0.22119999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7319
    sort_std: 0.0042
    global_rank: 41
    paper_rank: 229
    rank_delta: 188
    rank_delta_abs: 188
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
    value: 0.5963
    std: 0.0232
    paper_value: 0.5963
    paper_std: 0.0232
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.676
    at_pub_std: 0.024
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0797
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
    value_gap: 0.10699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.7033
    sort_std: null
    global_rank: 69
    paper_rank: 171
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.498
    std: 0.0181
    paper_value: 0.498
    paper_std: 0.0181
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6094
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.11140000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.15739999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6554
    sort_std: 0.011
    global_rank: 110
    paper_rank: 242
    rank_delta: 132
    rank_delta_abs: 132
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.4746
    std: 0.0274
    paper_value: 0.4746
    paper_std: 0.0274
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6486
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.17399999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6486
    true_std: 0.0063
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.17399999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.6486
    sort_std: 0.0063
    global_rank: 123
    paper_rank: 259
    rank_delta: 136
    rank_delta_abs: 136
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.6364
    std: 0.0126
    paper_value: 0.6364
    paper_std: 0.0126
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.6364
    true_std: 0.0126
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6364
    sort_std: 0.0126
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.6344
    std: 0.0205
    paper_value: 0.6344
    paper_std: 0.0205
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.617
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.01739999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6344
    true_std: 0.0205
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6344
    sort_std: 0.0205
    global_rank: 135
    paper_rank: 135
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
    value: 0.3522
    std: 0.0271
    paper_value: 0.3522
    paper_std: 0.0271
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4265
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.07429999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.27099999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6232
    sort_std: 0.019
    global_rank: 144
    paper_rank: 317
    rank_delta: 173
    rank_delta_abs: 173
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.4805
    std: 0.0181
    paper_value: 0.4805
    paper_std: 0.0181
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6124
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.13190000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6124
    true_std: 0.0053
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.13190000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.6124
    sort_std: 0.0053
    global_rank: 149
    paper_rank: 254
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.609
    std: null
    paper_value: 0.609
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
    table_ref: Table 2
    source_ref: geom_pei2020geom
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.609
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.609
    true_std: null
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.609
    sort_std: null
    global_rank: 156
    paper_rank: 156
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
    value: 0.5939
    std: 0.0198
    paper_value: 0.5939
    paper_std: 0.0198
    metric: Accuracy
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
    source_ref: zhu2020beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.603
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2206.14418'
    at_pub_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    at_pub_source_date_iso: '2022-06-29'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-06-29'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.009099999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.603
    true_std: 0.0231
    value_gap_source_arxiv: '2206.14418'
    value_gap_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    value_gap_source_is_current_paper: false
    value_gap: 0.009099999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.0231
    global_rank: 164
    paper_rank: 172
    rank_delta: 8
    rank_delta_abs: 8
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
    value: 0.3995
    std: 0.0175
    paper_value: 0.3995
    paper_std: 0.0175
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6027
    at_pub_std: 0.007
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.2032
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6027
    true_std: 0.007
    value_gap_source_arxiv: '2506.19343'
    value_gap_source_title: Discrepancy-Aware Graph Mask Auto-Encoder
    value_gap_source_is_current_paper: false
    value_gap: 0.2032
    has_value_note: false
    value_note: ''
    sort_value: 0.6027
    sort_std: 0.007
    global_rank: 165
    paper_rank: 302
    rank_delta: 137
    rank_delta_abs: 137
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4691
    std: 0.0215
    paper_value: 0.4691
    paper_std: 0.0215
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.482
    at_pub_std: 0.0263
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.012899999999999967
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
    value_gap: 0.07380000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5429
    sort_std: null
    global_rank: 208
    paper_rank: 262
    rank_delta: 54
    rank_delta_abs: 54
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
    value: 0.4697
    std: 0.0343
    paper_value: 0.4697
    paper_std: 0.0343
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5281
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05840000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5281
    true_std: 0.0063
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.05840000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.5281
    sort_std: 0.0063
    global_rank: 214
    paper_rank: 262
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.5268
    std: 0.0214
    paper_value: 0.5268
    paper_std: 0.0214
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5268
    true_std: 0.0214
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5268
    sort_std: 0.0214
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.4774
    std: 0.0205
    paper_value: 0.4774
    paper_std: 0.0205
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4399
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.03749999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4774
    true_std: 0.0205
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4774
    sort_std: 0.0205
    global_rank: 256
    paper_rank: 256
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4193
    std: 0.0329
    paper_value: 0.4193
    paper_std: 0.0329
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4193
    true_std: 0.0329
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4193
    sort_std: 0.0329
    global_rank: 294
    paper_rank: 294
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
    value: 0.3384
    std: 0.0277
    paper_value: 0.3384
    paper_std: 0.0277
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Chameleon heterophilic dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3913
    at_pub_std: 0.0134
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0529
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3913
    true_std: 0.0134
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.0529
    has_value_note: false
    value_note: ''
    sort_value: 0.3913
    sort_std: 0.0134
    global_rank: 308
    paper_rank: 318
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
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
    value: 0.703
    std: null
    paper_value: 0.703
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
    source_ref: Kipf & Welling 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.09130000000000005
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
    value_gap: 0.17390000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 665
    rank_delta: 644
    rank_delta_abs: 644
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.725
    std: null
    paper_value: 0.725
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
    source_ref: Veličković et al. 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8013
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.07630000000000003
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
    value_gap: 0.08300000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 440
    rank_delta: 394
    rank_delta_abs: 394
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.7308
    std: 0.0084
    paper_value: 0.7308
    paper_std: 0.0084
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
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.7906
    true_std: 0.0134
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.059799999999999964
    has_value_note: false
    value_note: ''
    sort_value: 0.7906
    sort_std: 0.0134
    global_rank: 80
    paper_rank: 374
    rank_delta: 294
    rank_delta_abs: 294
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
    value: 0.7149
    std: 0.0014
    paper_value: 0.7149
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
    source_ref: Veličković et al. 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7882
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07330000000000003
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
    value_gap: 0.07410000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.002
    global_rank: 83
    paper_rank: 572
    rank_delta: 489
    rank_delta_abs: 489
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
    value: 0.7156
    std: 0.0056
    paper_value: 0.7156
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Peng et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7869
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07130000000000003
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
    value_gap: 0.07130000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7869
    sort_std: 0.0016
    global_rank: 90
    paper_rank: 563
    rank_delta: 473
    rank_delta_abs: 473
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
    value: 0.7275
    std: 0.0046
    paper_value: 0.7275
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
    source_ref: Hassani et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7808
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.053300000000000014
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
    value_gap: 0.053300000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0006
    global_rank: 108
    paper_rank: 411
    rank_delta: 303
    rank_delta_abs: 303
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
    value: 0.7159
    std: 0.0042
    paper_value: 0.7159
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
    source_ref: Thakoor et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7182
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0022999999999999687
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
    value_gap: 0.04410000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.002
    global_rank: 171
    paper_rank: 561
    rank_delta: 390
    rank_delta_abs: 390
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
    value: 0.7121
    std: 0.0024
    paper_value: 0.7121
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
    source_ref: Zhu et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7133
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0012000000000000899
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7523
    true_std: 0.0119
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.040200000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.7523
    sort_std: 0.0119
    global_rank: 211
    paper_rank: 598
    rank_delta: 387
    rank_delta_abs: 387
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
    value: 0.7141
    std: 0.0038
    paper_value: 0.7141
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
    source_ref: Zhu et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7226
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2208.06743'
    at_pub_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    at_pub_source_date_iso: '2022-08-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.008500000000000063
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
    value_gap: 0.03090000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 576
    rank_delta: 331
    rank_delta_abs: 331
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
    value: 0.5691
    std: 0.0042
    paper_value: 0.5691
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6958
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.12669999999999992
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
    value_gap: 0.15979999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 928
    rank_delta: 527
    rank_delta_abs: 527
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.6675
    std: 0.0037
    paper_value: 0.6675
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Kipf & Welling 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.699
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.03149999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.03149999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.699
    sort_std: 0.0057
    global_rank: 689
    paper_rank: 796
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.5882
    std: 0.0061
    paper_value: 0.5882
    paper_std: 0.0061
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
    source_ref: Perozzi et al. 2014
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6785
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.09030000000000005
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
    value_gap: 0.09030000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.6785
    sort_std: 0.0079
    global_rank: 759
    paper_rank: 916
    rank_delta: 157
    rank_delta_abs: 157
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.6522
    std: 0.0043
    paper_value: 0.6522
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
    source_ref: Kipf & Welling 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6639
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.011700000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6639
    true_std: 0.0024
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.011700000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.6639
    sort_std: 0.0024
    global_rank: 806
    paper_rank: 834
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4764
    std: 0.0077
    paper_value: 0.4764
    paper_std: 0.0077
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
    source_ref: Grover et al. 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6552
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.17880000000000001
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
    value_gap: 0.17880000000000001
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
- &id006
  dataset: Coauthor-CS
  rows:
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.969
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
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-fa
    model_key: gwn-fa
    model_plain: GWN-fa
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-sym
    model_key: gwn-sym
    model_plain: GWN-sym
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9593
    std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: 0.9593
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.931
    std: 0.0017
    paper_value: 0.931
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
    source_ref: original papers
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.936
    at_pub_std: 0.015
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9514
    true_std: 0.0025
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.020399999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0025
    global_rank: 14
    paper_rank: 69
    rank_delta: 55
    rank_delta_abs: 55
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.9465
    std: 0.0018
    paper_value: 0.9465
    paper_std: 0.0018
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9465
    true_std: 0.0018
    value_gap_source_arxiv: '2402.15270'
    value_gap_source_title: Smoothed Graph Contrastive Learning via Seamless Proximity
      Integration
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9465
    sort_std: 0.0018
    global_rank: 21
    paper_rank: 21
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
    value: 0.9241
    std: 0.0027
    paper_value: 0.9241
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: original papers
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.938
    at_pub_std: 0.004
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.013899999999999912
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9437
    true_std: 0.0028
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.01959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9437
    sort_std: 0.0028
    global_rank: 23
    paper_rank: 113
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Convolutional Neural Networks and Label
      Propagation
    comparison_source_arxiv: '2002.06755'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9195
    std: 0.004
    paper_value: 0.9195
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.922
    at_pub_std: 0.006
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0025000000000000577
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.935
    true_std: 0.003
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.01550000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.003
    global_rank: 47
    paper_rank: 136
    rank_delta: 89
    rank_delta_abs: 89
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
    value: 0.9332
    std: 0.0012
    paper_value: 0.9332
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.931
    at_pub_std: 0.0
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0021999999999999797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9332
    true_std: 0.0012
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9332
    sort_std: 0.0012
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.9326
    std: 0.0036
    paper_value: 0.9326
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9331
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9331
    true_std: 0.0013
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.000500000000000056
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: 0.0013
    global_rank: 59
    paper_rank: 64
    rank_delta: 5
    rank_delta_abs: 5
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
    value: 0.9278
    std: 0.0023
    paper_value: 0.9278
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.928
    at_pub_std: 0.001
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-02-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9301
    true_std: 0.0003
    value_gap_source_arxiv: '2502.20885'
    value_gap_source_title: A Fused Gromov-Wasserstein Approach to Subgraph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0023000000000000798
    has_value_note: false
    value_note: ''
    sort_value: 0.9301
    sort_std: 0.0003
    global_rank: 75
    paper_rank: 100
    rank_delta: 25
    rank_delta_abs: 25
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
    value: 0.9042
    std: 0.0008
    paper_value: 0.9042
    paper_std: 0.0008
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.917
    at_pub_std: 0.014
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.012800000000000034
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.928
    true_std: 0.002
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: 0.023800000000000043
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.002
    global_rank: 96
    paper_rank: 171
    rank_delta: 75
    rank_delta_abs: 75
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
    value: 0.9211
    std: 0.0009
    paper_value: 0.9211
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9211
    at_pub_std: 0.09
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
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
    true_value: 0.9211
    true_std: 0.0009
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0009
    global_rank: 127
    paper_rank: 127
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
    value: 0.9197
    std: 0.0019
    paper_value: 0.9197
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
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9211
    at_pub_std: 0.12
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0014000000000000679
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9211
    true_std: 0.0012
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0014000000000000679
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0012
    global_rank: 126
    paper_rank: 136
    rank_delta: 10
    rank_delta_abs: 10
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
    value: 0.9001
    std: 0.0071
    paper_value: 0.9001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9001
    at_pub_std: 0.71
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9005
    true_std: 0.0035
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0035
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.8508
    std: 0.0003
    paper_value: 0.8508
    paper_std: 0.0003
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.851
    at_pub_std: 0.0
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.851
    true_std: 0.0
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.851
    sort_std: 0.0
    global_rank: 201
    paper_rank: 201
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.8461
    std: 0.0022
    paper_value: 0.8461
    paper_std: 0.0022
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-CS node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8461
    at_pub_std: 0.22
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8461
    true_std: 0.0022
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8461
    sort_std: 0.0022
    global_rank: 205
    paper_rank: 205
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
  dataset: Coauthor-Physics
  rows:
  - model: GrokFormer
    model_key: grokformer
    model_plain: GrokFormer
    value: 0.9831
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9831
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PolyFormer
    model_key: polyformer
    model_plain: PolyFormer
    value: 0.9808
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9808
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9796
    std: 0.0081
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9796
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9545
    std: 0.0017
    paper_value: 0.9545
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.962
    at_pub_std: 0.001
    at_pub_source_arxiv: '2103.14958'
    at_pub_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without explicit
      negative sampling'
    at_pub_source_date_iso: '2021-03-27'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.007499999999999951
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9782
    true_std: 0.0028
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.023699999999999943
    has_value_note: false
    value_note: ''
    sort_value: 0.9782
    sort_std: 0.0028
    global_rank: 6
    paper_rank: 149
    rank_delta: 143
    rank_delta_abs: 143
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without
      explicit negative sampling'
    comparison_source_arxiv: '2103.14958'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9554
    std: 0.0019
    paper_value: 0.9554
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.965
    at_pub_std: 0.001
    at_pub_source_arxiv: '2103.14958'
    at_pub_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without explicit
      negative sampling'
    at_pub_source_date_iso: '2021-03-27'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.009599999999999942
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9774
    true_std: 0.0035
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9774
    sort_std: 0.0035
    global_rank: 9
    paper_rank: 134
    rank_delta: 125
    rank_delta_abs: 125
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SelfGNN: Self-supervised Graph Neural Networks without
      explicit negative sampling'
    comparison_source_arxiv: '2103.14958'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9739
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 18
    sort_value: 0.9739
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.9613
    std: 0.0012
    paper_value: 0.9613
    paper_std: 0.0012
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9613
    true_std: 0.0012
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9613
    sort_std: 0.0012
    global_rank: 76
    paper_rank: 76
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
    value: 0.9354
    std: 0.0005
    paper_value: 0.9354
    paper_std: 0.0005
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.935
    at_pub_std: 0.001
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9597
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.02429999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9597
    sort_std: 0.0007
    global_rank: 83
    paper_rank: 241
    rank_delta: 158
    rank_delta_abs: 158
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
    value: 0.9587
    std: 0.0015
    paper_value: 0.9587
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.959
    at_pub_std: 0.002
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.959
    true_std: 0.002
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.002
    global_rank: 88
    paper_rank: 89
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.9576
    std: 0.0038
    paper_value: 0.9576
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.958
    at_pub_std: 0.004
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.004
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.004
    global_rank: 94
    paper_rank: 99
    rank_delta: 5
    rank_delta_abs: 5
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
    value: 0.9539
    std: 0.0032
    paper_value: 0.9539
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9526
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2206.12933'
    at_pub_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0012999999999999678
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9574
    true_std: 0.0006
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0035000000000000586
    has_value_note: false
    value_note: ''
    sort_value: 0.9574
    sort_std: 0.0006
    global_rank: 102
    paper_rank: 155
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVRL
    model_key: mvrl
    model_plain: MVRL
    value: 0.9553
    std: 0.001
    paper_value: 0.9553
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.953
    at_pub_std: 0.001
    at_pub_source_arxiv: '2205.15746'
    at_pub_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    at_pub_source_date_iso: '2022-05-31'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0023000000000000798
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9553
    true_std: 0.001
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9553
    sort_std: 0.001
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    comparison_source_arxiv: '2205.15746'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9492
    std: 0.0007
    paper_value: 0.9492
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9492
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
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
    true_value: 0.952
    true_std: 0.001
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.0027999999999999137
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.001
    global_rank: 170
    paper_rank: 185
    rank_delta: 15
    rank_delta_abs: 15
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
    value: 0.9177
    std: 0.0015
    paper_value: 0.9177
    paper_std: 0.0015
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.949
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.031299999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: null
    global_rank: 188
    paper_rank: 293
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9457
    std: 0.0038
    paper_value: 0.9457
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9451
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0005999999999999339
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
    value_gap_source_is_current_paper: false
    value_gap: 0.0031999999999999806
    has_value_note: false
    value_note: ''
    sort_value: 0.9489
    sort_std: 0.0009
    global_rank: 191
    paper_rank: 197
    rank_delta: 6
    rank_delta_abs: 6
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
    value: 0.9452
    std: 0.0
    paper_value: 0.9452
    paper_std: 0.0
    metric: Accuracy
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9452
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-01-31'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9452
    true_std: 0.0
    value_gap_source_arxiv: '2401.17580'
    value_gap_source_title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9452
    sort_std: 0.0
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
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.9119
    std: 0.0004
    paper_value: 0.9119
    paper_std: 0.0004
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Coauthor-Physics node classification
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.912
    at_pub_std: 0.0
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.001
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.001
    global_rank: 299
    paper_rank: 299
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Kipf and Welling 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8728
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.057800000000000074
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
    value_gap: 0.08540000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 657
    rank_delta: 626
    rank_delta_abs: 626
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.83
    std: null
    paper_value: 0.83
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
    source_ref: Veličković et al. 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05900000000000005
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
    value_gap: 0.059700000000000086
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 498
    rank_delta: 431
    rank_delta_abs: 431
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8108
    std: 0.0017
    paper_value: 0.8108
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
    source_ref: Thakoor et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8144
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0036000000000000476
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
    value_gap: 0.06220000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 170
    paper_rank: 691
    rank_delta: 521
    rank_delta_abs: 521
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
    value: 0.8008
    std: 0.0053
    paper_value: 0.8008
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
    source_ref: Zhu et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8362
    at_pub_std: 0.0113
    at_pub_source_arxiv: '2208.06743'
    at_pub_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    at_pub_source_date_iso: '2022-08-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0354000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.07120000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.002
    global_rank: 176
    paper_rank: 737
    rank_delta: 561
    rank_delta_abs: 561
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    comparison_source_arxiv: '2208.06743'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.8303
    std: 0.0027
    paper_value: 0.8303
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Hassani et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8538
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.023499999999999965
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
    value_gap: 0.037699999999999956
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.005
    global_rank: 205
    paper_rank: 498
    rank_delta: 293
    rank_delta_abs: 293
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
    value: 0.8229
    std: 0.0056
    paper_value: 0.8229
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Veličković et al. 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8508
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.027900000000000036
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
    value_gap: 0.040100000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.002
    global_rank: 227
    paper_rank: 579
    rank_delta: 352
    rank_delta_abs: 352
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
    value: 0.8251
    std: 0.0147
    paper_value: 0.8251
    paper_std: 0.0147
    metric: Accuracy
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
    source_ref: Peng et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8526
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02750000000000008
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
    value_gap: 0.02750000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8526
    sort_std: 0.0008
    global_rank: 276
    paper_rank: 544
    rank_delta: 268
    rank_delta_abs: 268
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8381
    std: 0.0087
    paper_value: 0.8381
    paper_std: 0.0087
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.8516
    true_std: 0.0077
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.013500000000000068
    has_value_note: false
    value_note: ''
    sort_value: 0.8516
    sort_std: 0.0077
    global_rank: 281
    paper_rank: 379
    rank_delta: 98
    rank_delta_abs: 98
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
    value: 0.8039
    std: 0.0042
    paper_value: 0.8039
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
    source_ref: Zhu et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.831
    at_pub_std: 0.003
    at_pub_source_arxiv: '2211.03710'
    at_pub_source_title: Graph Contrastive Learning with Implicit Augmentations
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.027100000000000013
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8409
    true_std: 0.0085
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03700000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.0085
    global_rank: 363
    paper_rank: 725
    rank_delta: 362
    rank_delta_abs: 362
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Implicit Augmentations
    comparison_source_arxiv: '2211.03710'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.7981
    std: 0.0087
    paper_value: 0.7981
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Kipf and Welling 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8059
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.007799999999999918
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
    value_gap: 0.037899999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0052
    global_rank: 418
    paper_rank: 747
    rank_delta: 329
    rank_delta_abs: 329
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
    value: 0.6947
    std: 0.0055
    paper_value: 0.6947
    paper_std: 0.0055
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
    source_ref: Perozzi et al. 2014
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.829
    at_pub_std: null
    at_pub_source_arxiv: '1909.00958'
    at_pub_source_title: 'Graph Representation Learning: A Survey'
    at_pub_source_date_iso: '2019-09-03'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.13429999999999997
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
    value_gap: 0.13429999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: null
    global_rank: 508
    paper_rank: 908
    rank_delta: 400
    rank_delta_abs: 400
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Representation Learning: A Survey'
    comparison_source_arxiv: '1909.00958'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.7124
    std: 0.0089
    paper_value: 0.7124
    paper_std: 0.0089
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
    source_ref: Grover et al. 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.803
    at_pub_std: null
    at_pub_source_arxiv: '1909.00958'
    at_pub_source_title: 'Graph Representation Learning: A Survey'
    at_pub_source_date_iso: '2019-09-03'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.09060000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.803
    true_std: null
    value_gap_source_arxiv: '1909.00958'
    value_gap_source_title: 'Graph Representation Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.09060000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.803
    sort_std: null
    global_rank: 728
    paper_rank: 896
    rank_delta: 168
    rank_delta_abs: 168
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
    value: 0.7107
    std: 0.0039
    paper_value: 0.7107
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Kipf and Welling 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8011
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.09040000000000004
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
    value_gap: 0.09040000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8011
    sort_std: 0.0022
    global_rank: 736
    paper_rank: 897
    rank_delta: 161
    rank_delta_abs: 161
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
    value: 0.5611
    std: 0.0034
    paper_value: 0.5611
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7475
    at_pub_std: 0.0222
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.1864
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
    value_gap: 0.2157
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 976
    rank_delta: 170
    rank_delta_abs: 170
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    comparison_source_arxiv: '2211.11761'
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8189
    std: 0.0593
    paper_value: 0.8189
    paper_std: 0.0593
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9157
    at_pub_std: 0.0196
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-02-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0968
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9279
    true_std: 0.0312
    value_gap_source_arxiv: '2302.03228'
    value_gap_source_title: Heterophily-Aware Graph Attention Network
    value_gap_source_is_current_paper: false
    value_gap: 0.10899999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9279
    sort_std: 0.0312
    global_rank: 11
    paper_rank: 190
    rank_delta: 179
    rank_delta_abs: 179
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8108
    std: 0.0793
    paper_value: 0.8108
    paper_std: 0.0793
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8486
    at_pub_std: 0.0604
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.037800000000000056
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9136
    true_std: 0.007
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1028
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 25
    paper_rank: 199
    rank_delta: 174
    rank_delta_abs: 174
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8135
    std: 0.0505
    paper_value: 0.8135
    paper_std: 0.0505
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8108
    at_pub_std: null
    at_pub_source_arxiv: '2207.08629'
    at_pub_source_title: Comprehensive Graph Gradual Pruning for Sparse Training in
      Graph Neural Networks
    at_pub_source_date_iso: '2022-07-18'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0027000000000000357
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8852
    true_std: 0.0133
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07169999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8852
    sort_std: 0.0133
    global_rank: 48
    paper_rank: 194
    rank_delta: 146
    rank_delta_abs: 146
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8216
    std: 0.048
    paper_value: 0.8216
    paper_std: 0.048
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.827
    at_pub_std: 0.053
    at_pub_source_arxiv: '2202.02296'
    at_pub_source_title: Graph-Coupled Oscillator Networks
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00539999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0471
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.04069999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0471
    global_rank: 85
    paper_rank: 181
    rank_delta: 96
    rank_delta_abs: 96
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8514
    std: 0.0487
    paper_value: 0.8514
    paper_std: 0.0487
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8514
    true_std: 0.0487
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8514
    sort_std: 0.0487
    global_rank: 109
    paper_rank: 109
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5946
    std: 0.0363
    paper_value: 0.5946
    paper_std: 0.0363
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.819
    at_pub_std: 0.054
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.22439999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: 0.054
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.22439999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.054
    global_rank: 190
    paper_rank: 447
    rank_delta: 257
    rank_delta_abs: 257
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5703
    std: 0.033
    paper_value: 0.5703
    paper_std: 0.033
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.792
    at_pub_std: 0.063
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-07-01'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.2217
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8082
    true_std: 0.036
    value_gap_source_arxiv: '2602.05358'
    value_gap_source_title: Bayesian Neighborhood Adaptation for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2379
    has_value_note: false
    value_note: ''
    sort_value: 0.8082
    sort_std: 0.036
    global_rank: 203
    paper_rank: 491
    rank_delta: 288
    rank_delta_abs: 288
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.6335
    std: 0.0461
    paper_value: 0.6335
    paper_std: 0.0461
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4648
    at_pub_std: 0.0797
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.16869999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7082
    true_std: 0.0271
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0747000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7082
    sort_std: 0.0271
    global_rank: 334
    paper_rank: 417
    rank_delta: 83
    rank_delta_abs: 83
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    comparison_source_arxiv: '2202.09025'
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.6757
    std: 0.0498
    paper_value: 0.6757
    paper_std: 0.0498
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6757
    true_std: 0.0498
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6757
    sort_std: 0.0498
    global_rank: 366
    paper_rank: 366
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
    value: 0.643
    std: 0.0543
    paper_value: 0.643
    paper_std: 0.0543
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5351
    at_pub_std: 0.0326
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.1079
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: 0.0543
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.0543
    global_rank: 405
    paper_rank: 405
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    comparison_source_arxiv: '2202.09025'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.6081
    std: null
    paper_value: 0.6081
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
    table_ref: Table 3
    source_ref: Pei et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6081
    at_pub_std: null
    at_pub_source_arxiv: '2103.06064'
    at_pub_source_title: Graph Neural Networks Inspired by Classical Iterative Algorithms
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6412
    true_std: null
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: 0.03310000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6412
    sort_std: null
    global_rank: 407
    paper_rank: 434
    rank_delta: 27
    rank_delta_abs: 27
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
    value: 0.5885
    std: 0.0321
    paper_value: 0.5885
    paper_std: 0.0321
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.454
    at_pub_std: 0.0999
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-04-15'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.1345
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6309
    true_std: 0.0987
    value_gap_source_arxiv: '2304.07509'
    value_gap_source_title: Multi-View Graph Representation Learning Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.04239999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6309
    sort_std: 0.0987
    global_rank: 420
    paper_rank: 458
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    comparison_source_arxiv: '2202.09025'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.5486
    std: 0.0695
    paper_value: 0.5486
    paper_std: 0.0695
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.6066
    true_std: 0.0294
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05800000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.6066
    sort_std: 0.0294
    global_rank: 438
    paper_rank: 503
    rank_delta: 65
    rank_delta_abs: 65
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
    value: 0.5919
    std: 0.0409
    paper_value: 0.5919
    paper_std: 0.0409
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4932
    at_pub_std: 0.0919
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.09869999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5919
    true_std: 0.0409
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5919
    sort_std: 0.0409
    global_rank: 453
    paper_rank: 453
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.573
    std: 0.0551
    paper_value: 0.573
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5033
    at_pub_std: 0.0229
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06969999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.573
    true_std: 0.0551
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.573
    sort_std: 0.0551
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.5541
    std: 0.0456
    paper_value: 0.5541
    paper_std: 0.0456
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5541
    true_std: 0.0456
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5541
    sort_std: 0.0456
    global_rank: 502
    paper_rank: 502
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.5476
    std: 0.0506
    paper_value: 0.5476
    paper_std: 0.0506
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5476
    true_std: 0.0506
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5476
    sort_std: 0.0506
    global_rank: 504
    paper_rank: 504
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
    value: 0.3918
    std: 0.0557
    paper_value: 0.3918
    paper_std: 0.0557
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4155
    at_pub_std: 0.0312
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-04-15'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0237
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4867
    true_std: 0.2784
    value_gap_source_arxiv: '2304.07509'
    value_gap_source_title: Multi-View Graph Representation Learning Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.09490000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.4867
    sort_std: 0.2784
    global_rank: 572
    paper_rank: 627
    rank_delta: 55
    rank_delta_abs: 55
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
    value: 0.4294
    std: 0.0746
    paper_value: 0.4294
    paper_std: 0.0746
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilic split for Cornell
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4054
    at_pub_std: 0.0162
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.02400000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4294
    true_std: 0.0746
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4294
    sort_std: 0.0746
    global_rank: 614
    paper_rank: 614
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
    value: 0.79
    std: null
    paper_value: 0.79
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
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10699999999999998
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
    value_gap: 0.13959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 641
    rank_delta: 622
    rank_delta_abs: 622
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
    std: null
    paper_value: 0.79
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
    source_ref: velivckovic2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10699999999999998
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
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 641
    rank_delta: 618
    rank_delta_abs: 618
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
    value: 0.7997
    std: 0.0036
    paper_value: 0.7997
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
    source_ref: thakoor2021large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8134
    at_pub_std: 0.005
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.013700000000000045
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.08330000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.883
    sort_std: 0.001
    global_rank: 167
    paper_rank: 509
    rank_delta: 342
    rank_delta_abs: 342
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.8015
    std: 0.0034
    paper_value: 0.8015
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8645
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2208.06743'
    at_pub_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    at_pub_source_date_iso: '2022-08-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06300000000000006
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
    value_gap: 0.07150000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 224
    paper_rank: 489
    rank_delta: 265
    rank_delta_abs: 265
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    comparison_source_arxiv: '2208.06743'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.7983
    std: 0.009
    paper_value: 0.7983
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
    source_ref: peng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8726
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07430000000000003
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
    value_gap: 0.07430000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8726
    sort_std: 0.0016
    global_rank: 225
    paper_rank: 522
    rank_delta: 297
    rank_delta_abs: 297
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
    value: 0.7963
    std: 0.0038
    paper_value: 0.7963
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
    source_ref: hassani2020contrastive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8725
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07620000000000005
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
    value_gap: 0.07620000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8725
    sort_std: 0.0012
    global_rank: 226
    paper_rank: 536
    rank_delta: 310
    rank_delta_abs: 310
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
    value: 0.7743
    std: 0.0084
    paper_value: 0.7743
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
    source_ref: velivckovic2019deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8703
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09599999999999997
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
    value_gap: 0.09650000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8708
    sort_std: 0.0017
    global_rank: 235
    paper_rank: 786
    rank_delta: 551
    rank_delta_abs: 551
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
    value: 0.7135
    std: 0.0005
    paper_value: 0.7135
    paper_std: 0.0005
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
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8638
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.1503
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
    value_gap: 0.15549999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 914
    rank_delta: 671
    rank_delta_abs: 671
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
    value: 0.6987
    std: 0.0125
    paper_value: 0.6987
    paper_std: 0.0125
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
    source_ref: perozzi2014deepwalk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8652
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.16649999999999998
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
    value_gap: 0.16649999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8652
    sort_std: 0.0012
    global_rank: 255
    paper_rank: 924
    rank_delta: 669
    rank_delta_abs: 669
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8029
    std: 0.01
    paper_value: 0.8029
    paper_std: 0.01
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
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.8564
    true_std: 0.0028
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0535000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8564
    sort_std: 0.0028
    global_rank: 274
    paper_rank: 477
    rank_delta: 203
    rank_delta_abs: 203
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
    value: 0.6647
    std: 0.01
    paper_value: 0.6647
    paper_std: 0.01
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
    source_ref: grover2016node2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.852
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.18730000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.852
    true_std: 0.0002
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.18730000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.852
    sort_std: 0.0002
    global_rank: 287
    paper_rank: 943
    rank_delta: 656
    rank_delta_abs: 656
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
    value: 0.8037
    std: 0.0075
    paper_value: 0.8037
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
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8128
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009099999999999997
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
    value_gap: 0.04749999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8512
    sort_std: 0.0023
    global_rank: 291
    paper_rank: 467
    rank_delta: 176
    rank_delta_abs: 176
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
    value: 0.7716
    std: 0.0031
    paper_value: 0.7716
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2016variational
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8133
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.04170000000000007
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
    value_gap: 0.05910000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8307
    sort_std: 0.0029
    global_rank: 342
    paper_rank: 801
    rank_delta: 459
    rank_delta_abs: 459
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.7173
    std: 0.0092
    paper_value: 0.7173
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2016variational
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016)
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7828
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0655
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
    value_gap: 0.11209999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8294
    sort_std: 0.0031
    global_rank: 347
    paper_rank: 908
    rank_delta: 561
    rank_delta_abs: 561
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
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
- &id011
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
    value: 0.3965
    std: 0.0281
    paper_value: 0.3965
    paper_std: 0.0281
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.2945
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10200000000000004
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.748
    true_std: 0.005
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.3515
    has_value_note: false
    value_note: ''
    sort_value: 0.748
    sort_std: 0.005
    global_rank: 10
    paper_rank: 188
    rank_delta: 178
    rank_delta_abs: 178
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.379
    std: 0.0202
    paper_value: 0.379
    paper_std: 0.0202
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4075
    at_pub_std: 0.0144
    at_pub_source_arxiv: '2206.14418'
    at_pub_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    at_pub_source_date_iso: '2022-06-29'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02849999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.619
    true_std: 0.014
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.24
    has_value_note: false
    value_note: ''
    sort_value: 0.619
    sort_std: 0.014
    global_rank: 42
    paper_rank: 207
    rank_delta: 165
    rank_delta_abs: 165
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
    value: 0.3628
    std: 0.0152
    paper_value: 0.3628
    paper_std: 0.0152
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.557
    at_pub_std: 0.024
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.19420000000000004
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
    value_gap: 0.2439
    has_value_note: false
    value_note: ''
    sort_value: 0.6067
    sort_std: null
    global_rank: 51
    paper_rank: 231
    rank_delta: 180
    rank_delta_abs: 180
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.3547
    std: 0.0129
    paper_value: 0.3547
    paper_std: 0.0129
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3875
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.032799999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.24619999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6009
    sort_std: 0.0044
    global_rank: 55
    paper_rank: 244
    rank_delta: 189
    rank_delta_abs: 189
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.3209
    std: 0.0327
    paper_value: 0.3209
    paper_std: 0.0327
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.563
    at_pub_std: 0.022
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.24209999999999993
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
    value_gap: 0.24209999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.563
    sort_std: 0.022
    global_rank: 77
    paper_rank: 270
    rank_delta: 193
    rank_delta_abs: 193
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.355
    std: 0.0091
    paper_value: 0.355
    paper_std: 0.0091
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4153
    at_pub_std: 0.0109
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.06030000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.1259
    has_value_note: false
    value_note: ''
    sort_value: 0.4809
    sort_std: 0.0021
    global_rank: 112
    paper_rank: 243
    rank_delta: 131
    rank_delta_abs: 131
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.3264
    std: 0.0078
    paper_value: 0.3264
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4624
    at_pub_std: 0.007
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.13599999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4624
    true_std: 0.007
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.13599999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.4624
    sort_std: 0.007
    global_rank: 125
    paper_rank: 267
    rank_delta: 142
    rank_delta_abs: 142
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
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
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.4229
    std: 0.0143
    paper_value: 0.4229
    paper_std: 0.0143
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.428
    true_std: 0.0101
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.005099999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.428
    sort_std: 0.0101
    global_rank: 151
    paper_rank: 163
    rank_delta: 12
    rank_delta_abs: 12
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
    value: 0.3133
    std: 0.0122
    paper_value: 0.3133
    paper_std: 0.0122
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4109
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09759999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4268
    true_std: 0.011
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.11349999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.4268
    sort_std: 0.011
    global_rank: 157
    paper_rank: 274
    rank_delta: 117
    rank_delta_abs: 117
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.4117
    std: 0.0194
    paper_value: 0.4117
    paper_std: 0.0194
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4259
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2210.00513'
    at_pub_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01419999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4259
    true_std: 0.0069
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: 0.01419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.4259
    sort_std: 0.0069
    global_rank: 159
    paper_rank: 174
    rank_delta: 15
    rank_delta_abs: 15
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
    value: 0.2948
    std: 0.0148
    paper_value: 0.2948
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3511
    at_pub_std: 0.0092
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-17'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.05630000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.13019999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.425
    sort_std: 0.0135
    global_rank: 161
    paper_rank: 282
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.318
    std: 0.0077
    paper_value: 0.318
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4222
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.10420000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4222
    true_std: 0.0063
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.10420000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.4222
    sort_std: 0.0063
    global_rank: 164
    paper_rank: 270
    rank_delta: 106
    rank_delta_abs: 106
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.2928
    std: 0.0133
    paper_value: 0.2928
    paper_std: 0.0133
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3335
    at_pub_std: 0.0124
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.040700000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.10020000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.393
    sort_std: 0.0079
    global_rank: 194
    paper_rank: 282
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.3814
    std: null
    paper_value: 0.3814
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
    table_ref: Table 2
    source_ref: geom_pei2020geom
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3815
    at_pub_std: 0.0092
    at_pub_source_arxiv: '2210.00513'
    at_pub_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3832
    true_std: 0.0092
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: 0.0017999999999999683
    has_value_note: false
    value_note: ''
    sort_value: 0.3832
    sort_std: 0.0092
    global_rank: 202
    paper_rank: 204
    rank_delta: 2
    rank_delta_abs: 2
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
    value: 0.3293
    std: 0.0158
    paper_value: 0.3293
    paper_std: 0.0158
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3754
    at_pub_std: 0.0219
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04610000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.04610000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3754
    sort_std: 0.0219
    global_rank: 217
    paper_rank: 266
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.3597
    std: 0.012
    paper_value: 0.3597
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3597
    true_std: 0.012
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3597
    sort_std: 0.012
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.3011
    std: 0.0192
    paper_value: 0.3011
    paper_std: 0.0192
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3525
    at_pub_std: 0.0121
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0514
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3525
    true_std: 0.0121
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.0514
    has_value_note: false
    value_note: ''
    sort_value: 0.3525
    sort_std: 0.0121
    global_rank: 247
    paper_rank: 280
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.2803
    std: 0.0161
    paper_value: 0.2803
    paper_std: 0.0161
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.3465
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06619999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3465
    true_std: 0.0081
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.06619999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3465
    sort_std: 0.0081
    global_rank: 256
    paper_rank: 287
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.2284
    std: 0.0072
    paper_value: 0.2284
    paper_std: 0.0072
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2284
    true_std: 0.0072
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2284
    sort_std: 0.0072
    global_rank: 312
    paper_rank: 312
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8324
    std: 0.0495
    paper_value: 0.8324
    paper_std: 0.0495
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.9291
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.09670000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9295
    true_std: 0.0131
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: 0.09709999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9295
    sort_std: 0.0131
    global_rank: 39
    paper_rank: 230
    rank_delta: 191
    rank_delta_abs: 191
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8162
    std: 0.0551
    paper_value: 0.8162
    paper_std: 0.0551
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8681
    at_pub_std: 0.0224
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.051899999999999946
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.007
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.1068
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.007
    global_rank: 45
    paper_rank: 265
    rank_delta: 220
    rank_delta_abs: 220
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8486
    std: 0.0677
    paper_value: 0.8486
    paper_std: 0.0677
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: Zhu et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.849
    at_pub_std: 0.072
    at_pub_source_arxiv: '2202.02296'
    at_pub_source_title: Graph-Coupled Oscillator Networks
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9189
    true_std: 0.0393
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.07030000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9189
    sort_std: 0.0393
    global_rank: 52
    paper_rank: 188
    rank_delta: 136
    rank_delta_abs: 136
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8432
    std: 0.0602
    paper_value: 0.8432
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8243
    at_pub_std: 0.0689
    at_pub_source_arxiv: '2112.03499'
    at_pub_source_title: A Piece-wise Polynomial Filtering Approach for Graph Neural
      Networks
    at_pub_source_date_iso: '2021-12-07'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.018899999999999917
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8961
    true_std: 0.0152
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05290000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8961
    sort_std: 0.0152
    global_rank: 82
    paper_rank: 208
    rank_delta: 126
    rank_delta_abs: 126
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.8703
    std: 0.0236
    paper_value: 0.8703
    paper_std: 0.0236
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8703
    true_std: 0.0236
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8703
    sort_std: 0.0236
    global_rank: 128
    paper_rank: 128
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Het. Rep.
    model_key: het. rep.
    model_plain: Het. Rep.
    value: 0.8378
    std: 0.0567
    paper_value: 0.8378
    paper_std: 0.0567
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: uncertain
    protocol_note: Ablation study variant.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8378
    true_std: 0.0567
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8378
    sort_std: 0.0567
    global_rank: 221
    paper_rank: 221
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
    value: 0.5946
    std: 0.0616
    paper_value: 0.5946
    paper_std: 0.0616
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.8197
    true_std: 0.0158
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.22509999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8197
    sort_std: 0.0158
    global_rank: 261
    paper_rank: 600
    rank_delta: 339
    rank_delta_abs: 339
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6162
    std: 0.0378
    paper_value: 0.6162
    paper_std: 0.0378
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.798
    at_pub_std: 0.043
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.18180000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.0645
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.20000000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.0645
    global_rank: 266
    paper_rank: 568
    rank_delta: 302
    rank_delta_abs: 302
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.6059
    std: 0.0756
    paper_value: 0.6059
    paper_std: 0.0756
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5853
    at_pub_std: 0.0298
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02059999999999995
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8148
    true_std: 0.0279
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.20889999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8148
    sort_std: 0.0279
    global_rank: 271
    paper_rank: 584
    rank_delta: 313
    rank_delta_abs: 313
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
    value: 0.6
    std: 0.048
    paper_value: 0.6
    paper_std: 0.048
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.784
    at_pub_std: 0.054
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.18400000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7933
    true_std: 0.0447
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.19330000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0447
    global_rank: 323
    paper_rank: 587
    rank_delta: 264
    rank_delta_abs: 264
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.5757
    std: 0.0568
    paper_value: 0.5757
    paper_std: 0.0568
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    true_value: 0.7574
    true_std: 0.0312
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.18169999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7574
    sort_std: 0.0312
    global_rank: 377
    paper_rank: 638
    rank_delta: 261
    rank_delta_abs: 261
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
    value: 0.6238
    std: 0.0561
    paper_value: 0.6238
    paper_std: 0.0561
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5675
    at_pub_std: 0.0597
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05630000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7301
    true_std: 0.0552
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: false
    value_gap: 0.10629999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7301
    sort_std: 0.0552
    global_rank: 426
    paper_rank: 557
    rank_delta: 131
    rank_delta_abs: 131
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
    value: 0.5919
    std: 0.0585
    paper_value: 0.5919
    paper_std: 0.0585
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5277
    at_pub_std: 0.0198
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.06420000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6841
    true_std: 0.0501
    value_gap_source_arxiv: '2510.21207'
    value_gap_source_title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised
      Learning on Diverse Graphs with Heterogeneous Specialization'
    value_gap_source_is_current_paper: false
    value_gap: 0.09220000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.6841
    sort_std: 0.0501
    global_rank: 485
    paper_rank: 612
    rank_delta: 127
    rank_delta_abs: 127
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.6757
    std: null
    paper_value: 0.6757
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
    table_ref: Table 3
    source_ref: Pei et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.676
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.676
    true_std: null
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.000300000000000078
    has_value_note: false
    value_note: ''
    sort_value: 0.676
    sort_std: null
    global_rank: 491
    paper_rank: 491
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.6405
    std: 0.0746
    paper_value: 0.6405
    paper_std: 0.0746
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6405
    true_std: 0.0746
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6405
    sort_std: 0.0746
    global_rank: 537
    paper_rank: 537
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
    value: 0.592
    std: 0.0426
    paper_value: 0.592
    paper_std: 0.0426
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5027
    at_pub_std: 0.0221
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.08929999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.0426
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.0426
    global_rank: 609
    paper_rank: 609
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.5864
    std: 0.0453
    paper_value: 0.5864
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.5878
    at_pub_std: 0.0341
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-04-15'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5909
    true_std: 0.1626
    value_gap_source_arxiv: '2304.07509'
    value_gap_source_title: Multi-View Graph Representation Learning Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.0044999999999999485
    has_value_note: false
    value_note: ''
    sort_value: 0.5909
    sort_std: 0.1626
    global_rank: 613
    paper_rank: 618
    rank_delta: 5
    rank_delta_abs: 5
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
    value: 0.5049
    std: 0.0221
    paper_value: 0.5049
    paper_std: 0.0221
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5049
    true_std: 0.0221
    value_gap_source_arxiv: '2307.16026'
    value_gap_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5049
    sort_std: 0.0221
    global_rank: 672
    paper_rank: 672
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4192
    std: 0.0776
    paper_value: 0.4192
    paper_std: 0.0776
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4864
    at_pub_std: 0.0292
    at_pub_source_arxiv: '2202.09025'
    at_pub_source_title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    at_pub_source_date_iso: '2022-02-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-08-19'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06719999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4864
    true_std: 0.0292
    value_gap_source_arxiv: '2308.10077'
    value_gap_source_title: Contrastive Learning for Non-Local Graphs with Multi-Resolution
      Structural Views
    value_gap_source_is_current_paper: false
    value_gap: 0.06719999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4864
    sort_std: 0.0292
    global_rank: 682
    paper_rank: 699
    rank_delta: 17
    rank_delta_abs: 17
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
    value: 0.4649
    std: 0.0649
    paper_value: 0.4649
    paper_std: 0.0649
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/public
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.4231
    at_pub_std: 0.0221
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-04-15'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.041800000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.47
    true_std: 0.2928
    value_gap_source_arxiv: '2304.07509'
    value_gap_source_title: Multi-View Graph Representation Learning Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.005099999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.2928
    global_rank: 687
    paper_rank: 690
    rank_delta: 3
    rank_delta_abs: 3
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
- &id012
  dataset: Wisconsin
  rows:
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.958
    std: 0.02
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
    global_rank: 1
    sort_value: 0.958
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.938
    std: 0.024
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
    sort_value: 0.938
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMD++
    model_key: dmd++
    model_plain: DMD++
    value: 0.919
    std: 0.026
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    global_rank: 3
    sort_value: 0.919
    sort_std: 0.026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8431
    std: 0.034
    paper_value: 0.8431
    paper_std: 0.034
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8629
    at_pub_std: 0.045
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.01980000000000004
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.918
    true_std: 0.031
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.07490000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.031
    global_rank: 4
    paper_rank: 64
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8667
    std: 0.0469
    paper_value: 0.8667
    paper_std: 0.0469
    metric: Accuracy
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
    source_ref: Zhu et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8765
    at_pub_std: 0.0498
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.00979999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.879
    true_std: 0.042
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.012299999999999978
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.042
    global_rank: 27
    paper_rank: 41
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREET
    model_key: greet
    model_plain: GREET
    value: 0.849
    std: 0.0448
    paper_value: 0.849
    paper_std: 0.0448
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.849
    true_std: 0.0448
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.849
    sort_std: 0.0448
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5471
    std: 0.0687
    paper_value: 0.5471
    paper_std: 0.0687
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.843
    at_pub_std: 0.037
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.29589999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.843
    true_std: 0.037
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.29589999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.843
    sort_std: 0.037
    global_rank: 67
    paper_rank: 212
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8412
    std: 0.0345
    paper_value: 0.8412
    paper_std: 0.0345
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8373
    at_pub_std: 0.0402
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-02-23'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0038999999999999035
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8412
    true_std: 0.0345
    value_gap_source_arxiv: '2302.12357'
    value_gap_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8412
    sort_std: 0.0345
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8333
    std: 0.0201
    paper_value: 0.8333
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8156
    at_pub_std: 0.0464
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-02-23'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.01770000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8333
    true_std: 0.0201
    value_gap_source_arxiv: '2302.12357'
    value_gap_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8333
    sort_std: 0.0201
    global_rank: 76
    paper_rank: 76
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
    value: 0.5647
    std: 0.0655
    paper_value: 0.5647
    paper_std: 0.0655
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.831
    at_pub_std: 0.032
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2663
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.032
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2663
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.032
    global_rank: 79
    paper_rank: 205
    rank_delta: 126
    rank_delta_abs: 126
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
    value: 0.8118
    std: 0.0556
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_display: May 2026
    date_iso: '2026-05-20'
    venue: null
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 89
    sort_value: 0.8118
    sort_std: 0.0556
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.6412
    std: null
    paper_value: 0.6412
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
    table_ref: Table 2
    source_ref: Pei et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6451
    at_pub_std: 0.0366
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0039000000000000146
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6757
    true_std: null
    value_gap_source_arxiv: '2406.10863'
    value_gap_source_title: Global-Local Graph Neural Networks for Node-Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.034499999999999975
    has_value_note: false
    value_note: ''
    sort_value: 0.6757
    sort_std: null
    global_rank: 160
    paper_rank: 171
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE-FA
    model_key: grace-fa
    model_plain: GRACE-FA
    value: 0.6373
    std: 0.0681
    paper_value: 0.6373
    paper_std: 0.0681
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6373
    true_std: 0.0681
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6373
    sort_std: 0.0681
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.6237
    std: 0.0432
    paper_value: 0.6237
    paper_std: 0.0432
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6237
    true_std: 0.0432
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6237
    sort_std: 0.0432
    global_rank: 181
    paper_rank: 181
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
    value: 0.5667
    std: 0.0551
    paper_value: 0.5667
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5667
    true_std: 0.0551
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5667
    sort_std: 0.0551
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
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.5541
    std: 0.0596
    paper_value: 0.5541
    paper_std: 0.0596
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5541
    true_std: 0.0596
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5541
    sort_std: 0.0596
    global_rank: 210
    paper_rank: 210
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
    value: 0.5255
    std: 0.038
    paper_value: 0.5255
    paper_std: 0.038
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5255
    true_std: 0.038
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5255
    sort_std: 0.038
    global_rank: 221
    paper_rank: 221
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
    value: 0.5235
    std: 0.0412
    paper_value: 0.5235
    paper_std: 0.0412
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5235
    true_std: 0.0412
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5235
    sort_std: 0.0412
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.5078
    std: 0.0406
    paper_value: 0.5078
    paper_std: 0.0406
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5078
    true_std: 0.0406
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5078
    sort_std: 0.0406
    global_rank: 233
    paper_rank: 233
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
    value: 0.5
    std: 0.0583
    paper_value: 0.5
    paper_std: 0.0583
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5
    true_std: 0.0583
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5
    sort_std: 0.0583
    global_rank: 236
    paper_rank: 236
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.4598
    std: 0.0276
    paper_value: 0.4598
    paper_std: 0.0276
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4598
    true_std: 0.0276
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4598
    sort_std: 0.0276
    global_rank: 241
    paper_rank: 241
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.3745
    std: 0.0709
    paper_value: 0.3745
    paper_std: 0.0709
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3745
    true_std: 0.0709
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3745
    sort_std: 0.0709
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.3353
    std: 0.0492
    paper_value: 0.3353
    paper_std: 0.0492
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for heterophilic datasets as per Geom-GCN/official
      splits.
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
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
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3353
    true_std: 0.0492
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3353
    sort_std: 0.0492
    global_rank: 245
    paper_rank: 245
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
  - *id005
  - *id006
- benchmark: Heterophilic Graphs
  datasets:
  - *id007
  - *id008
  - *id009
  - *id010
  - *id011
  - *id012
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
    - dataset: Wisconsin
      dataset_slug: wisconsin
single_proposed_model: GREET
main_figure: /figures/2211.14065/main_figure.jpegoptim.jpg
---

