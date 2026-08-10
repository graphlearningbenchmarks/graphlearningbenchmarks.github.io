---
title: Graph External Attention Enhanced Transformer
arxiv_id: '2405.21061'
source_url: ''
authors:
- name: Jianqing Liang
  orcid: null
  s2_author_id: '1864107'
  s2_url: null
- name: Min Chen
  orcid: null
  s2_author_id: '2304363343'
  s2_url: null
- name: Jiye Liang
  orcid: null
  s2_author_id: '2237914945'
  s2_url: null
published_date: May 31, 2024
published_date_iso: '2024-05-31'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: 'The Transformer architecture has recently gained considerable attention
  in the field of graph representation learning, as it naturally overcomes several
  limitations of Graph Neural Networks (GNNs) with customized attention mechanisms
  or positional and structural encodings. Despite making some progress, existing works
  tend to overlook external information of graphs, specifically the correlation between
  graphs. Intuitively, graphs with similar structures should have similar representations.
  Therefore, we propose Graph External Attention (GEA) -- a novel attention mechanism
  that leverages multiple external node/edge key-value units to capture inter-graph
  correlations implicitly. On this basis, we design an effective architecture called
  Graph External Attention Enhanced Transformer (GEAET), which integrates local structure
  and global interaction information for more comprehensive graph representations.
  Extensive experiments on benchmark datasets demonstrate that GEAET achieves state-of-the-art
  empirical performance. The source code is available for reproducibility at: https://github.com/icm1018/GEAET.'
codebase_url: https://github.com/icm1018/GEAET
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GEAET
mrr: 0.1189
adjusted_mrr: 0.1189
mrr_dataset_count: 3
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 3
  total: 5
task_categories:
- link_prediction
- node_classification
experiment_scopes:
- edge-level
- node-level
results:
- &id003
  dataset: COCO-SP
  rows:
  - model: FloydNet
    model_key: floydnet
    model_plain: FloydNet
    value: 0.4901
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_display: Jan 2026
    date_iso: '2026-01-27'
    venue: arXiv.org
    codebase_url: https://github.com/ocx-lab/FloydNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: 'initializes the representation for each pair (i, j)
      as: MLP_init ([G, X_i, X_j, E_ij])'
    is_global_top: true
    global_rank: 1
    sort_value: 0.4901
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CRaWl
    model_key: crawl
    model_plain: CRaWl
    value: 0.4588
    std: 0.0079
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4588
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.444
    std: 0.0065
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.444
    sort_std: 0.0065
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEAET
    model_key: geaet
    model_plain: GEAET
    value: 0.3895
    std: null
    paper_value: 0.3895
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.113235
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: text
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-31'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3895
    true_std: null
    value_gap_source_arxiv: '2405.21061'
    value_gap_source_title: Graph External Attention Enhanced Transformer
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3895
    sort_std: null
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.388
    std: 0.004
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 16
    sort_value: 0.388
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2078
    std: 0.0031
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 48
    sort_value: 0.2078
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.031
    std: 0.016
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 79
    sort_value: 0.031
    sort_std: 0.016
    comparison_type: global_top
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
- &id002
  dataset: PCQM-Contact
  rows:
  - model: FloydNet
    model_key: floydnet
    model_plain: FloydNet
    value: 0.6143
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_display: Jan 2026
    date_iso: '2026-01-27'
    venue: arXiv.org
    codebase_url: https://github.com/ocx-lab/FloydNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: initialization of the relationship tensor... constructed
      by integrating node, edge, and graph-level features
    is_global_top: true
    global_rank: 1
    sort_value: 0.6143
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.4737
    std: 0.0024
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4737
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer + LapPE
    model_key: exphormer + lappe
    model_plain: Exphormer + LapPE
    value: 0.4737
    std: 0.0024
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4737
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.3242
    std: 0.0008
    paper_value: 0.3242
    paper_std: 0.0008
    metric: MRR
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
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3495
    at_pub_std: 0.001
    at_pub_source_arxiv: '2401.01233'
    at_pub_source_title: 'GEN: A Practical Alternative to Graph Transformers for Long-Range
      Graph Modeling'
    at_pub_source_date_iso: '2024-01-02'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.02529999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.467
    true_std: 0.0004
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.14280000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.467
    sort_std: 0.0004
    global_rank: 8
    paper_rank: 74
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GEN: A Practical Alternative to Graph Transformers for
      Long-Range Graph Modeling'
    comparison_source_arxiv: '2401.01233'
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.318
    std: 0.0027
    paper_value: 0.318
    paper_std: 0.0027
    metric: MRR
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
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.318
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4617
    true_std: 0.0005
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.1437
    has_value_note: false
    value_note: ''
    sort_value: 0.4617
    sort_std: 0.0005
    global_rank: 15
    paper_rank: 78
    rank_delta: 63
    rank_delta_abs: 63
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
    value: 0.4617
    std: 0.0005
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.03386'
    title: Learning Long Range Dependencies on Graphs via Random Walks
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/BorgwardtLab/NeuralWalker
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 16
    sort_value: 0.4617
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3234
    std: 0.0006
    paper_value: 0.3234
    paper_std: 0.0006
    metric: MRR
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
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3424
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2401.01233'
    at_pub_source_title: 'GEN: A Practical Alternative to Graph Transformers for Long-Range
      Graph Modeling'
    at_pub_source_date_iso: '2024-01-02'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.01899999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4526
    true_std: 0.0006
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.12919999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4526
    sort_std: 0.0006
    global_rank: 28
    paper_rank: 76
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GEN: A Practical Alternative to Graph Transformers for
      Long-Range Graph Modeling'
    comparison_source_arxiv: '2401.01233'
    is_best: false
    is_std_outlier: false
  - model: GEAET
    model_key: geaet
    model_plain: GEAET
    value: 0.3518
    std: 0.0011
    paper_value: 0.3518
    paper_std: 0.0011
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.113235
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-31'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3518
    true_std: 0.0011
    value_gap_source_arxiv: '2405.21061'
    value_gap_source_title: Graph External Attention Enhanced Transformer
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3518
    sort_std: 0.0011
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
  - model: Graph Diffuser
    model_key: graph diffuser
    model_plain: Graph Diffuser
    value: 0.3388
    std: 0.0011
    paper_value: 0.3388
    paper_std: 0.0011
    metric: MRR
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
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.3388
    true_std: 0.0011
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3388
    sort_std: 0.0011
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
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.3341
    std: 0.0006
    paper_value: 0.3341
    paper_std: 0.0006
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.335
    true_std: 0.0003
    value_gap_source_arxiv: '2410.09737'
    value_gap_source_title: Towards Stable, Globally Expressive Graph Representations
      with Laplacian Eigenvectors
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.335
    sort_std: 0.0003
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer
    model_key: transformer
    model_plain: Transformer
    value: 0.3174
    std: 0.002
    paper_value: 0.3174
    paper_std: 0.002
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: LRGB
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3174
    true_std: 0.002
    value_gap_source_arxiv: '2410.09737'
    value_gap_source_title: Towards Stable, Globally Expressive Graph Representations
      with Laplacian Eigenvectors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3174
    sort_std: 0.002
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: PascalVOC-SP
  rows:
  - model: NeuralWalker
    model_key: neuralwalker
    model_plain: NeuralWalker
    value: 0.4912
    std: 0.0042
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/goombalab/chimera
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.4912
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PPGT
    model_key: ppgt
    model_plain: PPGT
    value: 0.4641
    std: 0.0033
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: utilize relative random walk probabilities (RRWP) as
      our demonstrating example of graph PE
    is_global_top: true
    global_rank: 2
    sort_value: 0.4641
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CRaWl
    model_key: crawl
    model_plain: CRaWl
    value: 0.4588
    std: 0.0079
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports 45.88 +/- 0.79 percent; normalize both values
      to fractions.
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4588
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEAET
    model_key: geaet
    model_plain: GEAET
    value: 0.4585
    std: null
    paper_value: 0.4585
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.113235
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: text
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-31'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4585
    true_std: null
    value_gap_source_arxiv: '2405.21061'
    value_gap_source_title: Graph External Attention Enhanced Transformer
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4585
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.388
    std: 0.004
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 44
    sort_value: 0.388
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.238
    std: 0.016
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 86
    sort_value: 0.238
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.114
    std: 0.023
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 101
    sort_value: 0.114
    sort_std: 0.023
    comparison_type: global_top
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
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PascalVOC-SP
      dataset_slug: pascalvoc-sp
    - dataset: COCO-SP
      dataset_slug: coco-sp
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PCQM-Contact
      dataset_slug: pcqm-contact
single_proposed_model: GEAET
main_figure: /figures/2405.21061/main_figure.jpegoptim.jpg
---

