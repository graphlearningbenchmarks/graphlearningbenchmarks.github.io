---
title: Learning Long Range Dependencies on Graphs via Random Walks
arxiv_id: '2406.03386'
source_url: ''
authors:
- name: Dexiong Chen
  orcid: null
  s2_author_id: '81299639'
  s2_url: null
- name: Till Hendrik Schulz
  orcid: null
  s2_author_id: '2304749126'
  s2_url: null
- name: Karsten M. Borgwardt
  orcid: null
  s2_author_id: '2268189981'
  s2_url: null
published_date: Jun 5, 2024
published_date_iso: '2024-06-05'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Message-passing graph neural networks (GNNs) excel at capturing local relationships
  but struggle with long-range dependencies in graphs. In contrast, graph transformers
  (GTs) enable global information exchange but often oversimplify the graph structure
  by representing graphs as sets of fixed-length vectors. This work introduces a novel
  architecture that overcomes the shortcomings of both approaches by combining the
  long-range information of random walks with local message passing. By treating random
  walks as sequences, our architecture leverages recent advances in sequence models
  to effectively capture long-range dependencies within these walks. Based on this
  concept, we propose a framework that offers (1) more expressive graph representations
  through random walk sequences, (2) the ability to utilize any sequence model for
  capturing long-range dependencies, and (3) the flexibility by integrating various
  GNN and GT architectures. Our experimental evaluations demonstrate that our approach
  achieves significant performance improvements on 19 graph and node benchmark datasets,
  notably outperforming existing methods by up to 13\ Code:.
codebase_url: https://github.com/BorgwardtLab/NeuralWalker
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NeuralWalker
mrr: 0.25
adjusted_mrr: 0.0833
mrr_dataset_count: 1
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
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
  - model: NeuralWalker
    model_key: neuralwalker
    model_plain: NeuralWalker
    value: 0.4707
    std: 0.0007
    paper_value: 0.4707
    paper_std: 0.0007
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4707
    true_std: 0.0007
    value_gap_source_arxiv: '2406.03386'
    value_gap_source_title: Learning Long Range Dependencies on Graphs via Random
      Walks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4707
    sort_std: 0.0007
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.4703
    std: 0.0014
    paper_value: 0.4703
    paper_std: 0.0014
    metric: MRR
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
    source_ref: tonshoff2023did
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.3498
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2401.01233'
    at_pub_source_title: 'GEN: A Practical Alternative to Graph Transformers for Long-Range
      Graph Modeling'
    at_pub_source_date_iso: '2024-01-02'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1205
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4703
    true_std: 0.0014
    value_gap_source_arxiv: '2406.03386'
    value_gap_source_title: Learning Long Range Dependencies on Graphs via Random
      Walks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4703
    sort_std: 0.0014
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GEN: A Practical Alternative to Graph Transformers for
      Long-Range Graph Modeling'
    comparison_source_arxiv: '2401.01233'
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.467
    std: 0.0004
    paper_value: 0.467
    paper_std: 0.0004
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
    source_ref: bresson2017residual; tonshoff2023did
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.3495
    at_pub_std: 0.001
    at_pub_source_arxiv: '2401.01233'
    at_pub_source_title: 'GEN: A Practical Alternative to Graph Transformers for Long-Range
      Graph Modeling'
    at_pub_source_date_iso: '2024-01-02'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.11750000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.467
    true_std: 0.0004
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.467
    sort_std: 0.0004
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GEN: A Practical Alternative to Graph Transformers for
      Long-Range Graph Modeling'
    comparison_source_arxiv: '2401.01233'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.4617
    std: 0.0005
    paper_value: 0.4617
    paper_std: 0.0005
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
    source_ref: xu2019powerful; tonshoff2023did
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-05'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4617
    true_std: 0.0005
    value_gap_source_arxiv: '2406.03386'
    value_gap_source_title: Learning Long Range Dependencies on Graphs via Random
      Walks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4617
    sort_std: 0.0005
    global_rank: 16
    paper_rank: 16
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
    value: 0.4526
    std: 0.0006
    paper_value: 0.4526
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
    source_ref: kipf2016semi; tonshoff2023did
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 5, 2024
    date_display: Jun 2024
    date_iso: '2024-06-05'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.3424
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2401.01233'
    at_pub_source_title: 'GEN: A Practical Alternative to Graph Transformers for Long-Range
      Graph Modeling'
    at_pub_source_date_iso: '2024-01-02'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.11020000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4526
    true_std: 0.0006
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4526
    sort_std: 0.0006
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GEN: A Practical Alternative to Graph Transformers for
      Long-Range Graph Modeling'
    comparison_source_arxiv: '2401.01233'
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
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PCQM-Contact
      dataset_slug: pcqm-contact
single_proposed_model: NeuralWalker
main_figure: /figures/2406.03386/main_figure.jpegoptim.jpg
---

