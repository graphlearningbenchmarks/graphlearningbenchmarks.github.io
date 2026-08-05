---
title: Hypergraph Neural Network with State Space Models for Node Classification
arxiv_id: '2508.06587'
source_url: ''
authors:
- name: A. Quadir
  orcid: null
  s2_author_id: null
  s2_url: null
- name: M. Tanveer
  orcid: null
  s2_author_id: null
  s2_url: null
published_date: Aug 8, 2025
published_date_iso: '2025-08-08'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: In recent years, graph neural networks (GNNs) have gained significant attention
  for node classification tasks on graph-structured data. However, traditional GNNs
  primarily focus on adjacency relationships between nodes, often overlooking the
  role-based characteristics that can provide complementary insights for learning
  expressive node representations. Existing frameworks for extracting role-based features
  are largely unsupervised and often fail to translate effectively into downstream
  predictive tasks. To address these limitations, we propose a hypergraph neural network
  with a state space model (HGMN). The model integrates role-aware representations
  into GNNs by combining hypergraph construction with state-space modeling in a principled
  manner. HGMN employs hypergraph construction techniques to capture higher-order
  relationships and leverages a learnable mamba transformer mechanism to fuse role-based
  and adjacency-based embeddings. By exploring two distinct hypergraph construction
  strategies, degree-based and neighborhood-based, the framework reinforces connectivity
  among nodes with structural similarity, thereby enriching the learned representations.
  Furthermore, the inclusion of hypergraph convolution layers enables the model to
  account for complex dependencies within hypergraph structures. To alleviate the
  over-smoothing problem encountered in deeper networks, we incorporate residual connections,
  which improve stability and promote effective feature propagation across layers.
  Comprehensive experiments on benchmark datasets including OGB, ACM, DBLP, IIP TerroristRel,
  Cora, Citeseer, and Pubmed demonstrate that HGMN consistently outperforms strong
  baselines in node classification tasks. These results support the claim that explicitly
  incorporating role-based features within a hypergraph framework offers tangible
  benefits for node classification tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HGMN (L)
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
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ogbn-products
  rows:
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.7955
    std: 0.014
    paper_value: 0.7955
    paper_std: 0.014
    metric: Micro-F1
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
    source_ref: rampavsek2022recipe
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard OGB node classification task using Micro-F1 metric.
    date: Aug 8, 2025
    date_display: Aug 2025
    date_iso: '2025-08-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7955
    true_std: 0.014
    value_gap_source_arxiv: '2508.06587'
    value_gap_source_title: Hypergraph Neural Network with State Space Models for
      Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7955
    sort_std: 0.014
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
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.7933
    std: 0.015
    paper_value: 0.7933
    paper_std: 0.015
    metric: Micro-F1
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
    source_ref: ying2021transformers
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard OGB node classification task using Micro-F1 metric.
    date: Aug 8, 2025
    date_display: Aug 2025
    date_iso: '2025-08-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7933
    true_std: 0.015
    value_gap_source_arxiv: '2508.06587'
    value_gap_source_title: Hypergraph Neural Network with State Space Models for
      Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.015
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
  - model: GROVER
    model_key: grover
    model_plain: GROVER
    value: 0.7895
    std: 0.017
    paper_value: 0.7895
    paper_std: 0.017
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
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
    source_ref: rong2020self
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard OGB node classification task using Micro-F1 metric.
    date: Aug 8, 2025
    date_display: Aug 2025
    date_iso: '2025-08-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7895
    true_std: 0.017
    value_gap_source_arxiv: '2508.06587'
    value_gap_source_title: Hypergraph Neural Network with State Space Models for
      Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7895
    sort_std: 0.017
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
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.7802
    std: 0.016
    paper_value: 0.7802
    paper_std: 0.016
    metric: Micro-F1
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
    source_ref: kreuzer2021rethinking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard OGB node classification task using Micro-F1 metric.
    date: Aug 8, 2025
    date_display: Aug 2025
    date_iso: '2025-08-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7802
    true_std: 0.016
    value_gap_source_arxiv: '2508.06587'
    value_gap_source_title: Hypergraph Neural Network with State Space Models for
      Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7802
    sort_std: 0.016
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.7748
    std: 0.018
    paper_value: 0.7748
    paper_std: 0.018
    metric: Micro-F1
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
    source_ref: hou2022graphmae
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard OGB node classification task using Micro-F1 metric.
    date: Aug 8, 2025
    date_display: Aug 2025
    date_iso: '2025-08-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7748
    true_std: 0.018
    value_gap_source_arxiv: '2508.06587'
    value_gap_source_title: Hypergraph Neural Network with State Space Models for
      Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7748
    sort_std: 0.018
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
single_proposed_model: HGMN (L)
main_figure: /figures/2508.06587/main_figure.jpegoptim.jpg
---

