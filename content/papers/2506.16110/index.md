---
title: Mitigating Over-Squashing in Graph Neural Networks by Spectrum-Preserving Sparsification
arxiv_id: '2506.16110'
source_url: ''
authors:
- name: Langzhang Liang
  orcid: null
  s2_author_id: '2155276820'
  s2_url: null
- name: Fanchen Bu
  orcid: null
  s2_author_id: '2367734491'
  s2_url: null
- name: Zixing Song
  orcid: null
  s2_author_id: '2114791973'
  s2_url: null
- name: Zenglin Xu
  orcid: null
  s2_author_id: '2298925809'
  s2_url: null
- name: Shirui Pan
  orcid: null
  s2_author_id: '2304445964'
  s2_url: null
- name: Kijung Shin
  orcid: null
  s2_author_id: '2242112674'
  s2_url: null
published_date: Jun 19, 2025
published_date_iso: '2025-06-19'
published_venue: ICML 2025
published_conference: ICML 2025
published_conference_short: ICML
published_conference_slug: icml
abstract: The message-passing paradigm of Graph Neural Networks often struggles with
  exchanging information across distant nodes typically due to structural bottlenecks
  in certain graph regions, a limitation known as over-squashing. To reduce such bottlenecks,
  graph rewiring, which modifies graph topology, has been widely used. However, existing
  graph rewiring techniques often overlook the need to preserve critical properties
  of the original graph, e.g., spectral properties. Moreover, many approaches rely
  on increasing edge count to improve connectivity, which introduces significant computational
  overhead and exacerbates the risk of over-smoothing. In this paper, we propose a
  novel graph rewiring method that leverages spectrum-preserving graph sparsification,
  for mitigating over-squashing. Our method generates graphs with enhanced connectivity
  while maintaining sparsity and largely preserving the original graph spectrum, effectively
  balancing structural bottleneck reduction and graph property preservation. Experimental
  results validate the effectiveness of our approach, demonstrating its superiority
  over strong baseline methods in classification accuracy and retention of the Laplacian
  spectrum.
codebase_url: https://github.com/Jinx-byebye/GOKU
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GOKU
mrr: 0.0029
adjusted_mrr: 0.0029
mrr_dataset_count: 4
benchmark_categories:
- TU Dortmund
- Heterophilic Graphs
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id004
  dataset: Cornell
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: acm-gcn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: rf-gcn
    model_plain: R-SoftGraphAIN
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
  - model: GOKU
    model_key: goku
    model_plain: GOKU
    value: 0.694
    std: 0.021
    paper_value: 0.694
    paper_std: 0.021
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
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.694
    true_std: 0.021
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.694
    sort_std: 0.021
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
  - model: DR
    model_key: dr
    model_plain: DR
    value: 0.679
    std: 0.047
    paper_value: 0.679
    paper_std: 0.047
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
    protocol_note: Node classification using GCNII backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.679
    true_std: 0.047
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.679
    sort_std: 0.047
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
  - model: LASER
    model_key: laser
    model_plain: LASER
    value: 0.608
    std: 0.036
    paper_value: 0.608
    paper_std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GCNII backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.608
    true_std: 0.036
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.608
    sort_std: 0.036
    global_rank: 388
    paper_rank: 388
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTR
    model_key: gtr
    model_plain: GTR
    value: 0.592
    std: 0.048
    paper_value: 0.592
    paper_std: 0.048
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
    protocol_note: Node classification using GCNII backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.048
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.048
    global_rank: 405
    paper_rank: 405
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDRF
    model_key: sdrf
    model_plain: SDRF
    value: 0.422
    std: 0.015
    paper_value: 0.422
    paper_std: 0.015
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
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.546
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2111.14522'
    at_pub_source_title: Understanding over-squashing and bottlenecks on graphs via
      curvature
    at_pub_source_date_iso: '2021-11-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-11-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.12400000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.546
    true_std: 0.0039
    value_gap_source_arxiv: '2111.14522'
    value_gap_source_title: Understanding over-squashing and bottlenecks on graphs
      via curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.12400000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.546
    sort_std: 0.0039
    global_rank: 459
    paper_rank: 556
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding over-squashing and bottlenecks on graphs
      via curvature
    comparison_source_arxiv: '2111.14522'
    is_best: false
    is_std_outlier: false
  - model: None
    model_key: none
    model_plain: None
    value: 0.415
    std: 0.018
    paper_value: 0.415
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5366
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2407.09381'
    at_pub_source_title: The Effectiveness of Curvature-Based Rewiring and the Role
      of Hyperparameters in GNNs Revisited
    at_pub_source_date_iso: '2024-07-12'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-07-12'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.12159999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5366
    true_std: 0.0014
    value_gap_source_arxiv: '2407.09381'
    value_gap_source_title: The Effectiveness of Curvature-Based Rewiring and the
      Role of Hyperparameters in GNNs Revisited
    value_gap_source_is_current_paper: false
    value_gap: 0.12159999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.5366
    sort_std: 0.0014
    global_rank: 474
    paper_rank: 558
    rank_delta: 84
    rank_delta_abs: 84
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: The Effectiveness of Curvature-Based Rewiring and the
      Role of Hyperparameters in GNNs Revisited
    comparison_source_arxiv: '2407.09381'
    is_best: false
    is_std_outlier: false
  - model: BORF
    model_key: borf
    model_plain: BORF
    value: 0.508
    std: 0.011
    paper_value: 0.508
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.508
    true_std: 0.011
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.508
    sort_std: 0.011
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
  - model: FoSR
    model_key: fosr
    model_plain: FoSR
    value: 0.402
    std: 0.016
    paper_value: 0.402
    paper_std: 0.016
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
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4416
    true_std: 0.0146
    value_gap_source_arxiv: '2508.20597'
    value_gap_source_title: Local Virtual Nodes for Alleviating Over-Squashing in
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03959999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4416
    sort_std: 0.0146
    global_rank: 544
    paper_rank: 564
    rank_delta: 20
    rank_delta_abs: 20
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
- &id002
  dataset: ENZYMES
  rows:
  - model: WL
    model_key: bgnn(m)-cs
    model_plain: WL
    value: 0.8068
    std: 0.0149
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8068
    sort_std: 0.0149
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: bgnn
    model_plain: WL
    value: 0.7936
    std: 0.0281
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7936
    sort_std: 0.0281
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: bgnn(m)-sc
    model_plain: WL
    value: 0.7889
    std: 0.0079
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7889
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FoSR
    model_key: fosr
    model_plain: FoSR
    value: 0.288
    std: 0.01
    paper_value: 0.288
    paper_std: 0.01
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.4555
    at_pub_std: 0.01258
    at_pub_source_arxiv: '2210.11790'
    at_pub_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    at_pub_source_date_iso: '2022-10-21'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-21'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.16750000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4555
    true_std: 0.01258
    value_gap_source_arxiv: '2210.11790'
    value_gap_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.16750000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.4555
    sort_std: 0.01258
    global_rank: 200
    paper_rank: 273
    rank_delta: 73
    rank_delta_abs: 73
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    comparison_source_arxiv: '2210.11790'
    is_best: false
    is_std_outlier: false
  - model: SDRF
    model_key: sdrf
    model_plain: SDRF
    value: 0.324
    std: 0.013
    paper_value: 0.324
    paper_std: 0.013
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.39583
    at_pub_std: 0.01333
    at_pub_source_arxiv: '2210.11790'
    at_pub_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    at_pub_source_date_iso: '2022-10-21'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-21'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.07183
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.39583
    true_std: 0.01333
    value_gap_source_arxiv: '2210.11790'
    value_gap_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.07183
    has_value_note: false
    value_note: ''
    sort_value: 0.39583
    sort_std: 0.01333
    global_rank: 226
    paper_rank: 254
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    comparison_source_arxiv: '2210.11790'
    is_best: false
    is_std_outlier: false
  - model: None
    model_key: none
    model_plain: None
    value: 0.335
    std: 0.013
    paper_value: 0.335
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.39017
    at_pub_std: 0.01166
    at_pub_source_arxiv: '2210.11790'
    at_pub_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    at_pub_source_date_iso: '2022-10-21'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-10-21'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.05517
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.39017
    true_std: 0.01166
    value_gap_source_arxiv: '2210.11790'
    value_gap_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.05517
    has_value_note: false
    value_note: ''
    sort_value: 0.39017
    sort_std: 0.01166
    global_rank: 227
    paper_rank: 251
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    comparison_source_arxiv: '2210.11790'
    is_best: false
    is_std_outlier: false
  - model: BORF
    model_key: borf
    model_plain: BORF
    value: 0.314
    std: 0.015
    paper_value: 0.314
    paper_std: 0.015
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.355
    at_pub_std: 0.012
    at_pub_source_arxiv: '2211.15779'
    at_pub_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    at_pub_source_date_iso: '2022-11-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-11-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.04099999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.355
    true_std: 0.012
    value_gap_source_arxiv: '2211.15779'
    value_gap_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.04099999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.355
    sort_std: 0.012
    global_rank: 243
    paper_rank: 256
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    comparison_source_arxiv: '2211.15779'
    is_best: false
    is_std_outlier: false
  - model: LASER
    model_key: laser
    model_plain: LASER
    value: 0.353
    std: 0.013
    paper_value: 0.353
    paper_std: 0.013
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.34333
    at_pub_std: 0.06936
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.009669999999999956
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.353
    true_std: 0.013
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.353
    sort_std: 0.013
    global_rank: 245
    paper_rank: 245
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOKU
    model_key: goku
    model_plain: GOKU
    value: 0.338
    std: 0.012
    paper_value: 0.338
    paper_std: 0.012
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.338
    true_std: 0.012
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.338
    sort_std: 0.012
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
  - model: GTR
    model_key: gtr
    model_plain: GTR
    value: 0.284
    std: 0.018
    paper_value: 0.284
    paper_std: 0.018
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: GIN backbone on Enzymes dataset
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.26333
    at_pub_std: 0.05821
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.020669999999999966
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.284
    true_std: 0.018
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.284
    sort_std: 0.018
    global_rank: 275
    paper_rank: 275
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
  - model: LASER
    model_key: laser
    model_plain: LASER
    value: 0.803
    std: 0.016
    paper_value: 0.803
    paper_std: 0.016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GCNII backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.82204
    at_pub_std: 0.06728
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.019039999999999946
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.82204
    true_std: 0.06728
    value_gap_source_arxiv: '2310.01668'
    value_gap_source_title: Locality-Aware Graph Rewiring in GNNs
    value_gap_source_is_current_paper: false
    value_gap: 0.019039999999999946
    has_value_note: false
    value_note: ''
    sort_value: 0.82204
    sort_std: 0.06728
    global_rank: 566
    paper_rank: 619
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOKU
    model_key: goku
    model_plain: GOKU
    value: 0.818
    std: 0.014
    paper_value: 0.818
    paper_std: 0.014
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GCNII backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.818
    true_std: 0.014
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.818
    sort_std: 0.014
    global_rank: 580
    paper_rank: 580
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BORF
    model_key: borf
    model_plain: BORF
    value: 0.782
    std: 0.016
    paper_value: 0.782
    paper_std: 0.016
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GIN backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.81684
    at_pub_std: 0.07964
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.03483999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.81684
    true_std: 0.07964
    value_gap_source_arxiv: '2310.01668'
    value_gap_source_title: Locality-Aware Graph Rewiring in GNNs
    value_gap_source_is_current_paper: false
    value_gap: 0.03483999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.81684
    sort_std: 0.07964
    global_rank: 583
    paper_rank: 664
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DR
    model_key: dr
    model_plain: DR
    value: 0.816
    std: 0.017
    paper_value: 0.816
    paper_std: 0.017
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GCNII backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.816
    true_std: 0.017
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.816
    sort_std: 0.017
    global_rank: 585
    paper_rank: 585
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FoSR
    model_key: fosr
    model_plain: FoSR
    value: 0.756
    std: 0.017
    paper_value: 0.756
    paper_std: 0.017
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GCN backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.75895
    at_pub_std: 0.07211
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.002950000000000008
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.804
    true_std: 0.0243
    value_gap_source_arxiv: '2508.20597'
    value_gap_source_title: Local Virtual Nodes for Alleviating Over-Squashing in
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04800000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.804
    sort_std: 0.0243
    global_rank: 613
    paper_rank: 710
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDRF
    model_key: sdrf
    model_plain: SDRF
    value: 0.795
    std: 0.026
    paper_value: 0.795
    paper_std: 0.026
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GIN backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.773
    at_pub_std: 0.023
    at_pub_source_arxiv: '2211.15779'
    at_pub_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    at_pub_source_date_iso: '2022-11-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.02200000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.795
    true_std: 0.026
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.795
    sort_std: 0.026
    global_rank: 642
    paper_rank: 642
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTR
    model_key: gtr
    model_plain: GTR
    value: 0.79
    std: 0.014
    paper_value: 0.79
    paper_std: 0.014
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GCNII backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.78632
    at_pub_std: 0.06201
    at_pub_source_arxiv: '2310.01668'
    at_pub_source_title: Locality-Aware Graph Rewiring in GNNs
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0036800000000000166
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.79
    true_std: 0.014
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: 0.014
    global_rank: 653
    paper_rank: 653
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: None
    model_key: none
    model_plain: None
    value: 0.761
    std: 0.031
    paper_value: 0.761
    paper_std: 0.031
    metric: Accuracy
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on Mutag using GIN backbone.
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.755
    at_pub_std: 0.029
    at_pub_source_arxiv: '2211.15779'
    at_pub_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    at_pub_source_date_iso: '2022-11-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.761
    true_std: 0.031
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.761
    sort_std: 0.031
    global_rank: 700
    paper_rank: 700
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: Texas
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: gpf-plus
    model_plain: R-SoftGraphAIN
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
  - model: GOKU
    model_key: goku
    model_plain: GOKU
    value: 0.724
    std: 0.022
    paper_value: 0.724
    paper_std: 0.022
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
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.724
    true_std: 0.022
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.724
    sort_std: 0.022
    global_rank: 397
    paper_rank: 397
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DR
    model_key: dr
    model_plain: DR
    value: 0.678
    std: 0.025
    paper_value: 0.678
    paper_std: 0.025
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
    source_ref: Attali et al. 2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.678
    true_std: 0.025
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.678
    sort_std: 0.025
    global_rank: 440
    paper_rank: 440
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDRF
    model_key: sdrf
    model_plain: SDRF
    value: 0.445
    std: 0.039
    paper_value: 0.445
    paper_std: 0.039
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
    source_ref: Topping et al. 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GIN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6446
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2111.14522'
    at_pub_source_title: Understanding over-squashing and bottlenecks on graphs via
      curvature
    at_pub_source_date_iso: '2021-11-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-03-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.19959999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6446
    true_std: 0.0038
    value_gap_source_arxiv: '2603.26178'
    value_gap_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    value_gap_source_is_current_paper: false
    value_gap: 0.19959999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6446
    sort_std: 0.0038
    global_rank: 483
    paper_rank: 633
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding over-squashing and bottlenecks on graphs
      via curvature
    comparison_source_arxiv: '2111.14522'
    is_best: false
    is_std_outlier: false
  - model: BORF
    model_key: borf
    model_plain: BORF
    value: 0.499
    std: 0.034
    paper_value: 0.499
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
    source_ref: Nguyen et al. 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GIN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.631
    at_pub_std: 0.017
    at_pub_source_arxiv: '2211.15779'
    at_pub_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    at_pub_source_date_iso: '2022-11-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-11-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.132
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.631
    true_std: 0.017
    value_gap_source_arxiv: '2211.15779'
    value_gap_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.132
    has_value_note: false
    value_note: ''
    sort_value: 0.631
    sort_std: 0.017
    global_rank: 498
    paper_rank: 616
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    comparison_source_arxiv: '2211.15779'
    is_best: false
    is_std_outlier: false
  - model: None
    model_key: none
    model_plain: None
    value: 0.464
    std: 0.045
    paper_value: 0.464
    paper_std: 0.045
    metric: Accuracy
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
    protocol_note: Node classification using GIN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.778
    at_pub_std: 0.012
    at_pub_source_arxiv: '2201.12843'
    at_pub_source_title: Graph Representation Learning via Aggregation Enhancement
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2021-11-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.314
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6119
    true_std: 0.0049
    value_gap_source_arxiv: '2111.14522'
    value_gap_source_title: Understanding over-squashing and bottlenecks on graphs
      via curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.14789999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6119
    sort_std: 0.0049
    global_rank: 523
    paper_rank: 630
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Representation Learning via Aggregation Enhancement
    comparison_source_arxiv: '2201.12843'
    is_best: false
    is_std_outlier: false
  - model: FoSR
    model_key: fosr
    model_plain: FoSR
    value: 0.46
    std: 0.016
    paper_value: 0.46
    paper_std: 0.016
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
    source_ref: Karhadkar et al. 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GCN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.47
    at_pub_std: 0.037
    at_pub_source_arxiv: '2211.15779'
    at_pub_source_title: Revisiting Over-smoothing and Over-squashing using Ollivier's
      Ricci Curvature
    at_pub_source_date_iso: '2022-11-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-08-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.009999999999999953
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5286
    true_std: 0.0172
    value_gap_source_arxiv: '2508.20597'
    value_gap_source_title: Local Virtual Nodes for Alleviating Over-Squashing in
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06859999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.5286
    sort_std: 0.0172
    global_rank: 611
    paper_rank: 630
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTR
    model_key: gtr
    model_plain: GTR
    value: 0.495
    std: 0.029
    paper_value: 0.495
    paper_std: 0.029
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
    source_ref: Black et al. 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GIN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.495
    true_std: 0.029
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.495
    sort_std: 0.029
    global_rank: 619
    paper_rank: 619
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LASER
    model_key: laser
    model_plain: LASER
    value: 0.465
    std: 0.045
    paper_value: 0.465
    paper_std: 0.045
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: Barbero et al. 2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification using GIN backbone
    date: Jun 19, 2025
    date_display: Jun 2025
    date_iso: '2025-06-19'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-19'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.465
    true_std: 0.045
    value_gap_source_arxiv: '2506.16110'
    value_gap_source_title: Mitigating Over-Squashing in Graph Neural Networks by
      Spectrum-Preserving Sparsification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.465
    sort_std: 0.045
    global_rank: 630
    paper_rank: 630
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
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
- benchmark: Heterophilic Graphs
  datasets:
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: GOKU
main_figure: /figures/2506.16110/main_figure.jpegoptim.jpg
---

