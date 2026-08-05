---
title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive Graph Representation
  Learning
arxiv_id: '2510.12369'
source_url: ''
authors:
- name: Yang Xiang
  orcid: null
  s2_author_id: '2221245673'
  s2_url: null
- name: Li Fan
  orcid: null
  s2_author_id: '2328626590'
  s2_url: null
- name: Chenke Yin
  orcid: null
  s2_author_id: '2291751888'
  s2_url: null
- name: Chengtao Ji
  orcid: null
  s2_author_id: '2329164509'
  s2_url: null
published_date: Oct 14, 2025
published_date_iso: '2025-10-14'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Foundation models in language and vision benefit from a unified discrete
  token interface that converts raw inputs into sequences for scalable pre-training
  and inference. For graphs, an effective tokenizer should yield reusable discrete
  codes that capture both node semantics and relational structure across scales, yet
  prior quantization-based graph tokenizers typically combine residual vector quantization
  (RVQ) levels with fixed rules and often focus on a single structural view, limiting
  cross-task transfer. We present a hierarchical quantized tokenization framework
  with task-conditioned routing and dual-view token streams. It produces multi-scale
  codes and two synchronized sequences: a local stream that preserves node-level information
  and a diffusion-style multi-hop stream that summarizes connectivity. A lightweight
  router learns task-dependent mixtures over RVQ depths to select an appropriate granularity,
  while a gated cross-attention module aligns and fuses the two streams into a single
  token sequence without altering the downstream backbone encoder. Experiments on
  node classification and link prediction show consistent gains over strong quantized
  baselines at matched compute, with ablations verifying contributions from hierarchical
  quantization, adaptive routing, and fusion.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GRIT
- TAU-GRIT
mrr: 0.0955
adjusted_mrr: 0.0955
mrr_dataset_count: 3
benchmark_categories:
- Classic
- GNNBenchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 2
  total: 6
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id003
  dataset: CIFAR10
  rows:
  - model: Tango_GPS
    model_key: randalign
    model_plain: Tango_GPS
    value: 0.7942
    std: 0.00072
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: Apr 15, 2024
    date_display: Apr 2024
    date_iso: '2024-04-15'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7942
    sort_std: 0.00072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: differential encoding
    model_plain: Tango_GPS
    value: 0.79067
    std: 0.00269
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    venue: IEEE Transactions on Big Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.79067
    sort_std: 0.00269
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ppgt
    model_plain: Tango_GPS
    value: 0.7856
    std: 0.007
    metric: Accuracy
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
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7856
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TAU-GRIT
    model_key: tau-grit
    model_plain: TAU-GRIT
    value: 0.77784
    std: 0.0049
    paper_value: 0.77784
    paper_std: 0.0049
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
    protocol_note: Average and std over 5 runs for graph-level classification
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.77784
    true_std: 0.0049
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.77784
    sort_std: 0.0049
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
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.76468
    std: 0.00881
    paper_value: 0.76468
    paper_std: 0.00881
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average and std over 5 runs for graph-level classification
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76468
    at_pub_std: 0.00881
    at_pub_source_arxiv: '2310.20519'
    at_pub_source_title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    at_pub_source_date_iso: '2023-10-31'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76468
    true_std: 0.00881
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76468
    sort_std: 0.00881
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.72298
    std: 0.00356
    paper_value: 0.72298
    paper_std: 0.00356
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average and std over 5 runs for graph-level classification
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.72298
    at_pub_std: 0.00356
    at_pub_source_arxiv: '2408.07654'
    at_pub_source_title: 'Graph Triple Attention Network: A Decoupled Perspective'
    at_pub_source_date_iso: '2024-08-14'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.72298
    true_std: 0.00356
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72298
    sort_std: 0.00356
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.68702
    std: 0.00409
    paper_value: 0.68702
    paper_std: 0.00409
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Average and std over 5 runs for graph-level classification
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.68702
    at_pub_std: 0.00409
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.68702
    true_std: 0.00409
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.68702
    sort_std: 0.00409
    global_rank: 78
    paper_rank: 78
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
- &id002
  dataset: MNIST
  rows:
  - model: Tango_GPS
    model_key: schrödinger gnn
    model_plain: Tango_GPS
    value: 0.9913
    std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9913
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: cnn
    model_plain: Tango_GPS
    value: 0.9907
    std: 0.0007
    metric: Accuracy
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9907
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: mpnn
    model_plain: Tango_GPS
    value: 0.9895
    std: 0.0006
    metric: Accuracy
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9895
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TAU-GRIT
    model_key: tau-grit
    model_plain: TAU-GRIT
    value: 0.98213
    std: 0.00098
    paper_value: 0.98213
    paper_std: 0.00098
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
    protocol_note: Standard graph classification task on MNIST as per Dwivedi et al.
      2023 setup
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98213
    true_std: 0.00098
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98213
    sort_std: 0.00098
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.98173
    std: 0.00087
    paper_value: 0.98173
    paper_std: 0.00087
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST as per Dwivedi et al.
      2023 setup
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98173
    at_pub_std: 0.00087
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98173
    true_std: 0.00087
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98173
    sort_std: 0.00087
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.98108
    std: 0.00111
    paper_value: 0.98108
    paper_std: 0.00111
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
    protocol_note: Standard graph classification task on MNIST as per Dwivedi et al.
      2023 setup
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98108
    at_pub_std: 0.00111
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98108
    true_std: 0.00111
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98108
    sort_std: 0.00111
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.98051
    std: 0.00126
    paper_value: 0.98051
    paper_std: 0.00126
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
    protocol_note: Standard graph classification task on MNIST as per Dwivedi et al.
      2023 setup
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98051
    at_pub_std: 0.00126
    at_pub_source_arxiv: '2408.07654'
    at_pub_source_title: 'Graph Triple Attention Network: A Decoupled Perspective'
    at_pub_source_date_iso: '2024-08-14'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98051
    true_std: 0.00126
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98051
    sort_std: 0.00126
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
  dataset: ZINC
  rows:
  - model: GPS
    model_key: tigt
    model_plain: GPS
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS
    model_key: ppgn++
    model_plain: GPS
    value: 0.02
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_display: Feb 2023
    date_iso: '2023-02-22'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.02
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: subgraphormer
    model_plain: GPS
    value: 0.02
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.02
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.059
    std: 0.002
    paper_value: 0.059
    paper_std: 0.002
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard graph regression task on ZINC; results averaged over 5
      runs.
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.023
    at_pub_std: 0.001
    at_pub_source_arxiv: '2310.20519'
    at_pub_source_title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    at_pub_source_date_iso: '2023-10-31'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.023
    true_std: 0.001
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.036
    has_value_note: false
    value_note: ''
    sort_value: 0.023
    sort_std: 0.001
    global_rank: 8
    paper_rank: 32
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    comparison_source_arxiv: '2310.20519'
    is_best: false
    is_std_outlier: false
  - model: TAU-GRIT
    model_key: tau-grit
    model_plain: TAU-GRIT
    value: 0.051
    std: 0.001
    paper_value: 0.051
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard graph regression task on ZINC; results averaged over 5
      runs.
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.051
    true_std: 0.001
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.051
    sort_std: 0.001
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
- benchmark: Classic
  datasets:
  - *id001
- benchmark: GNNBenchmark
  datasets:
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
    - dataset: CIFAR10
      dataset_slug: cifar10
main_figure: /figures/2510.12369/main_figure.jpegoptim.jpg
---

