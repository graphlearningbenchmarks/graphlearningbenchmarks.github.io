---
title: Diffusion Improves Graph Learning
arxiv_id: '1911.05485'
source_url: ''
authors:
- name: Johannes Klicpera
  orcid: null
  s2_author_id: '51516539'
  s2_url: null
- name: Stefan Weißenberger
  orcid: null
  s2_author_id: '8350757'
  s2_url: null
- name: Stephan Günnemann
  orcid: null
  s2_author_id: '3075189'
  s2_url: null
published_date: Oct 28, 2019
published_date_iso: '2019-10-28'
published_venue: NeurIPS 2019
published_conference: NeurIPS 2019
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Graph convolution is the core of most Graph Neural Networks (GNNs) and
  usually approximated by message passing between direct (one-hop) neighbors. In this
  work, we remove the restriction of using only the direct neighbors by introducing
  a powerful, yet spatially localized graph convolution: Graph diffusion convolution
  (GDC). GDC leverages generalized graph diffusion, examples of which are the heat
  kernel and personalized PageRank. It alleviates the problem of noisy and often arbitrarily
  defined edges in real graphs. We show that GDC is closely related to spectral-based
  models and thus combines the strengths of both spatial (message passing) and spectral
  methods. We demonstrate that replacing message passing with graph diffusion convolution
  consistently leads to significant performance improvements across a wide range of
  models on both supervised and unsupervised tasks and a variety of datasets. Furthermore,
  GDC is not limited to GNNs but can trivially be combined with any graph-based model
  or algorithm (e.g. spectral clustering) without requiring any changes to the latter
  or affecting its computational complexity. Our implementation is available online.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  dataset: Amazon-Photo
  rows:
  - model: SGT
    model_key: msh-gnn
    model_plain: SGT
    value: 0.9766
    std: 0.005
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
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGT
    model_key: geomancer
    model_plain: SGT
    value: 0.9705
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
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGT
    model_key: graphtarif
    model_plain: SGT
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
    global_rank: 3
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
    value: 0.9186
    std: 0.002
    paper_value: 0.9186
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.897
    at_pub_std: 0.017
    at_pub_source_arxiv: '1909.03211'
    at_pub_source_title: Measuring and Relieving the Over-smoothing Problem for Graph
      Neural Networks from the Topological View
    at_pub_source_date_iso: '2019-09-07'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.021599999999999953
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04830000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 5
    paper_rank: 332
    rank_delta: 327
    rank_delta_abs: 327
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Measuring and Relieving the Over-smoothing Problem for
      Graph Neural Networks from the Topological View
    comparison_source_arxiv: '1909.03211'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9282
    std: 0.0023
    paper_value: 0.9282
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.906
    at_pub_std: 0.007
    at_pub_source_arxiv: '1909.03211'
    at_pub_source_title: Measuring and Relieving the Over-smoothing Problem for Graph
      Neural Networks from the Topological View
    at_pub_source_date_iso: '2019-09-07'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.022199999999999998
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.03499999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 16
    paper_rank: 228
    rank_delta: 212
    rank_delta_abs: 212
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Measuring and Relieving the Over-smoothing Problem for
      Graph Neural Networks from the Topological View
    comparison_source_arxiv: '1909.03211'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.9142
    std: 0.0026
    paper_value: 0.9142
    paper_std: 0.0026
    metric: Accuracy
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9573
    true_std: 0.0012
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04310000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9573
    sort_std: 0.0012
    global_rank: 25
    paper_rank: 362
    rank_delta: 337
    rank_delta_abs: 337
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
    value: 0.5134
    std: 0.0196
    paper_value: 0.5134
    paper_std: 0.0196
    metric: Accuracy
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
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
    value_gap: 0.4175
    has_value_note: false
    value_note: ''
    sort_value: 0.9309
    sort_std: 0.0008
    global_rank: 206
    paper_rank: 539
    rank_delta: 333
    rank_delta_abs: 333
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JK
    model_key: jk
    model_plain: JK
    value: 0.9293
    std: 0.0021
    paper_value: 0.9293
    paper_std: 0.0021
    metric: Accuracy
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.9293
    sort_std: 0.0021
    global_rank: 218
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8724
    std: 0.0065
    paper_value: 0.8724
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-25'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9211
    true_std: 0.0032
    value_gap_source_arxiv: '2305.15747'
    value_gap_source_title: Union Subgraph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04870000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0032
    global_rank: 314
    paper_rank: 467
    rank_delta: 153
    rank_delta_abs: 153
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
    value: 0.7926
    std: 0.0009
    paper_value: 0.7926
    paper_std: 0.0009
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.1079
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0008
    global_rank: 423
    paper_rank: 498
    rank_delta: 75
    rank_delta_abs: 75
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARMA
    model_key: arma
    model_plain: ARMA
    value: 0.9205
    std: 0.0024
    paper_value: 0.9205
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: 0.864
    at_pub_std: 0.03
    at_pub_source_arxiv: '1909.03211'
    at_pub_source_title: Measuring and Relieving the Over-smoothing Problem for Graph
      Neural Networks from the Topological View
    at_pub_source_date_iso: '2019-09-07'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.056499999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: 0.0495
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.020499999999999963
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.0495
    global_rank: 428
    paper_rank: 323
    rank_delta: -105
    rank_delta_abs: 105
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Measuring and Relieving the Over-smoothing Problem for
      Graph Neural Networks from the Topological View
    comparison_source_arxiv: '1909.03211'
    is_best: false
    is_std_outlier: true
  - model: DCSBM
    model_key: dcsbm
    model_plain: DCSBM
    value: 0.6713
    std: 0.0249
    paper_value: 0.6713
    paper_std: 0.0249
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6713
    sort_std: 0.0249
    global_rank: 522
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: Spectral
    model_key: spectral
    model_plain: Spectral
    value: 0.5365
    std: 0.0322
    paper_value: 0.5365
    paper_std: 0.0322
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
    table_ref: Table tab:hyper:photo
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5365
    sort_std: 0.0322
    global_rank: 537
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
main_figure: /figures/1911.05485/main_figure.jpegoptim.jpg
---

