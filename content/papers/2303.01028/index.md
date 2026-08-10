---
title: 'Specformer: Spectral Graph Neural Networks Meet Transformers'
arxiv_id: '2303.01028'
source_url: ''
authors:
- name: Deyu Bo
  orcid: null
  s2_author_id: '1491450638'
  s2_url: null
- name: Chuan Shi
  orcid: null
  s2_author_id: '2113917199'
  s2_url: null
- name: Lele Wang
  orcid: null
  s2_author_id: '2277570603'
  s2_url: null
- name: Renjie Liao
  orcid: null
  s2_author_id: '2246396'
  s2_url: null
published_date: Mar 2, 2023
published_date_iso: '2023-03-02'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Spectral graph neural networks (GNNs) learn graph representations via spectral-domain
  graph convolutions. However, most existing spectral graph filters are scalar-to-scalar
  functions, i.e., mapping a single eigenvalue to a single filtered value, thus ignoring
  the global pattern of the spectrum. Furthermore, these filters are often constructed
  based on some fixed-order polynomials, which have limited expressiveness and flexibility.
  To tackle these issues, we introduce Specformer, which effectively encodes the set
  of all eigenvalues and performs self-attention in the spectral domain, leading to
  a learnable set-to-set spectral filter. We also design a decoder with learnable
  bases to enable non-local graph convolution. Importantly, Specformer is equivariant
  to permutation. By stacking multiple Specformer layers, one can build a powerful
  spectral GNN. On synthetic datasets, we show that our Specformer can better recover
  ground-truth spectral filters than other spectral GNNs. Extensive experiments of
  both node-level and graph-level tasks on real-world graph datasets show that our
  Specformer outperforms state-of-the-art GNNs and learns meaningful spectrum patterns.
  Code and data are available at.
codebase_url: https://github.com/bdy9527/Specformer
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Specformer
- Specformer-medium
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: PCQM4Mv2
  rows:
  - model: DeMol
    model_key: demol
    model_plain: DeMol
    value: 0.0603
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 186.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted to ICLR 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.0603
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TGT-At
    model_key: tgt-at
    model_plain: TGT-At
    value: 0.0671
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted to ICLR 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.0671
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGT-At (+RDKit)
    model_key: tgt-at (+rdkit)
    model_plain: TGT-At (+RDKit)
    value: 0.0683
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/shamim-hussain/tgt
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.0683
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS-medium
    model_key: gps-medium
    model_plain: GPS-medium
    value: 0.0858
    std: null
    paper_value: 0.0858
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.4
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GPS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-31'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0858
    true_std: null
    value_gap_source_arxiv: '2310.20519'
    value_gap_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0858
    sort_std: null
    global_rank: 22
    paper_rank: 22
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
    value: 0.0869
    std: null
    paper_value: 0.0869
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 89.3
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.0862
    at_pub_std: null
    at_pub_source_arxiv: '2208.05863'
    at_pub_source_title: 'GEM-2: Next Generation Molecular Property Prediction Network
      by Modeling Full-range Many-body Interactions'
    at_pub_source_date_iso: '2022-08-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0007000000000000062
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0862
    true_std: null
    value_gap_source_arxiv: '2402.04538'
    value_gap_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0007000000000000062
    has_value_note: false
    value_note: ''
    sort_value: 0.0862
    sort_std: null
    global_rank: 29
    paper_rank: 33
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GEM-2: Next Generation Molecular Property Prediction
      Network by Modeling Full-range Many-body Interactions'
    comparison_source_arxiv: '2208.05863'
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.0864
    std: null
    paper_value: 0.0864
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.139
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.0864
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0864
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0864
    sort_std: null
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
  - model: GRPE
    model_key: grpe
    model_plain: GRPE
    value: 0.089
    std: null
    paper_value: 0.089
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.089
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0876
    true_std: null
    value_gap_source_arxiv: '2402.04538'
    value_gap_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0013999999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.0876
    sort_std: null
    global_rank: 35
    paper_rank: 38
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer-medium
    model_key: specformer-medium
    model_plain: Specformer-medium
    value: 0.0916
    std: null
    paper_value: 0.0916
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0916
    true_std: null
    value_gap_source_arxiv: '2303.01028'
    value_gap_source_title: 'Specformer: Spectral Graph Neural Networks Meet Transformers'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0916
    sort_std: null
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
  - model: GPS-small
    model_key: gps-small
    model_plain: GPS-small
    value: 0.0938
    std: null
    paper_value: 0.0938
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: GPS
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.0938
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-05-19'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0938
    true_std: null
    value_gap_source_arxiv: '2305.11424'
    value_gap_source_title: IJCAI--23 Formatting Instructions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0938
    sort_std: null
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
  - model: GIN-VN
    model_key: gin-vn
    model_plain: GIN-VN
    value: 0.1083
    std: null
    paper_value: 0.1083
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.7
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.1083
    at_pub_std: null
    at_pub_source_arxiv: '2207.02505'
    at_pub_source_title: Pure Transformers are Powerful Graph Learners
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1083
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1083
    sort_std: null
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
  - model: GCN-VN
    model_key: gcn-vn
    model_plain: GCN-VN
    value: 0.1153
    std: null
    paper_value: 0.1153
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 4.9
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.1152
    at_pub_std: null
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.00010000000000000286
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1152
    true_std: null
    value_gap_source_arxiv: '2402.04538'
    value_gap_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000000286
    has_value_note: false
    value_note: ''
    sort_value: 0.1152
    sort_std: null
    global_rank: 61
    paper_rank: 62
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    comparison_source_arxiv: '2201.12787'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.1379
    std: null
    paper_value: 0.1379
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.1379
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-10-31'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1195
    true_std: null
    value_gap_source_arxiv: '2310.20519'
    value_gap_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.0184
    has_value_note: false
    value_note: ''
    sort_value: 0.1195
    sort_std: null
    global_rank: 67
    paper_rank: 77
    rank_delta: 10
    rank_delta_abs: 10
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
    value: 0.1195
    std: null
    paper_value: 0.1195
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Mar 2, 2023
    date_display: Mar 2023
    date_iso: '2023-03-02'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.1195
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1195
    true_std: null
    value_gap_source_arxiv: '2603.00568'
    value_gap_source_title: Enhancing Molecular Property Predictions by Learning from
      Bond Modelling and Interactions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1195
    sort_std: null
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
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: PCQM4Mv2
      dataset_slug: pcqm4mv2
main_figure: /figures/2303.01028/main_figure.jpegoptim.jpg
---

