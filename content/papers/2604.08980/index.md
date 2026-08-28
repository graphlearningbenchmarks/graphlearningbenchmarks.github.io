---
title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
  Learning'
arxiv_id: '2604.08980'
source_url: ''
authors:
- name: Yi Luo
  orcid: null
  s2_author_id: '2118265204'
  s2_url: null
- name: Xu Sun
  orcid: null
  s2_author_id: '2220471137'
  s2_url: null
- name: Guangchun Luo
  orcid: null
  s2_author_id: '2346917313'
  s2_url: null
- name: Aiguo Chen
  orcid: null
  s2_author_id: '2238440114'
  s2_url: null
published_date: Apr 10, 2026
published_date_iso: '2026-04-10'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) have been widely adopted in engineering applications
  such as social network analysis, chemical research and computer vision. However,
  their efficacy is severely compromised by the inherent homophily assumption, which
  fails to hold for heterophilic graphs where dissimilar nodes are frequently connected.
  To address this fundamental limitation in graph learning, we first draw inspiration
  from the recently discovered monophily property of real-world graphs, and propose
  Neighbourhood Transformers (NT), a novel paradigm that applies self-attention within
  every local neighbourhood instead of aggregating messages to the central node as
  in conventional message-passing GNNs. This design makes NT inherently monophily-aware
  and theoretically guarantees its expressiveness is no weaker than traditional message-passing
  frameworks. For practical engineering deployment, we further develop a neighbourhood
  partitioning strategy equipped with switchable attentions, which reduces the space
  consumption of NT by over 95\ Extensive experiments on 10 real-world datasets (5
  heterophilic and 5 homophilic graphs) show that NT outperforms all current state-of-the-art
  methods on node classification tasks, demonstrating its superior performance and
  cross-domain adaptability. The full implementation code of this work is publicly
  available at to facilitate reproducibility and industrial adoption.
codebase_url: https://github.com/cf020031308/MoNT
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- NT*
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterophily Benchmark
benchmark_coverage:
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 3
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Minesweeper
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9903
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
    global_rank: 1
    sort_value: 0.9903
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9899
    std: 0.0016
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
    global_rank: 2
    sort_value: 0.9899
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.9827
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    sort_value: 0.9827
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NT*
    model_key: nt
    model_plain: NT*
    value: 0.9792
    std: 0.0028
    paper_value: 0.9792
    paper_std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9792
    true_std: 0.0028
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9792
    sort_std: 0.0028
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
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9746
    std: 0.0036
    paper_value: 0.9746
    paper_std: 0.0036
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9749
    true_std: 0.0048
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.9749
    sort_std: 0.0048
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8975
    std: 0.0052
    paper_value: 0.8975
    paper_std: 0.0052
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
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8975
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9744
    true_std: 0.0017
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07690000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0017
    global_rank: 9
    paper_rank: 29
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9709
    std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 11
    sort_value: 0.9709
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Dir-NT
    model_key: dir-nt
    model_plain: Dir-NT
    value: 0.9392
    std: 0.0059
    paper_value: 0.9392
    paper_std: 0.0059
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9392
    true_std: 0.0059
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9392
    sort_std: 0.0059
    global_rank: 17
    paper_rank: 17
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
    value: 0.9063
    std: 0.0067
    paper_value: 0.9063
    paper_std: 0.0067
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9229
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.01660000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9229
    true_std: 0.0061
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.01660000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0061
    global_rank: 20
    paper_rank: 27
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: DIFFormer
    model_key: difformer
    model_plain: DIFFormer
    value: 0.9089
    std: 0.0058
    paper_value: 0.9089
    paper_std: 0.0058
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9089
    true_std: 0.0058
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9089
    sort_std: 0.0058
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9074
    std: 0.0053
    paper_value: 0.9074
    paper_std: 0.0053
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9042
    at_pub_std: 0.001
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0031999999999999806
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9074
    true_std: 0.0053
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9074
    sort_std: 0.0053
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8671
    std: 0.0088
    paper_value: 0.8671
    paper_std: 0.0088
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8771
    true_std: 0.0069
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8771
    sort_std: 0.0069
    global_rank: 33
    paper_rank: 35
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Dir-GNN
    model_key: dir-gnn
    model_plain: Dir-GNN
    value: 0.8705
    std: 0.0069
    paper_value: 0.8705
    paper_std: 0.0069
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
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8705
    true_std: 0.0069
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8705
    sort_std: 0.0069
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.8419
    std: 0.0066
    paper_value: 0.8419
    paper_std: 0.0066
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8419
    true_std: 0.0066
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8419
    sort_std: 0.0066
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
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8109
    std: 0.0102
    paper_value: 0.8109
    paper_std: 0.0102
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8109
    true_std: 0.0102
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8109
    sort_std: 0.0102
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8
    std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    venue: 'Accepted to ICLR 2026. OpenReview: https://openreview.net/forum?id=FmxRzlu0rT'
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 49
    sort_value: 0.8
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: Questions
  rows:
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9733
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    venue: 'Accepted to ICLR 2026. OpenReview: https://openreview.net/forum?id=FmxRzlu0rT'
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9733
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGS-GNN
    model_key: ags-gnn
    model_plain: AGS-GNN
    value: 0.9727
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MeanGNN
    model_key: meangnn
    model_plain: MeanGNN
    value: 0.9716
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
    arxiv_id: '2506.14291'
    title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
    date: Jun 17, 2025
    date_display: Jun 2025
    date_iso: '2025-06-17'
    venue: null
    codebase_url: https://github.com/benfinkelshtein/EquivarianceEverywhere
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9716
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7609
    std: 0.0127
    paper_value: 0.7609
    paper_std: 0.0127
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
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9715
    at_pub_std: null
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.2106
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9715
    true_std: 0.0004
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: false
    value_gap: 0.2106
    has_value_note: false
    value_note: ''
    sort_value: 0.9715
    sort_std: 0.0004
    global_rank: 4
    paper_rank: 34
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.7173
    std: 0.0147
    paper_value: 0.7173
    paper_std: 0.0147
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9349
    true_std: 0.004
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.2175999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9349
    sort_std: 0.004
    global_rank: 23
    paper_rank: 44
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NT*
    model_key: nt
    model_plain: NT*
    value: 0.7936
    std: 0.0069
    paper_value: 0.7936
    paper_std: 0.0069
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7936
    true_std: 0.0069
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7936
    sort_std: 0.0069
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.7892
    std: 0.0089
    paper_value: 0.7892
    paper_std: 0.0089
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7892
    true_std: 0.0089
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7892
    sort_std: 0.0089
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
  - model: Dir-NT
    model_key: dir-nt
    model_plain: Dir-NT
    value: 0.7799
    std: 0.01
    paper_value: 0.7799
    paper_std: 0.01
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7799
    true_std: 0.01
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7799
    sort_std: 0.01
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7644
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.7644
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Dir-GNN
    model_key: dir-gnn
    model_plain: Dir-GNN
    value: 0.7613
    std: 0.0124
    paper_value: 0.7613
    paper_std: 0.0124
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
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7613
    true_std: 0.0124
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7613
    sort_std: 0.0124
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.7576
    std: 0.0166
    paper_value: 0.7576
    paper_std: 0.0166
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7576
    true_std: 0.0166
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7576
    sort_std: 0.0166
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7427
    std: 0.0146
    paper_value: 0.7427
    paper_std: 0.0146
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7427
    true_std: 0.0146
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7427
    sort_std: 0.0146
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.7394
    std: 0.0106
    paper_value: 0.7394
    paper_std: 0.0106
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7394
    true_std: 0.0106
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7394
    sort_std: 0.0106
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIFFormer
    model_key: difformer
    model_plain: DIFFormer
    value: 0.7215
    std: 0.0131
    paper_value: 0.7215
    paper_std: 0.0131
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7215
    true_std: 0.0131
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7215
    sort_std: 0.0131
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
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.6817
    std: 0.0153
    paper_value: 0.6817
    paper_std: 0.0153
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6817
    true_std: 0.0153
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6817
    sort_std: 0.0153
    global_rank: 52
    paper_rank: 52
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: Tolokers
  rows:
  - model: NT*
    model_key: nt
    model_plain: NT*
    value: 0.8591
    std: 0.0083
    paper_value: 0.8591
    paper_std: 0.0083
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8591
    true_std: 0.0083
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8591
    sort_std: 0.0083
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
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.8591
    std: 0.0074
    paper_value: 0.8591
    paper_std: 0.0074
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8591
    true_std: 0.0074
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8591
    sort_std: 0.0074
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
  - model: Dir-NT
    model_key: dir-nt
    model_plain: Dir-NT
    value: 0.8502
    std: 0.0077
    paper_value: 0.8502
    paper_std: 0.0077
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8502
    true_std: 0.0077
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8502
    sort_std: 0.0077
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.8377
    std: 0.0078
    paper_value: 0.8377
    paper_std: 0.0078
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8377
    true_std: 0.0078
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8377
    sort_std: 0.0078
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.8371
    std: 0.0048
    paper_value: 0.8371
    paper_std: 0.0048
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8371
    true_std: 0.0048
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8371
    sort_std: 0.0048
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8364
    std: 0.0067
    paper_value: 0.8364
    paper_std: 0.0067
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
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8364
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2405.20724'
    at_pub_source_title: on Large Graphs using Intersecting Communities
    at_pub_source_date_iso: '2024-05-31'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8364
    true_std: 0.0067
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8364
    sort_std: 0.0067
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
  - model: DIFFormer
    model_key: difformer
    model_plain: DIFFormer
    value: 0.8357
    std: 0.0068
    paper_value: 0.8357
    paper_std: 0.0068
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8357
    true_std: 0.0068
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8357
    sort_std: 0.0068
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
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8311
    std: 0.0104
    paper_value: 0.8311
    paper_std: 0.0104
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8311
    true_std: 0.0104
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8311
    sort_std: 0.0104
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
  - model: Dir-GNN
    model_key: dir-gnn
    model_plain: Dir-GNN
    value: 0.8119
    std: 0.0105
    paper_value: 0.8119
    paper_std: 0.0105
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
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8119
    true_std: 0.0105
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8119
    sort_std: 0.0105
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.7832
    std: 0.0095
    paper_value: 0.7832
    paper_std: 0.0095
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7832
    true_std: 0.0095
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7832
    sort_std: 0.0095
    global_rank: 26
    paper_rank: 26
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
    value: 0.7816
    std: 0.0002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    venue: 'Accepted to ICLR 2026. OpenReview: https://openreview.net/forum?id=FmxRzlu0rT'
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 29
    sort_value: 0.7816
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.781
    std: 0.0103
    paper_value: 0.781
    paper_std: 0.0103
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using default data splits.
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.781
    true_std: 0.0103
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.781
    sort_std: 0.0103
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterophily Benchmark
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Minesweeper
      dataset_slug: minesweeper
    - dataset: Tolokers
      dataset_slug: tolokers
    - dataset: Questions
      dataset_slug: questions
single_proposed_model: NT*
main_figure: /figures/2604.08980/main_figure.jpegoptim.jpg
---

