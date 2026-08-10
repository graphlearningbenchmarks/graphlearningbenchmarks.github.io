---
title: 'OpenGraph: Towards Open Graph Foundation Models'
arxiv_id: '2403.01121'
source_url: ''
authors:
- name: Lianghao Xia
  orcid: null
  s2_author_id: '1830455155'
  s2_url: null
- name: Ben Kao
  orcid: null
  s2_author_id: '2289844482'
  s2_url: null
- name: Chao Huang
  orcid: null
  s2_author_id: '2261248317'
  s2_url: null
published_date: Mar 2, 2024
published_date_iso: '2024-03-02'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph learning has become essential in various domains, including recommendation
  systems and social network analysis. Graph Neural Networks (GNNs) have emerged as
  promising techniques for encoding structural information and improving performance
  in tasks like link prediction and node classification. However, a key challenge
  remains: the difficulty of generalizing to unseen graph data with different properties.
  In this work, we propose a novel graph foundation model, called OpenGraph, to address
  this challenge. Our approach tackles several technical obstacles. Firstly, we enhance
  data augmentation using a large language model (LLM) to overcome data scarcity in
  real-world scenarios. Secondly, we introduce a unified graph tokenizer that enables
  the model to generalize effectively to diverse graph data, even when encountering
  unseen properties during training. Thirdly, our developed scalable graph transformer
  captures node-wise dependencies within the global topological context. Extensive
  experiments validate the effectiveness of our framework. By adapting OpenGraph\
  to new graph characteristics and comprehending diverse graphs, our approach achieves
  remarkable zero-shot graph learning performance across various settings. We release
  the model implementation at https://github.com/HKUDS/OpenGraph.'
codebase_url: https://github.com/HKUDS/OpenGraph
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- OpenGraph
mrr: 0.0016
adjusted_mrr: 0.001
mrr_dataset_count: 2
benchmark_categories:
- Classic
- OGB
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- link_prediction
- node_classification
experiment_scopes:
- edge-level
- node-level
results:
- &id002
  dataset: CiteSeer
  is_multi_metric: true
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
    metric_values:
    - 0.9575
    - null
    metric_stds:
    - 0.0058
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    published_venue: ''
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9575
    sort_std: 0.0058
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
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    metric_values:
    - 0.939
    - null
    metric_stds:
    - 0.0187
    - null
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
    published_venue: ''
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.939
    sort_std: 0.0187
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
  - model: EERM
    model_key: eerm
    model_plain: EERM
    metric_values:
    - 0.9112
    - null
    metric_stds:
    - 0.0145
    - null
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
    published_venue: ''
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9112
    sort_std: 0.0145
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.8774
    - null
    metric_stds:
    - 0.0041
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    published_venue: ''
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    is_global_top: true
    global_rank: 20
    is_best: false
    sort_value: 0.8774
    sort_std: 0.0041
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.32
    - 0.2096
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8769
    sort_std: 0.004
    true_value: 0.8769
    true_std: 0.004
    paper_value: 0.32
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5569
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_note: ''
    at_pub_value: 0.8769
    at_pub_std: 0.004
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.5569
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.281
    - 0.2025
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.808
    sort_std: 0.0026
    true_value: 0.808
    true_std: 0.0026
    paper_value: 0.281
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.527
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_note: ''
    at_pub_value: 0.808
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.527
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
    global_rank: 46
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.284
    - 0.1791
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.789
    sort_std: 0.002
    true_value: 0.789
    true_std: 0.002
    paper_value: 0.284
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5050000000000001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_note: ''
    at_pub_value: 0.789
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.5050000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
    global_rank: 83
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.282
    - 0.1705
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7618
    sort_std: 0.0078
    true_value: 0.7618
    true_std: 0.0078
    paper_value: 0.282
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.47980000000000006
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_note: ''
    at_pub_value: 0.7618
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.47980000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
    global_rank: 165
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.259
    - 0.1993
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7289
    sort_std: 0.001
    true_value: 0.7289
    true_std: 0.001
    paper_value: 0.259
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.4699
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_note: ''
    at_pub_value: 0.719
    at_pub_std: 0.0169
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.45999999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
    global_rank: 401
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    metric_values:
    - 0.298
    - 0.163
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.725
    sort_std: 0.007
    true_value: 0.725
    true_std: 0.007
    paper_value: 0.298
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.427
    value_gap_source_arxiv: '2207.11996'
    value_gap_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    value_note: ''
    at_pub_value: 0.725
    at_pub_std: 0.007
    at_pub_source_arxiv: '2207.11996'
    at_pub_source_title: Generative Subgraph Contrast for Self-Supervised Graph Representation
      Learning
    at_pub_source_date_iso: '2022-07-25'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-07-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.427
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    comparison_source_arxiv: '2207.11996'
    is_best: false
    is_std_outlier: false
    global_rank: 446
  - model: OpenGraph
    model_key: opengraph
    model_plain: OpenGraph
    metric_values:
    - 0.7221
    - null
    metric_stds:
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7221
    sort_std: null
    true_value: 0.7221
    true_std: null
    paper_value: 0.7221
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
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
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 493
  - model: GPrompt
    model_key: gprompt
    model_plain: GPrompt
    metric_values:
    - 0.28
    - 0.1519
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.5321
    sort_std: 0.1094
    true_value: 0.5321
    true_std: 0.1094
    paper_value: 0.28
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.2521
    value_gap_source_arxiv: '2406.05346'
    value_gap_source_title: 'ProG: A Graph Prompt Learning Benchmark'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
    global_rank: 941
  - model: GPF
    model_key: gpf
    model_plain: GPF
    metric_values:
    - 0.311
    - 0.1984
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4902
    sort_std: 0.0453
    true_value: 0.4902
    true_std: 0.0453
    paper_value: 0.311
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.17920000000000003
    value_gap_source_arxiv: '2602.05567'
    value_gap_source_title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph
      Neural Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 953
  - model: MF
    model_key: mf
    model_plain: MF
    metric_values:
    - 0.174
    - 0.1727
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.174
    sort_std: null
    true_value: 0.174
    true_std: null
    paper_value: 0.174
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
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
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 989
  metrics:
  - Accuracy
  - F1
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - F1
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: PubMed
  is_multi_metric: true
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    metric_values:
    - 0.9518
    - null
    metric_stds:
    - 0.0011
    - null
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
    published_venue: ''
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9518
    sort_std: 0.0011
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
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    metric_values:
    - 0.9513
    - null
    metric_stds:
    - 0.0038
    - null
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
    published_venue: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.9513
    sort_std: 0.0038
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
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    metric_values:
    - 0.9511
    - null
    metric_stds:
    - 0.0036
    - null
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
    published_venue: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.9511
    sort_std: 0.0036
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.427
    - 0.3296
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9296
    sort_std: 0.0015
    true_value: 0.9296
    true_std: 0.0015
    paper_value: 0.427
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5025999999999999
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_note: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.47000000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.472
    - 0.3657
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9233
    sort_std: 0.0018
    true_value: 0.9233
    true_std: 0.0018
    paper_value: 0.472
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.45130000000000003
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_note: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.42500000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.8881
    - null
    metric_stds:
    - 0.0015
    - null
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
    published_venue: ''
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 134
    is_best: false
    sort_value: 0.8881
    sort_std: 0.0015
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.441
    - 0.3064
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.881
    sort_std: null
    true_value: 0.881
    true_std: null
    paper_value: 0.441
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.44
    value_gap_source_arxiv: '2308.10737'
    value_gap_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    value_note: ''
    at_pub_value: 0.881
    at_pub_std: null
    at_pub_source_arxiv: '2308.10737'
    at_pub_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    at_pub_source_date_iso: '2023-08-21'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-21'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.44
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    comparison_source_arxiv: '2308.10737'
    is_best: false
    is_std_outlier: false
    global_rank: 181
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.429
    - 0.3163
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8708
    sort_std: 0.0017
    true_value: 0.8708
    true_std: 0.0017
    paper_value: 0.429
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.4418
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_note: ''
    at_pub_value: 0.8703
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.44129999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
    global_rank: 235
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.443
    - 0.3114
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.869
    sort_std: 0.0074
    true_value: 0.869
    true_std: 0.0074
    paper_value: 0.443
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.426
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_note: ''
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.426
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
    global_rank: 243
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    metric_values:
    - 0.407
    - 0.413
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8196
    sort_std: 0.0073
    true_value: 0.8196
    true_std: 0.0073
    paper_value: 0.407
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.4126
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_note: ''
    at_pub_value: 0.8196
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.4126
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
    global_rank: 376
  - model: OpenGraph
    model_key: opengraph
    model_plain: OpenGraph
    metric_values:
    - 0.6869
    - 0.6537
    metric_stds:
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6869
    sort_std: null
    true_value: 0.6869
    true_std: null
    paper_value: 0.6869
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
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
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 933
  - model: GPF
    model_key: gpf
    model_plain: GPF
    metric_values:
    - 0.422
    - 0.267
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5716
    sort_std: 0.1099
    true_value: 0.5716
    true_std: 0.1099
    paper_value: 0.422
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.1496
    value_gap_source_arxiv: '2502.08092'
    value_gap_source_title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-12'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
    global_rank: 957
  - model: GPrompt
    model_key: gprompt
    model_plain: GPrompt
    metric_values:
    - 0.471
    - 0.3705
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.471
    sort_std: null
    true_value: 0.471
    true_std: null
    paper_value: 0.471
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
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
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 961
  - model: MF
    model_key: mf
    model_plain: MF
    metric_values:
    - 0.347
    - 0.3346
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.347
    sort_std: null
    true_value: 0.347
    true_std: null
    paper_value: 0.347
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
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
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 975
  metrics:
  - Accuracy
  - F1
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - F1
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: ogbl-ddi
  rows:
  - model: OpenGraph
    model_key: opengraph
    model_plain: OpenGraph
    value: 0.0921
    std: null
    paper_value: 0.0921
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Zero-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0921
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0921
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF
    model_key: gpf
    model_plain: GPF
    value: 0.0839
    std: null
    paper_value: 0.0839
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0839
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0839
    sort_std: null
    global_rank: 2
    paper_rank: 2
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
    value: 0.0821
    std: null
    paper_value: 0.0821
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0821
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0821
    sort_std: null
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
  - model: GPrompt
    model_key: gprompt
    model_plain: GPrompt
    value: 0.0769
    std: null
    paper_value: 0.0769
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0769
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0769
    sort_std: null
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.074
    std: null
    paper_value: 0.074
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.074
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.074
    sort_std: null
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.0735
    std: null
    paper_value: 0.0735
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0735
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0735
    sort_std: null
    global_rank: 6
    paper_rank: 6
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
    value: 0.0711
    std: null
    paper_value: 0.0711
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0711
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0711
    sort_std: null
    global_rank: 7
    paper_rank: 7
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
    value: 0.0705
    std: null
    paper_value: 0.0705
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0705
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0705
    sort_std: null
    global_rank: 8
    paper_rank: 8
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
    value: 0.0621
    std: null
    paper_value: 0.0621
    paper_std: null
    metric: Recall@20
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0621
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0621
    sort_std: null
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
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.0536
    std: null
    paper_value: 0.0536
    paper_std: null
    metric: Recall@20
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Five-shot evaluation on ogbl-ddi link prediction task.
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0536
    true_std: null
    value_gap_source_arxiv: '2403.01121'
    value_gap_source_title: 'OpenGraph: Towards Open Graph Foundation Models'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0536
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Recall@20
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@20
  paper_metrics:
  - Recall@20
  metric: Recall@20
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: OGB
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-ddi
      dataset_slug: ogbl-ddi
single_proposed_model: OpenGraph
main_figure: /figures/2403.01121/main_figure.jpegoptim.jpg
---

