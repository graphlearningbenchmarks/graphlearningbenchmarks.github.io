---
title: 'Expressivity and Generalization: Fragment-Biases for Molecular GNNs'
arxiv_id: '2406.08210'
source_url: ''
authors:
- name: Tom Wollschlager
  orcid: null
  s2_author_id: '2220630368'
  s2_url: null
- name: Niklas Kemper
  orcid: null
  s2_author_id: '2305820461'
  s2_url: null
- name: Leon Hetzel
  orcid: null
  s2_author_id: '2120909910'
  s2_url: null
- name: Johanna Sommer
  orcid: null
  s2_author_id: '2064883584'
  s2_url: null
- name: Stephan Günnemann
  orcid: null
  s2_author_id: '2241501445'
  s2_url: null
published_date: Jun 12, 2024
published_date_iso: '2024-06-12'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: Although recent advances in higher-order Graph Neural Networks (GNNs) improve
  the theoretical expressiveness and molecular property predictive performance, they
  often fall short of the empirical performance of models that explicitly use fragment
  information as inductive bias. However, for these approaches, there exists no theoretic
  expressivity study. In this work, we propose the Fragment-WL test, an extension
  to the well-known Weisfeiler&Leman (WL) test, which enables the theoretic analysis
  of these fragment-biased GNNs. Building on the insights gained from the Fragment-WL
  test, we develop a new GNN architecture and a fragmentation with infinite vocabulary
  that significantly boosts expressiveness. We show the effectiveness of our model
  on synthetic and real-world data where we outperform all GNNs on Peptides and have
  12% lower error than all GNNs on ZINC and 34% lower error than other fragment-biased
  models. Furthermore, we show that our model exhibits superior generalization capabilities
  compared to the latest transformer-based architectures, positioning it as a robust
  solution for a range of molecular modeling tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- FragNet
mrr: 0.0244
adjusted_mrr: 0.0081
mrr_dataset_count: 1
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: Peptides-struct
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3496
    std: 0.0013
    paper_value: 0.3496
    paper_std: 0.0013
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.246
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.10360000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2421
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.10750000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2421
    sort_std: 0.0016
    global_rank: 1
    paper_rank: 192
    rank_delta: 191
    rank_delta_abs: 191
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: true
    is_std_outlier: false
  - model: IPR-MPNN
    model_key: ipr-mpnn
    model_plain: IPR-MPNN
    value: 0.2422
    std: 0.0007
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_display: May 2024
    date_iso: '2024-05-27'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.2422
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniGCN
    model_key: unigcn
    model_plain: UniGCN
    value: 0.2425
    std: 0.0009
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.05499'
    title: Unitary convolutions for learning on graphs and groups
    date: Oct 7, 2024
    date_display: Oct 2024
    date_iso: '2024-10-07'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Weber-GeoML/Unitary_Convolutions
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2425
    sort_std: 0.0009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.3547
    std: 0.0045
    paper_value: 0.3547
    paper_std: 0.0045
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3547
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2310.01704'
    at_pub_source_title: Transformers are efficient hierarchical chemical graph learners
    at_pub_source_date_iso: '2023-10-02'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2429
    true_std: 0.0019
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.11180000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2429
    sort_std: 0.0019
    global_rank: 4
    paper_rank: 193
    rank_delta: 189
    rank_delta_abs: 189
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.342
    std: 0.0013
    paper_value: 0.342
    paper_std: 0.0013
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.2477
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09430000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2431
    true_std: 0.002
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.09890000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2431
    sort_std: 0.002
    global_rank: 6
    paper_rank: 191
    rank_delta: 185
    rank_delta_abs: 185
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: true
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.246
    std: 0.0012
    paper_value: 0.246
    paper_std: 0.0012
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.246
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-04-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.246
    true_std: 0.0012
    value_gap_source_arxiv: '2504.12588'
    value_gap_source_title: Plain Transformers Can be Powerful Graph Learners
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.246
    sort_std: 0.0012
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FragNet
    model_key: fragnet
    model_plain: FragNet
    value: 0.2462
    std: 0.0021
    paper_value: 0.2462
    paper_std: 0.0021
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-12'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2462
    true_std: 0.0021
    value_gap_source_arxiv: '2406.08210'
    value_gap_source_title: 'Expressivity and Generalization: Fragment-Biases for
      Molecular GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2462
    sort_std: 0.0021
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
  - model: GatedGCN+RWSE
    model_key: gatedgcn+rwse
    model_plain: GatedGCN+RWSE
    value: 0.3357
    std: 0.0006
    paper_value: 0.3357
    paper_std: 0.0006
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.2529
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2301.11956'
    at_pub_source_title: On the Connection Between MPNN and Graph Transformer
    at_pub_source_date_iso: '2023-01-27'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.08279999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2485
    true_std: 0.0022
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0872
    has_value_note: false
    value_note: ''
    sort_value: 0.2485
    sort_std: 0.0022
    global_rank: 76
    paper_rank: 188
    rank_delta: 112
    rank_delta_abs: 112
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Connection Between MPNN and Graph Transformer
    comparison_source_arxiv: '2301.11956'
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.25
    std: 0.0012
    paper_value: 0.25
    paper_std: 0.0012
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.25
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-06'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.25
    true_std: 0.0005
    value_gap_source_arxiv: '2605.04834'
    value_gap_source_title: Bridging Input Feature Spaces Towards Graph Foundation
      Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.25
    sort_std: 0.0005
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
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.2503
    std: 0.0008
    paper_value: 0.2503
    paper_std: 0.0008
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-12'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2503
    true_std: 0.0008
    value_gap_source_arxiv: '2406.08210'
    value_gap_source_title: 'Expressivity and Generalization: Fragment-Biases for
      Molecular GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2503
    sort_std: 0.0008
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.2523
    std: 0.0013
    paper_value: 0.2523
    paper_std: 0.0013
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.2523
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2306.03561'
    at_pub_source_title: 'CIN++: Enhancing Topological Message Passing'
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-06-12'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2523
    true_std: 0.0013
    value_gap_source_arxiv: '2406.08210'
    value_gap_source_title: 'Expressivity and Generalization: Fragment-Biases for
      Molecular GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2523
    sort_std: 0.0013
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
  - model: SAN+RWSE
    model_key: san+rwse
    model_plain: SAN+RWSE
    value: 0.2545
    std: 0.0012
    paper_value: 0.2545
    paper_std: 0.0012
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.2545
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-07-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2545
    true_std: 0.0012
    value_gap_source_arxiv: '2407.12419'
    value_gap_source_title: Dirac-Bianconi Graph Neural Networks - Enabling Non-Diffusive
      Long-Range Graph Predictions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2545
    sort_std: 0.0012
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
  - model: SAN+LapPE
    model_key: san+lappe
    model_plain: SAN+LapPE
    value: 0.2683
    std: 0.0043
    paper_value: 0.2683
    paper_std: 0.0043
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard Peptides-struct test split
    date: Jun 12, 2024
    date_display: Jun 2024
    date_iso: '2024-06-12'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.2683
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.268
    true_std: 0.004
    value_gap_source_arxiv: '2502.01122'
    value_gap_source_title: Learning Efficient Positional Encodings with Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.268
    sort_std: 0.004
    global_rank: 164
    paper_rank: 164
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
    value: 0.4351
    std: 0.0008
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.03561'
    title: 'CIN++: Enhancing Topological Message Passing'
    date: Jun 6, 2023
    date_display: Jun 2023
    date_iso: '2023-06-06'
    venue: arXiv.org
    codebase_url: https://github.com/twitter-research/cwn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: For both datasets, we did not employ any feature augmentation
      such as positional encoding.
    is_global_top: true
    global_rank: 210
    sort_value: 0.4351
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: Peptides-struct
      dataset_slug: peptides-struct
single_proposed_model: FragNet
main_figure: /figures/2406.08210/main_figure.jpegoptim.jpg
---

