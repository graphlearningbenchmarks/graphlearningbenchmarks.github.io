---
title: Scalable Graph Condensation with Evolving Capabilities
arxiv_id: '2502.17614'
source_url: ''
authors:
- name: Shengbo Gong
  orcid: null
  s2_author_id: '2282949117'
  s2_url: null
- name: Mohammad Hashemi
  orcid: null
  s2_author_id: '2282948080'
  s2_url: null
- name: Juntong Ni
  orcid: null
  s2_author_id: '2282011606'
  s2_url: null
- name: Carl Yang
  orcid: null
  s2_author_id: '2307485020'
  s2_url: null
- name: Wei Jin
  orcid: null
  s2_author_id: '2282319889'
  s2_url: null
published_date: Feb 24, 2025
published_date_iso: '2025-02-24'
published_venue: KDD 2025
published_conference: KDD 2025
published_conference_short: KDD
published_conference_slug: kdd
abstract: The rapid growth of graph data creates significant scalability challenges
  as most graph algorithms scale quadratically with size. To mitigate these issues,
  Graph Condensation (GC) methods have been proposed to learn a small graph from a
  larger one, accelerating downstream tasks. However, existing approaches critically
  assume a static training set, which conflicts with the inherently dynamic and evolving
  nature of real-world graph data. This work introduces a novel framework for continual
  graph condensation, enabling efficient updates to the distilled graph that handle
  data streams without requiring costly retraining. This limitation leads to inefficiencies
  when condensing growing training sets. In this paper, we introduce GECC (raph volving
  lustering ondensation), a scalable graph condensation method designed to handle
  large-scale and evolving graph data. GECC employs a traceable and efficient approach
  by performing class-wise clustering on aggregated features. Furthermore, it can
  inherit previous condensation results as clustering centroids when the condensed
  graph expands, thereby attaining an evolving capability. This methodology is supported
  by robust theoretical foundations and demonstrates superior empirical performance.
  Comprehensive experiments including real world scenario show that GECC achieves
  better performance than most state-of-the-art graph condensation methods while delivering
  an around 1000$ $ speedup on large datasets.
codebase_url: https://github.com/Emory-Melody/GraphSlim
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GECC
mrr: 0.0029
adjusted_mrr: 0.001
mrr_dataset_count: 1
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
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
  - model: SimGC
    model_key: simgc
    model_plain: SimGC
    value: 0.664
    std: 0.0015
    paper_value: 0.664
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.738
    at_pub_std: 0.025
    at_pub_source_arxiv: '2403.14951'
    at_pub_source_title: Simple Graph Condensation
    at_pub_source_date_iso: '2024-03-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07399999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.738
    true_std: 0.025
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.07399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.738
    sort_std: 0.025
    global_rank: 290
    paper_rank: 802
    rank_delta: 512
    rank_delta_abs: 512
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Graph Condensation
    comparison_source_arxiv: '2403.14951'
    is_best: false
    is_std_outlier: false
  - model: GECC
    model_key: gecc
    model_plain: GECC
    value: 0.7325
    std: 0.0015
    paper_value: 0.7325
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7325
    true_std: 0.0015
    value_gap_source_arxiv: '2502.17614'
    value_gap_source_title: Scalable Graph Condensation with Evolving Capabilities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7325
    sort_std: 0.0015
    global_rank: 349
    paper_rank: 349
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEOM
    model_key: geom
    model_plain: GEOM
    value: 0.7303
    std: 0.0031
    paper_value: 0.7303
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7303
    true_std: 0.0031
    value_gap_source_arxiv: '2502.17614'
    value_gap_source_title: Scalable Graph Condensation with Evolving Capabilities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7303
    sort_std: 0.0031
    global_rank: 378
    paper_rank: 378
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
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.6262
    std: 0.0063
    paper_value: 0.6262
    paper_std: 0.0063
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
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.7049
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2206.09166'
    at_pub_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    at_pub_source_date_iso: '2022-06-18'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-18'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07869999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7049
    true_std: 0.0008
    value_gap_source_arxiv: '2206.09166'
    value_gap_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    value_gap_source_is_current_paper: false
    value_gap: 0.07869999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7049
    sort_std: 0.0008
    global_rank: 653
    paper_rank: 879
    rank_delta: 226
    rank_delta_abs: 226
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    comparison_source_arxiv: '2206.09166'
    is_best: false
    is_std_outlier: false
  - model: GCDM
    model_key: gcdm
    model_plain: GCDM
    value: 0.6935
    std: 0.0082
    paper_value: 0.6935
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
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.698
    at_pub_std: 0.002
    at_pub_source_arxiv: '2403.14951'
    at_pub_source_title: Simple Graph Condensation
    at_pub_source_date_iso: '2024-03-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0044999999999999485
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.698
    true_std: 0.002
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.0044999999999999485
    has_value_note: false
    value_note: ''
    sort_value: 0.698
    sort_std: 0.002
    global_rank: 696
    paper_rank: 706
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.6666
    std: 0.0054
    paper_value: 0.6666
    paper_std: 0.0054
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
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.69
    at_pub_std: 0.001
    at_pub_source_arxiv: '2403.14951'
    at_pub_source_title: Simple Graph Condensation
    at_pub_source_date_iso: '2024-03-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.023399999999999976
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.69
    true_std: 0.001
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.023399999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.69
    sort_std: 0.001
    global_rank: 716
    paper_rank: 797
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple Graph Condensation
    comparison_source_arxiv: '2403.14951'
    is_best: false
    is_std_outlier: false
  - model: GCondX
    model_key: gcondx
    model_plain: GCondX
    value: 0.6838
    std: 0.0045
    paper_value: 0.6838
    paper_std: 0.0045
    metric: Accuracy
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
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6838
    true_std: 0.0045
    value_gap_source_arxiv: '2502.17614'
    value_gap_source_title: Scalable Graph Condensation with Evolving Capabilities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6838
    sort_std: 0.0045
    global_rank: 741
    paper_rank: 741
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: KCenter
    model_key: kcenter
    model_plain: KCenter
    value: 0.5904
    std: 0.009
    paper_value: 0.5904
    paper_std: 0.009
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
    protocol_note: 'Non-Evolving setting: test accuracy on the final time step using
      the standard Planetoid split.'
    date: Feb 24, 2025
    date_display: Feb 2025
    date_iso: '2025-02-24'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-24'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5904
    true_std: 0.009
    value_gap_source_arxiv: '2502.17614'
    value_gap_source_title: Scalable Graph Condensation with Evolving Capabilities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5904
    sort_std: 0.009
    global_rank: 913
    paper_rank: 913
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: CiteSeer
      dataset_slug: citeseer
single_proposed_model: GECC
main_figure: /figures/2502.17614/main_figure.jpegoptim.jpg
---

