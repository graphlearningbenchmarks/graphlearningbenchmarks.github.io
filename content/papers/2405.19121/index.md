---
title: Spatio-Spectral Graph Neural Networks
arxiv_id: '2405.19121'
source_url: ''
authors:
- name: Simon Geisler
  orcid: null
  s2_author_id: '79462643'
  s2_url: null
- name: Arthur Kosmala
  orcid: null
  s2_author_id: '2192604719'
  s2_url: null
- name: Daniel C. Herbst
  orcid: null
  s2_author_id: '2303656359'
  s2_url: null
- name: Stephan Gunnemann
  orcid: null
  s2_author_id: '51249380'
  s2_url: null
published_date: May 29, 2024
published_date_iso: '2024-05-29'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Spatial Message Passing Graph Neural Networks (MPGNNs) are widely used for
  learning on graph-structured data. However, key limitations of l-step MPGNNs are
  that their"receptive field"is typically limited to the l-hop neighborhood of a node
  and that information exchange between distant nodes is limited by over-squashing.
  Motivated by these limitations, we propose Spatio-Spectral Graph Neural Networks
  (S$^2$GNNs) -- a new modeling paradigm for Graph Neural Networks (GNNs) that synergistically
  combines spatially and spectrally parametrized graph filters. Parameterizing filters
  partially in the frequency domain enables global yet efficient information propagation.
  We show that S$^2$GNNs vanquish over-squashing and yield strictly tighter approximation-theoretic
  error bounds than MPGNNs. Further, rethinking graph convolutions at a fundamental
  level unlocks new design spaces. For example, S$^2$GNNs allow for free positional
  encodings that make them strictly more expressive than the 1-Weisfeiler-Lehman (WL)
  test. Moreover, to obtain general-purpose S$^2$GNNs, we propose spectrally parametrized
  filters for directed graphs. S$^2$GNNs outperform spatial MPGNNs, graph transformers,
  and graph rewirings, e.g., on the peptide long-range benchmark tasks, and are competitive
  with state-of-the-art sequence modeling. On a 40 GB GPU, S$^2$GNNs scale to millions
  of nodes.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- LRGB
- GNNBenchmark
- LINKX Benchmarks
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 2
  total: 5
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- graph_classification
- graph_regression
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id004
  dataset: CLUSTER
  rows:
  - model: Tango_GPS
    model_key: grpe-small
    model_plain: Tango_GPS
    value: 0.81586
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 489.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.81586
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.80113
    std: 0.00138
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.80113
    sort_std: 0.00138
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.8003
    std: 0.0028
    paper_value: 0.8003
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
    source_ref: ma_graph_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.80026
    at_pub_std: 0.00277
    at_pub_source_arxiv: '2310.20519'
    at_pub_source_title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    at_pub_source_date_iso: '2023-10-31'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 4.0000000000040004e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8003
    true_std: 0.0028
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8003
    sort_std: 0.0028
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.7923
    std: 0.0035
    paper_value: 0.7923
    paper_std: 0.0035
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
    source_ref: hussain_global_2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.79232
    at_pub_std: 0.00348
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 2.0000000000020002e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.79232
    true_std: 0.00348
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.79232
    sort_std: 0.00348
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S² GatedGCN
    model_key: s² gatedgcn
    model_plain: S² GatedGCN
    value: 0.7808
    std: 0.0005
    paper_value: 0.7808
    paper_std: 0.0005
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7808
    true_std: 0.0005
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0005
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
  - model: GPTrans-Nano
    model_key: gptrans-nano
    model_plain: GPTrans-Nano
    value: 0.7807
    std: 0.0015
    paper_value: 0.7807
    paper_std: 0.0015
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
    source_ref: chen_graph_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.78069
    at_pub_std: 0.00154
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 9.99999999995449e-06
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7807
    true_std: 0.0015
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7807
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.7807
    std: 0.0004
    paper_value: 0.7807
    paper_std: 0.0004
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
    source_ref: shirzad_exphormer_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7807
    true_std: 0.0004
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7807
    sort_std: 0.0004
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.7803
    std: 0.0022
    paper_value: 0.7803
    paper_std: 0.0022
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
    source_ref: choi_topology-informed_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7803
    true_std: 0.0022
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7803
    sort_std: 0.0022
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.7802
    std: 0.0018
    paper_value: 0.7802
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: rampasek_recipe_2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.78016
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 4.0000000000040004e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7802
    true_std: 0.0018
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7802
    sort_std: 0.0018
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARGNP
    model_key: argnp
    model_plain: ARGNP
    value: 0.7735
    std: 0.0005
    paper_value: 0.7735
    paper_std: 0.0005
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
    source_ref: cai_automatic_2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7735
    true_std: 0.0005
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7735
    sort_std: 0.0005
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7608
    std: 0.002
    paper_value: 0.7608
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the CLUSTER task using fixed public splits as per Dwivedi
      et al. 2023.
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.76082
    at_pub_std: 0.00196
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 2.0000000000020002e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.76082
    true_std: 0.00196
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.76082
    sort_std: 0.00196
    global_rank: 55
    paper_rank: 56
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
- &id003
  dataset: Peptides-func
  rows:
  - model: S^2GCN
    model_key: s^2gcn
    model_plain: S^2GCN
    value: 0.7275
    std: 0.0066
    paper_value: 0.7275
    paper_std: 0.0066
    metric: AP
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7311
    true_std: 0.0066
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0035999999999999366
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: 0.0066
    global_rank: 1
    paper_rank: 4
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S^2 GCN + PE
    model_key: s^2 gcn + pe
    model_plain: S^2 GCN + PE
    value: 0.7311
    std: 0.0066
    paper_value: 0.7311
    paper_std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: PE is described as stable positional encodings almost
      free of cost for S2GNNs.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7311
    true_std: 0.0066
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: 0.0066
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: s4g
    model_plain: Tango_GPS
    value: 0.7293
    std: 0.0004
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7293
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.686
    std: 0.005
    paper_value: 0.686
    paper_std: 0.005
    metric: AP
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
    source_ref: tonshoff_where_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.686
    at_pub_std: 0.005
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
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
    true_value: 0.7261
    true_std: 0.0011
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.040099999999999913
    has_value_note: false
    value_note: ''
    sort_value: 0.7261
    sort_std: 0.0011
    global_rank: 5
    paper_rank: 62
    rank_delta: 57
    rank_delta_abs: 57
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS+HDSE
    model_key: gps+hdse
    model_plain: GPS+HDSE
    value: 0.7156
    std: 0.0058
    paper_value: 0.7156
    paper_std: 0.0058
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: luo_enhancing_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7156
    true_std: 0.0058
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7156
    sort_std: 0.0058
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
  - model: DRew-GCN
    model_key: drew-gcn
    model_plain: DRew-GCN
    value: 0.715
    std: 0.0044
    paper_value: 0.715
    paper_std: 0.0044
    metric: AP
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
    source_ref: gutteridge_drew_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.0044
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.0044
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
  - model: Graph Mamba
    model_key: graph mamba
    model_plain: Graph Mamba
    value: 0.7071
    std: 0.0083
    paper_value: 0.7071
    paper_std: 0.0083
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: behrouz_graph_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7071
    true_std: 0.0083
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7071
    sort_std: 0.0083
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
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.6988
    std: 0.0082
    paper_value: 0.6988
    paper_std: 0.0082
    metric: AP
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
    source_ref: ma_graph_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6988
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6988
    true_std: 0.0082
    value_gap_source_arxiv: '2408.07654'
    value_gap_source_title: 'Graph Triple Attention Network: A Decoupled Perspective'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6988
    sort_std: 0.0082
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph ViT
    model_key: graph vit
    model_plain: Graph ViT
    value: 0.6942
    std: 0.0075
    paper_value: 0.6942
    paper_std: 0.0075
    metric: AP
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
    source_ref: he_generalization_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6942
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2212.13350'
    at_pub_source_title: A Generalization of ViT/MLP-Mixer to Graphs
    at_pub_source_date_iso: '2022-12-27'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6942
    true_std: 0.0075
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6942
    sort_std: 0.0075
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G.MLPMixer
    model_key: g.mlpmixer
    model_plain: G.MLPMixer
    value: 0.6921
    std: 0.0054
    paper_value: 0.6921
    paper_std: 0.0054
    metric: AP
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
    source_ref: he_generalization_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6921
    true_std: 0.0054
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6921
    sort_std: 0.0054
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
  - model: MGT + RWPE
    model_key: mgt + rwpe
    model_plain: MGT + RWPE
    value: 0.6817
    std: 0.0064
    paper_value: 0.6817
    paper_std: 0.0064
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ngo_multiresolution_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6709
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2302.08647'
    at_pub_source_title: Multiresolution Graph Transformers and Wavelet Positional
      Encoding for Learning Hierarchical Structures
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.01079999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6817
    true_std: 0.0064
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6817
    sort_std: 0.0064
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PathNN
    model_key: pathnn
    model_plain: PathNN
    value: 0.6816
    std: 0.0026
    paper_value: 0.6816
    paper_std: 0.0026
    metric: AP
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
    source_ref: michel_path_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6816
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6816
    true_std: 0.0026
    value_gap_source_arxiv: '2310.07430'
    value_gap_source_title: Non-backtracking Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6816
    sort_std: 0.0026
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
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.6679
    std: 0.0074
    paper_value: 0.6679
    paper_std: 0.0074
    metric: AP
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
    source_ref: choi_topology-informed_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6679
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2402.02005'
    at_pub_source_title: Topology-Informed Graph Transformer
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6679
    true_std: 0.0074
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6679
    sort_std: 0.0074
    global_rank: 88
    paper_rank: 88
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
    value: 0.6569
    std: 0.0117
    paper_value: 0.6569
    paper_std: 0.0117
    metric: AP
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
    source_ref: giusti_cin_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 'Task: graph classification; Split: standard (rampasek_recipe_2022);
      Metric: AP'
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6569
    at_pub_std: 0.0117
    at_pub_source_arxiv: '2306.03561'
    at_pub_source_title: 'CIN++: Enhancing Topological Message Passing'
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6569
    true_std: 0.0117
    value_gap_source_arxiv: '2310.07430'
    value_gap_source_title: Non-backtracking Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6569
    sort_std: 0.0117
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AP
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: AP
  paper_metrics:
  - AP
  metric: AP
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Peptides-struct
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.246
    std: 0.0007
    paper_value: 0.246
    paper_std: 0.0007
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
    table_ref: Table 1
    source_ref: tonshoff_where_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.246
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
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
    true_value: 0.2421
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.003899999999999987
    has_value_note: false
    value_note: ''
    sort_value: 0.2421
    sort_std: 0.0016
    global_rank: 1
    paper_rank: 30
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GMN
    model_key: tango_gps
    model_plain: GMN
    value: 0.2422
    std: 0.0014
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Tango does not use additional encodings.
    is_global_top: true
    global_rank: 2
    sort_value: 0.2422
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GMN
    model_key: nba-gin+lappe
    model_plain: GMN
    value: 0.2424
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_display: Oct 2023
    date_iso: '2023-10-11'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/seonghyun26/nba-gnn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2424
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S^2GCN
    model_key: s^2gcn
    model_plain: S^2GCN
    value: 0.2467
    std: 0.0019
    paper_value: 0.2467
    paper_std: 0.0019
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.2447
    true_std: 0.0032
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.2447
    sort_std: 0.0032
    global_rank: 15
    paper_rank: 42
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S^2 GCN + PE
    model_key: s^2 gcn + pe
    model_plain: S^2 GCN + PE
    value: 0.2447
    std: 0.0032
    paper_value: 0.2447
    paper_std: 0.0032
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: PE (Positional Encoding) is typically computed on the
      graph structure.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2447
    true_std: 0.0032
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2447
    sort_std: 0.0032
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graph ViT
    model_key: graph vit
    model_plain: Graph ViT
    value: 0.2449
    std: 0.0016
    paper_value: 0.2449
    paper_std: 0.0016
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
    table_ref: Table 1
    source_ref: he_generalization_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.2449
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2405.17311'
    at_pub_source_title: Probabilistic Graph Rewiring via Virtual Nodes
    at_pub_source_date_iso: '2024-05-27'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2449
    true_std: 0.0016
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2449
    sort_std: 0.0016
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MGT + RWPE
    model_key: mgt + rwpe
    model_plain: MGT + RWPE
    value: 0.2453
    std: 0.0025
    paper_value: 0.2453
    paper_std: 0.0025
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
    table_ref: Table 1
    source_ref: ngo_multiresolution_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.2496
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2302.08647'
    at_pub_source_title: Multiresolution Graph Transformers and Wavelet Positional
      Encoding for Learning Hierarchical Structures
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.004299999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2453
    true_std: 0.0025
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2453
    sort_std: 0.0025
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multiresolution Graph Transformers and Wavelet Positional
      Encoding for Learning Hierarchical Structures
    comparison_source_arxiv: '2302.08647'
    is_best: true
    is_std_outlier: false
  - model: GPS+HDSE
    model_key: gps+hdse
    model_plain: GPS+HDSE
    value: 0.2457
    std: 0.0013
    paper_value: 0.2457
    paper_std: 0.0013
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
    table_ref: Table 1
    source_ref: luo_enhancing_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2457
    true_std: 0.0013
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2457
    sort_std: 0.0013
    global_rank: 27
    paper_rank: 27
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
    table_ref: Table 1
    source_ref: ma_graph_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.246
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2408.07654'
    value_gap_source_title: 'Graph Triple Attention Network: A Decoupled Perspective'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.246
    sort_std: 0.0012
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
  - model: Graph Mamba
    model_key: graph mamba
    model_plain: Graph Mamba
    value: 0.2473
    std: 0.0025
    paper_value: 0.2473
    paper_std: 0.0025
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
    table_ref: Table 1
    source_ref: behrouz_graph_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2473
    true_std: 0.0025
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2473
    sort_std: 0.0025
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G.MLPMixer
    model_key: g.mlpmixer
    model_plain: G.MLPMixer
    value: 0.2475
    std: 0.0015
    paper_value: 0.2475
    paper_std: 0.0015
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
    table_ref: Table 1
    source_ref: he_generalization_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2475
    true_std: 0.0015
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2475
    sort_std: 0.0015
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
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.2485
    std: 0.0015
    paper_value: 0.2485
    paper_std: 0.0015
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
    table_ref: Table 1
    source_ref: choi_topology-informed_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.2485
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2402.02005'
    at_pub_source_title: Topology-Informed Graph Transformer
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2485
    true_std: 0.0015
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2485
    sort_std: 0.0015
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
    table_ref: Table 1
    source_ref: giusti_cin_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.2523
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2306.03561'
    at_pub_source_title: 'CIN++: Enhancing Topological Message Passing'
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: TMLR 2023
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
    value_gap_source_arxiv: '2310.07430'
    value_gap_source_title: Non-backtracking Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2523
    sort_std: 0.0013
    global_rank: 103
    paper_rank: 103
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew-GCN
    model_key: drew-gcn
    model_plain: DRew-GCN
    value: 0.2536
    std: 0.0015
    paper_value: 0.2536
    paper_std: 0.0015
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
    table_ref: Table 1
    source_ref: gutteridge_drew_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2536
    true_std: 0.0015
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2536
    sort_std: 0.0015
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
  - model: PathNN
    model_key: pathnn
    model_plain: PathNN
    value: 0.2545
    std: 0.0032
    paper_value: 0.2545
    paper_std: 0.0032
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
    table_ref: Table 1
    source_ref: michel_path_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on the standard peptides-struct test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.254
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-12-03'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.0005000000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.254
    true_std: 0.0046
    value_gap_source_arxiv: '2312.01538'
    value_gap_source_title: Recurrent Distance Filtering for Graph Representation
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0005000000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.254
    sort_std: 0.0046
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- &id005
  dataset: arxiv-year
  rows:
  - model: DirGCN
    model_key: largescalenet
    model_plain: DirGCN
    value: 0.6582
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_display: Nov 2024
    date_iso: '2024-11-28'
    venue: null
    codebase_url: https://github.com/Qin87/ScaleNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6582
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S² DirGCN
    model_key: s² dirgcn
    model_plain: S² DirGCN
    value: 0.6495
    std: 0.0033
    paper_value: 0.6495
    paper_std: 0.0033
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on arxiv-year test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6495
    true_std: 0.0033
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6495
    sort_std: 0.0033
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
  - model: FaberNet
    model_key: fabernet
    model_plain: FaberNet
    value: 0.6462
    std: 0.0101
    paper_value: 0.6462
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
    source_ref: koke_holonets_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on arxiv-year test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.6462
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2310.02232'
    at_pub_source_title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    at_pub_source_date_iso: '2023-10-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6462
    true_std: 0.0101
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6462
    sort_std: 0.0101
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DirGCN
    model_key: dirgcn
    model_plain: DirGCN
    value: 0.6444
    std: 0.0027
    paper_value: 0.6444
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on arxiv-year test split
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6444
    true_std: 0.0027
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6444
    sort_std: 0.0027
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
  dataset: ogbn-products
  rows:
  - model: LargeGT-full
    model_key: advsyngnn
    model_plain: LargeGT-full
    value: 0.8931
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8931
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: gofa-f
    model_plain: LargeGT-full
    value: 0.8834
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
    arxiv_id: '2407.09709'
    title: 'GOFA: A Generative One-For-All Model for Joint Graph Language Modeling'
    date: Jul 12, 2024
    date_display: Jul 2024
    date_iso: '2024-07-12'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/JiaruiFeng/GOFA
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8834
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: llms
    model_plain: LargeGT-full
    value: 0.882
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2412.16441'
    title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
      Task-Trees'
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Zehong-Wang/GIT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.882
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.798
    std: 0.003
    paper_value: 0.798
    paper_std: 0.003
    metric: Accuracy
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
    protocol_note: Test split accuracy for ogbn-products node classification
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.801
    at_pub_std: 0.006
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8722
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.07419999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8722
    sort_std: 0.0005
    global_rank: 9
    paper_rank: 154
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S^2GAT
    model_key: s^2gat
    model_plain: S^2GAT
    value: 0.811
    std: 0.007
    paper_value: 0.811
    paper_std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split accuracy for ogbn-products node classification
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.007
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.007
    global_rank: 121
    paper_rank: 121
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
- benchmark: OGB
  datasets:
  - *id001
- benchmark: LRGB
  datasets:
  - *id002
  - *id003
- benchmark: GNNBenchmark
  datasets:
  - *id004
- benchmark: LINKX Benchmarks
  datasets:
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CLUSTER
      dataset_slug: cluster
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: arxiv-year
      dataset_slug: arxiv-year
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: Peptides-struct
      dataset_slug: peptides-struct
    - dataset: Peptides-func
      dataset_slug: peptides-func
main_figure: /figures/2405.19121/main_figure.jpegoptim.jpg
---

