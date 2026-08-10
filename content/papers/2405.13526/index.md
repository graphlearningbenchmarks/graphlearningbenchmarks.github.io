---
title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
arxiv_id: '2405.13526'
source_url: ''
authors:
- name: Joshua Southern
  orcid: null
  s2_author_id: '69470236'
  s2_url: null
- name: Francesco Di Giovanni
  orcid: null
  s2_author_id: '94290272'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2256977580'
  s2_url: null
- name: J. Lutzeyer
  orcid: null
  s2_author_id: '89948093'
  s2_url: null
published_date: May 22, 2024
published_date_iso: '2024-05-22'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: While message passing neural networks (MPNNs) have convincing success in
  a range of applications, they exhibit limitations such as the oversquashing problem
  and their inability to capture long-range interactions. Augmenting MPNNs with a
  virtual node (VN) removes the locality constraint of the layer aggregation and has
  been found to improve performance on a range of benchmarks. We provide a comprehensive
  theoretical analysis of the role of VNs and benefits thereof, through the lenses
  of oversquashing and sensitivity analysis. First, we characterize, precisely, how
  the improvement afforded by VNs on the mixing abilities of the network and hence
  in mitigating oversquashing, depends on the underlying topology. We then highlight
  that, unlike Graph-Transformers (GTs), classical instantiations of the VN are often
  constrained to assign uniform importance to different nodes. Consequently, we propose
  a variant of VN with the same computational complexity, which can have different
  sensitivity to nodes based on the graph structure. We show that this is an extremely
  effective and computationally efficient baseline for graph-level tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    value: 0.2429
    std: 0.0019
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 4
    sort_value: 0.2429
    sort_std: 0.0019
    comparison_type: global_top
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
  - model: GatedGCN+PE+VN_G
    model_key: gatedgcn+pe+vn_g
    model_plain: GatedGCN+PE+VN_G
    value: 0.2458
    std: 0.0006
    paper_value: 0.2458
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-27'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2458
    true_std: 0.0006
    value_gap_source_arxiv: '2405.17311'
    value_gap_source_title: Probabilistic Graph Rewiring via Virtual Nodes
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2458
    sort_std: 0.0006
    global_rank: 33
    paper_rank: 33
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
  - model: GatedGCN+PE-ViT
    model_key: gatedgcn+pe-vit
    model_plain: GatedGCN+PE-ViT
    value: 0.2465
    std: 0.0015
    paper_value: 0.2465
    paper_std: 0.0015
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2465
    true_std: 0.0015
    value_gap_source_arxiv: '2405.13526'
    value_gap_source_title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2465
    sort_std: 0.0015
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
  - model: GINE
    model_key: gine
    model_plain: GINE
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.2473
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.10740000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2473
    true_std: 0.0017
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.10740000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2473
    sort_std: 0.0017
    global_rank: 54
    paper_rank: 193
    rank_delta: 139
    rank_delta_abs: 139
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: false
    is_std_outlier: false
  - model: GatedGCN+PE
    model_key: gatedgcn+pe
    model_plain: GatedGCN+PE
    value: 0.2477
    std: 0.0009
    paper_value: 0.2477
    paper_std: 0.0009
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
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2477
    true_std: 0.0009
    value_gap_source_arxiv: '2405.13526'
    value_gap_source_title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2477
    sort_std: 0.0009
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.2481
    std: 0.0007
    paper_value: 0.2481
    paper_std: 0.0007
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.2481
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2481
    true_std: 0.0007
    value_gap_source_arxiv: '2510.12111'
    value_gap_source_title: 'Chimera: State Space Models Beyond Sequences'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2481
    sort_std: 0.0007
    global_rank: 74
    paper_rank: 74
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
    value: 0.2509
    std: 0.0014
    paper_value: 0.2509
    paper_std: 0.0014
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.25
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-06'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.25
    true_std: 0.0005
    value_gap_source_arxiv: '2605.04834'
    value_gap_source_title: Bridging Input Feature Spaces Towards Graph Foundation
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.25
    sort_std: 0.0005
    global_rank: 92
    paper_rank: 103
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CRaWl
    model_key: crawl
    model_plain: CRaWl
    value: 0.2506
    std: 0.0022
    paper_value: 0.2506
    paper_std: 0.0022
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.2506
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-01-29'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2506
    true_std: 0.0022
    value_gap_source_arxiv: '2501.17901'
    value_gap_source_title: Molecular fingerprints are strong models for peptide function
      prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2506
    sort_std: 0.0022
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN+PE-Mixer
    model_key: gatedgcn+pe-mixer
    model_plain: GatedGCN+PE-Mixer
    value: 0.2508
    std: 0.0007
    paper_value: 0.2508
    paper_std: 0.0007
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2508
    true_std: 0.0007
    value_gap_source_arxiv: '2405.13526'
    value_gap_source_title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2508
    sort_std: 0.0007
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew
    model_key: drew
    model_plain: DRew
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.2781
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-07-01'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.024500000000000022
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2536
    true_std: 0.0015
    value_gap_source_arxiv: '2507.00647'
    value_gap_source_title: Cooperative Sheaf Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2536
    sort_std: 0.0015
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Recurrent Distance Filtering for Graph Representation
      Learning
    comparison_source_arxiv: '2312.01538'
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-struct (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
main_figure: /figures/2405.13526/main_figure.jpegoptim.jpg
---

