---
title: Disentangled and Self-Explainable Node Representation Learning
arxiv_id: '2410.21043'
source_url: ''
authors:
- name: Simone Piaggesi
  orcid: null
  s2_author_id: '148115261'
  s2_url: null
- name: A. Panisson
  orcid: null
  s2_author_id: '2735649'
  s2_url: null
- name: Megha Khosla
  orcid: null
  s2_author_id: '2125218238'
  s2_url: null
published_date: Oct 28, 2024
published_date_iso: '2024-10-28'
published_venue: TMLR 2024
published_conference: TMLR 2024
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Node embeddings are low-dimensional vectors that capture node properties,
  typically learned through unsupervised structural similarity objectives or supervised
  tasks. While recent efforts have focused on post-hoc explanations for graph models,
  intrinsic interpretability in unsupervised node embeddings remains largely underexplored.
  To bridge this gap, we introduce DiSeNE (Disentangled and Self-Explainable Node
  Embedding), a framework that learns self-explainable node representations in an
  unsupervised fashion. By leveraging disentangled representation learning, DiSeNE
  ensures that each embedding dimension corresponds to a distinct topological substructure
  of the graph, thus offering clear, dimension-wise interpretability. We introduce
  new objective functions grounded in principled desiderata, jointly optimizing for
  structural fidelity, disentanglement, and human interpretability. Additionally,
  we propose several new metrics to evaluate representation quality and human interpretability.
  Extensive experiments on multiple benchmark datasets demonstrate that DiSeNE not
  only preserves the underlying graph structure but also provides transparent, human-understandable
  explanations for each embedding dimension.
codebase_url: https://github.com/simonepiaggesi/disene
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DiSe-GAE
- DiSe-FCAE
mrr: 0.0115
adjusted_mrr: 0.0038
mrr_dataset_count: 1
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
  dataset: PPI
  is_multi_metric: true
  rows:
  - model: GAMLP(JK)
    model_key: gamlp(jk)
    model_plain: GAMLP(JK)
    metric_values:
    - 0.9982
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    published_venue: ''
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9982
    sort_std: 0.01
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphCON-GCN
    model_key: graphcon-gcn
    model_plain: GraphCON-GCN
    metric_values:
    - 0.996
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    published_venue: ''
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.996
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    metric_values:
    - 0.9956
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02133'
    title: Simple and Deep Graph Convolutional Networks
    published_venue: ''
    date: Jul 4, 2020
    date_display: Jul 2020
    date_iso: '2020-07-04'
    codebase_url: https://github.com/DropEdge/DropEdge
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.9956
    sort_std: 0.02
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.985
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    published_venue: ''
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    is_global_top: true
    global_rank: 21
    is_best: false
    sort_value: 0.985
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.097
    - 0.306
    - null
    metric_stds:
    - 0.04
    - 0.005
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.958
    sort_std: 0.001
    true_value: 0.958
    true_std: 0.001
    paper_value: 0.097
    paper_std: 0.04
    has_value_gap: true
    has_value_note: false
    value_gap: 0.861
    value_gap_source_arxiv: '2201.13410'
    value_gap_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    value_note: ''
    at_pub_value: 0.958
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.13410'
    at_pub_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    at_pub_source_date_iso: '2022-01-31'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-01-31'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.861
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    comparison_source_arxiv: '2201.13410'
    is_best: false
    is_std_outlier: false
    global_rank: 78
  - model: DiSe-GAE
    model_key: dise-gae
    model_plain: DiSe-GAE
    metric_values:
    - 0.937
    - 0.515
    - 0.937
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.937
    sort_std: 0.001
    true_value: 0.937
    true_std: 0.001
    paper_value: 0.937
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 87
  - model: DiSe-FCAE
    model_key: dise-fcae
    model_plain: DiSe-FCAE
    metric_values:
    - 0.934
    - 0.484
    - 0.934
    metric_stds:
    - 0.003
    - 0.001
    - 0.003
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.934
    sort_std: 0.003
    true_value: 0.934
    true_std: 0.003
    paper_value: 0.934
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 88
  - model: DW+Dine
    model_key: dw+dine
    model_plain: DW+Dine
    metric_values:
    - 0.855
    - 0.569
    - null
    metric_stds:
    - 0.016
    - 0.022
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.855
    sort_std: 0.016
    true_value: 0.855
    true_std: 0.016
    paper_value: 0.855
    paper_std: 0.016
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 99
  - model: GAE+Dine
    model_key: gae+dine
    model_plain: GAE+Dine
    metric_values:
    - 0.646
    - 0.484
    - null
    metric_stds:
    - 0.003
    - 0.007
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.646
    sort_std: 0.003
    true_value: 0.646
    true_std: 0.003
    paper_value: 0.646
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 154
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - 0.015
    - 0.281
    - null
    metric_stds:
    - 0.003
    - 0.002
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.529
    sort_std: null
    true_value: 0.529
    true_std: null
    paper_value: 0.015
    paper_std: 0.003
    has_value_gap: true
    has_value_note: false
    value_gap: 0.514
    value_gap_source_arxiv: '2207.11996'
    value_gap_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    value_note: ''
    at_pub_value: 0.529
    at_pub_std: null
    at_pub_source_arxiv: '2009.10273'
    at_pub_source_title: Sub-graph Contrast for Scalable Self-Supervised Graph Representation
      Learning
    at_pub_source_date_iso: '2020-09-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.514
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Sub-graph Contrast for Scalable Self-Supervised Graph
      Representation Learning
    comparison_source_arxiv: '2009.10273'
    is_best: false
    is_std_outlier: false
    global_rank: 174
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.462
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.00494'
    title: Graph Neural Networks Gone Hogwild
    published_venue: ''
    date: Jun 29, 2024
    date_display: Jun 2024
    date_iso: '2024-06-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 183
    is_best: false
    sort_value: 0.462
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphAE
    model_key: graphae
    model_plain: GraphAE
    metric_values:
    - 0.452
    - 0.263
    - null
    metric_stds:
    - 0.008
    - 0.003
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.452
    sort_std: 0.008
    true_value: 0.452
    true_std: 0.008
    paper_value: 0.452
    paper_std: 0.008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 184
  - model: InfWalk
    model_key: infwalk
    model_plain: InfWalk
    metric_values:
    - 0.134
    - 0.312
    - null
    metric_stds:
    - 0.002
    - 0.002
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.134
    sort_std: 0.002
    true_value: 0.134
    true_std: 0.002
    paper_value: 0.134
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 194
  - model: DGLFRM
    model_key: dglfrm
    model_plain: DGLFRM
    metric_values:
    - 0.102
    - 0.515
    - null
    metric_stds:
    - 0.002
    - 0.008
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.102
    sort_std: 0.002
    true_value: 0.102
    true_std: 0.002
    paper_value: 0.102
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2410.21043'
    value_gap_source_title: Disentangled and Self-Explainable Node Representation
      Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-28'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: TMLR 2024
    date: Oct 28, 2024
    date_display: Oct 2024
    date_iso: '2024-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 195
  metrics:
  - F1
  - Topological Alignment
  - Overlap Consistency
  primary_metric: F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  - Topological Alignment
  - Overlap Consistency
  metric: F1
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
    - dataset: PPI
      dataset_slug: ppi
main_figure: /figures/2410.21043/main_figure.jpegoptim.jpg
---

