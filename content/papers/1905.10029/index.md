---
title: Power up! Robust Graph Convolutional Network via Graph Powering
arxiv_id: '1905.10029'
source_url: ''
authors:
- name: Ming Jin
  orcid: null
  s2_author_id: '1455155615'
  s2_url: null
- name: Heng Chang
  orcid: null
  s2_author_id: '144188238'
  s2_url: null
- name: Wenwu Zhu
  orcid: null
  s2_author_id: '145583986'
  s2_url: null
- name: S. Sojoudi
  orcid: null
  s2_author_id: '1685407'
  s2_url: null
published_date: May 24, 2019
published_date_iso: '2019-05-24'
published_venue: AAAI 2019
published_conference: AAAI 2019
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Graph convolutional networks (GCNs) are powerful tools for graph-structured
  data. However, they have been recently shown to be vulnerable to topological attacks.
  To enhance adversarial robustness, we go beyond spectral graph theory to robust
  graph theory. By challenging the classical graph Laplacian, we propose a new convolution
  operator that is provably robust in the spectral domain and is incorporated in the
  GCN architecture to improve expressivity and interpretability. By extending the
  original graph to a sequence of graphs, we also propose a robust training paradigm
  that encourages transferability across graphs that span a range of spatial and spectral
  characteristics. The proposed approaches are demonstrated in extensive experiments
  to simultaneously improve performance in both benign and adversarial situations.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- VPN
mrr: 0.0018
adjusted_mrr: 0.0006
mrr_dataset_count: 1
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9004
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 31
    sort_value: 0.9004
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.828
    std: 0.006
    paper_value: 0.828
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: zhu2019robust
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.828
    at_pub_std: 0.006
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-05-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8801
    true_std: 0.0047
    value_gap_source_arxiv: '2405.18581'
    value_gap_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.052100000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.8801
    sort_std: 0.0047
    global_rank: 126
    paper_rank: 515
    rank_delta: 389
    rank_delta_abs: 389
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.819
    std: 0.004
    paper_value: 0.819
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: abu2019mixhop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8781
    true_std: 0.017
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.05910000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8781
    sort_std: 0.017
    global_rank: 144
    paper_rank: 618
    rank_delta: 474
    rank_delta_abs: 474
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.81
    std: 0.0
    paper_value: 0.81
    paper_std: 0.0
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
    table_ref: Table 1
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.81
    at_pub_std: 0.0
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8683
    true_std: 0.0128
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.05829999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8683
    sort_std: 0.0128
    global_rank: 202
    paper_rank: 694
    rank_delta: 492
    rank_delta_abs: 492
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
    value: 0.672
    std: null
    paper_value: 0.672
    paper_std: null
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
    table_ref: Table 1
    source_ref: perozzi2014deepwalk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.672
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.829
    true_std: null
    value_gap_source_arxiv: '1909.00958'
    value_gap_source_title: 'Graph Representation Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.15699999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: null
    global_rank: 508
    paper_rank: 928
    rank_delta: 420
    rank_delta_abs: 420
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VPN
    model_key: vpn
    model_plain: VPN
    value: 0.823
    std: 0.003
    paper_value: 0.823
    paper_std: 0.003
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.823
    true_std: 0.003
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.823
    sort_std: 0.003
    global_rank: 570
    paper_rank: 570
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: vanilla GCN
    model_key: vanilla gcn
    model_plain: vanilla GCN
    value: 0.815
    std: null
    paper_value: 0.815
    paper_std: null
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-03-17'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.815
    true_std: null
    value_gap_source_arxiv: '2003.07450'
    value_gap_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.815
    sort_std: null
    global_rank: 659
    paper_rank: 659
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGCN(AR)
    model_key: igcn(ar)
    model_plain: IGCN(AR)
    value: 0.811
    std: null
    paper_value: 0.811
    paper_std: null
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
    table_ref: Table 1
    source_ref: li2019label
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: null
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: null
    global_rank: 686
    paper_rank: 686
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PowerLaplacian
    model_key: powerlaplacian
    model_plain: PowerLaplacian
    value: 0.805
    std: null
    paper_value: 0.805
    paper_std: null
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.805
    true_std: null
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: null
    global_rank: 715
    paper_rank: 715
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LNet
    model_key: lnet
    model_plain: LNet
    value: 0.795
    std: 0.018
    paper_value: 0.795
    paper_std: 0.018
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
    table_ref: Table 1
    source_ref: liao2019lanczosnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-08'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.795
    true_std: null
    value_gap_source_arxiv: '2106.04051'
    value_gap_source_title: 'Graph-MLP: Node Classification without Message Passing
      in Graph'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.795
    sort_std: null
    global_rank: 758
    paper_rank: 758
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
    value: 0.7768
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 806
    sort_value: 0.7768
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Planetoid
    model_key: planetoid
    model_plain: Planetoid
    value: 0.757
    std: null
    paper_value: 0.757
    paper_std: null
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
    table_ref: Table 1
    source_ref: yang2016revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.757
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2020-03-17'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.757
    true_std: null
    value_gap_source_arxiv: '2003.07450'
    value_gap_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.757
    sort_std: null
    global_rank: 845
    paper_rank: 845
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ICA
    model_key: ica
    model_plain: ICA
    value: 0.751
    std: null
    paper_value: 0.751
    paper_std: null
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
    table_ref: Table 1
    source_ref: lu2003link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.751
    at_pub_std: null
    at_pub_source_arxiv: '1710.10903'
    at_pub_source_title: Graph Attention Networks
    at_pub_source_date_iso: '2017-10-30'
    at_pub_source_date_label: ICLR 2017
    value_gap_source_date_iso: '2020-01-15'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.751
    true_std: null
    value_gap_source_arxiv: '2001.05140'
    value_gap_source_title: 'Graph-Bert: Only Attention is Needed for Learning Graph
      Representations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: null
    global_rank: 858
    paper_rank: 858
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LP
    model_key: lp
    model_plain: LP
    value: 0.68
    std: null
    paper_value: 0.68
    paper_std: null
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
    table_ref: Table 1
    source_ref: zhu2003semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.68
    at_pub_std: null
    at_pub_source_arxiv: '1603.08861'
    at_pub_source_title: Revisiting Semi-Supervised Learning with Graph Embeddings
    at_pub_source_date_iso: '2016-03-29'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.71
    true_std: 0.0
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.029999999999999916
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: 0.0
    global_rank: 898
    paper_rank: 921
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ManiReg
    model_key: manireg
    model_plain: ManiReg
    value: 0.595
    std: null
    paper_value: 0.595
    paper_std: null
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
    table_ref: Table 1
    source_ref: belkin2006manifold
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.595
    at_pub_std: null
    at_pub_source_arxiv: '1603.08861'
    at_pub_source_title: Revisiting Semi-Supervised Learning with Graph Embeddings
    at_pub_source_date_iso: '2016-03-29'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: JMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.604
    true_std: 0.008
    value_gap_source_arxiv: '2409.09111'
    value_gap_source_title: 'Transformers from Diffusion: A Unified Framework for
      Neural Message Passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.604
    sort_std: 0.008
    global_rank: 959
    paper_rank: 961
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SemiEmb
    model_key: semiemb
    model_plain: SemiEmb
    value: 0.59
    std: null
    paper_value: 0.59
    paper_std: null
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
    table_ref: Table 1
    source_ref: weston2012deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 1000 samples
      for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.59
    at_pub_std: null
    at_pub_source_arxiv: '1603.08861'
    at_pub_source_title: Revisiting Semi-Supervised Learning with Graph Embeddings
    at_pub_source_date_iso: '2016-03-29'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2020-01-15'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.59
    true_std: null
    value_gap_source_arxiv: '2001.05140'
    value_gap_source_title: 'Graph-Bert: Only Attention is Needed for Learning Graph
      Representations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.59
    sort_std: null
    global_rank: 967
    paper_rank: 967
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
- &id002
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9296
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 19
    sort_value: 0.9296
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.808
    std: 0.6
    paper_value: 0.808
    paper_std: 0.6
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
    table_ref: Table 1
    source_ref: abu2019mixhop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9004
    true_std: 0.0141
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.09239999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: 0.0141
    global_rank: 85
    paper_rank: 433
    rank_delta: 348
    rank_delta_abs: 348
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.789
    std: 0.0
    paper_value: 0.789
    paper_std: 0.0
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
    table_ref: Table 1
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.789
    at_pub_std: 0.0
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.0055
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.09419999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.0055
    global_rank: 164
    paper_rank: 659
    rank_delta: 495
    rank_delta_abs: 495
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.869
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 243
    sort_value: 0.869
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.653
    std: null
    paper_value: 0.653
    paper_std: null
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
    table_ref: Table 1
    source_ref: perozzi2014deepwalk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.653
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8652
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.21219999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8652
    sort_std: 0.0012
    global_rank: 255
    paper_rank: 946
    rank_delta: 691
    rank_delta_abs: 691
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VPN
    model_key: vpn
    model_plain: VPN
    value: 0.798
    std: 0.4
    paper_value: 0.798
    paper_std: 0.4
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.4
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.4
    global_rank: 527
    paper_rank: 527
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.793
    std: 0.3
    paper_value: 0.793
    paper_std: 0.3
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.793
    true_std: 0.3
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.793
    sort_std: 0.3
    global_rank: 597
    paper_rank: 597
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: vanilla GCN
    model_key: vanilla gcn
    model_plain: vanilla GCN
    value: 0.79
    std: null
    paper_value: 0.79
    paper_std: null
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-03-17'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.79
    true_std: null
    value_gap_source_arxiv: '2003.07450'
    value_gap_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: null
    global_rank: 642
    paper_rank: 642
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PowerLaplacian
    model_key: powerlaplacian
    model_plain: PowerLaplacian
    value: 0.783
    std: null
    paper_value: 0.783
    paper_std: null
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.783
    true_std: null
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.783
    sort_std: null
    global_rank: 720
    paper_rank: 720
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LNet
    model_key: lnet
    model_plain: LNet
    value: 0.783
    std: 0.3
    paper_value: 0.783
    paper_std: 0.3
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
    table_ref: Table 1
    source_ref: liao2019lanczosnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.783
    true_std: 0.3
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.783
    sort_std: 0.3
    global_rank: 721
    paper_rank: 721
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: IGCN(AR)
    model_key: igcn(ar)
    model_plain: IGCN(AR)
    value: 0.782
    std: null
    paper_value: 0.782
    paper_std: null
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
    table_ref: Table 1
    source_ref: li2019label
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-24'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: null
    value_gap_source_arxiv: '1905.10029'
    value_gap_source_title: Power up! Robust Graph Convolutional Network via Graph
      Powering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: null
    global_rank: 727
    paper_rank: 727
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Planetoid
    model_key: planetoid
    model_plain: Planetoid
    value: 0.772
    std: null
    paper_value: 0.772
    paper_std: null
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
    table_ref: Table 1
    source_ref: yang2016revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.772
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2020-03-17'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.772
    true_std: null
    value_gap_source_arxiv: '2003.07450'
    value_gap_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: null
    global_rank: 798
    paper_rank: 798
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ICA
    model_key: ica
    model_plain: ICA
    value: 0.739
    std: null
    paper_value: 0.739
    paper_std: null
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
    table_ref: Table 1
    source_ref: lu2003link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.739
    at_pub_std: null
    at_pub_source_arxiv: '1710.10903'
    at_pub_source_title: Graph Attention Networks
    at_pub_source_date_iso: '2017-10-30'
    at_pub_source_date_label: ICLR 2017
    value_gap_source_date_iso: '2020-01-15'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: null
    value_gap_source_arxiv: '2001.05140'
    value_gap_source_title: 'Graph-Bert: Only Attention is Needed for Learning Graph
      Representations'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: null
    global_rank: 892
    paper_rank: 892
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SemiEmb
    model_key: semiemb
    model_plain: SemiEmb
    value: 0.711
    std: null
    paper_value: 0.711
    paper_std: null
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
    table_ref: Table 1
    source_ref: weston2012deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.717
    at_pub_std: null
    at_pub_source_arxiv: '1710.10903'
    at_pub_source_title: Graph Attention Networks
    at_pub_source_date_iso: '2017-10-30'
    at_pub_source_date_label: ICLR 2017
    value_gap_source_date_iso: '2017-10-30'
    value_gap_source_date_label: ICLR 2017
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.717
    true_std: null
    value_gap_source_arxiv: '1710.10903'
    value_gap_source_title: Graph Attention Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.717
    sort_std: null
    global_rank: 909
    paper_rank: 916
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Attention Networks
    comparison_source_arxiv: '1710.10903'
    is_best: false
    is_std_outlier: false
  - model: LP
    model_key: lp
    model_plain: LP
    value: 0.63
    std: null
    paper_value: 0.63
    paper_std: null
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
    table_ref: Table 1
    source_ref: zhu2003semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.63
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.716
    true_std: 0.0
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.08599999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.716
    sort_std: 0.0
    global_rank: 910
    paper_rank: 951
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ManiReg
    model_key: manireg
    model_plain: ManiReg
    value: 0.707
    std: null
    paper_value: 0.707
    paper_std: null
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
    table_ref: Table 1
    source_ref: belkin2006manifold
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labels per class for training, 500 labeled
      samples for hyper-parameter setting, and 1,000 samples for testing.'
    date: May 24, 2019
    date_display: May 2019
    date_iso: '2019-05-24'
    published_venue: AAAI 2019
    published_conference: AAAI 2019
    at_pub_value: 0.707
    at_pub_std: null
    at_pub_source_arxiv: '1611.08402'
    at_pub_source_title: Geometric deep learning on graphs and manifolds using mixture
      model CNNs
    at_pub_source_date_iso: '2016-11-25'
    at_pub_source_date_label: '2016'
    value_gap_source_date_iso: '2023-01-23'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.713
    true_std: 0.014
    value_gap_source_arxiv: '2301.09474'
    value_gap_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.713
    sort_std: 0.014
    global_rank: 915
    paper_rank: 919
    rank_delta: 4
    rank_delta_abs: 4
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
single_proposed_model: VPN
main_figure: /figures/1905.10029/main_figure.jpegoptim.jpg
---

