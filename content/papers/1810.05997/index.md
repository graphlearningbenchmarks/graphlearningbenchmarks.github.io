---
title: 'Predict then Propagate: Graph Neural Networks meet Personalized PageRank'
arxiv_id: '1810.05997'
source_url: ''
authors:
- name: Johannes Klicpera
  orcid: null
  s2_author_id: '51516539'
  s2_url: null
- name: Aleksandar Bojchevski
  orcid: null
  s2_author_id: '11754930'
  s2_url: null
- name: Stephan Günnemann
  orcid: null
  s2_author_id: '3075189'
  s2_url: null
published_date: Sep 27, 2018
published_date_iso: '2018-09-27'
published_venue: ICLR 2018
published_conference: ICLR 2018
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Neural message passing algorithms for semi-supervised classification on
  graphs have recently achieved great success. However, for classifying a node these
  methods only consider nodes that are a few propagation steps away and the size of
  this utilized neighborhood is hard to extend. In this paper, we use the relationship
  between graph convolutional networks (GCN) and PageRank to derive an improved propagation
  scheme based on personalized PageRank. We utilize this propagation procedure to
  construct a simple model, personalized propagation of neural predictions (PPNP),
  and its fast approximation, APPNP. Our model's training time is on par or faster
  and its number of parameters on par or lower than previous models. It leverages
  a large, adjustable neighborhood for classification and can be easily combined with
  any neural network. We show that this model outperforms several recently proposed
  methods for semi-supervised classification in the most thorough study done so far
  for GCN-like models. Our implementation is available online.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- APPNP
mrr: 0.0588
adjusted_mrr: 0.0196
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
  dataset: PubMed
  is_multi_metric: true
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    metric_values:
    - 0.9518
    - null
    metric_stds:
    - 0.0011
    - null
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
    published_venue: ''
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9518
    sort_std: 0.0011
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
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    metric_values:
    - 0.9513
    - null
    metric_stds:
    - 0.0038
    - null
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
    published_venue: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.9513
    sort_std: 0.0038
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
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    metric_values:
    - 0.9511
    - null
    metric_stds:
    - 0.0036
    - null
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
    published_venue: ''
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.9511
    sort_std: 0.0036
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    metric_values:
    - 0.7973
    - 0.7966
    metric_stds:
    - 0.0031
    - 0.0031
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9355
    sort_std: 0.006
    true_value: 0.9355
    true_std: 0.006
    paper_value: 0.7973
    paper_std: 0.0031
    has_value_gap: true
    has_value_note: false
    value_gap: 0.1382
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.7868
    - null
    metric_stds:
    - 0.0038
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9296
    sort_std: 0.0015
    true_value: 0.9296
    true_std: 0.0015
    paper_value: 0.7868
    paper_std: 0.0038
    has_value_gap: true
    has_value_note: false
    value_gap: 0.14279999999999993
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_note: ''
    at_pub_value: 0.79
    at_pub_std: null
    at_pub_source_arxiv: '1710.10370'
    at_pub_source_title: Topology Adaptive Graph Convolutional Networks
    at_pub_source_date_iso: '2017-10-28'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0031999999999999806
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.7776
    - null
    metric_stds:
    - 0.0044
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9233
    sort_std: 0.0018
    true_value: 0.9233
    true_std: 0.0018
    paper_value: 0.7776
    paper_std: 0.0044
    has_value_gap: true
    has_value_note: false
    value_gap: 0.14570000000000005
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_note: ''
    at_pub_value: 0.79
    at_pub_std: 0.003
    at_pub_source_arxiv: '1710.10370'
    at_pub_source_title: Topology Adaptive Graph Convolutional Networks
    at_pub_source_date_iso: '2017-10-28'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.012400000000000078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: behind
    comparison_source_title: Topology Adaptive Graph Convolutional Networks
    comparison_source_arxiv: '1710.10370'
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.8881
    - null
    metric_stds:
    - 0.0015
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    published_venue: ''
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 134
    is_best: false
    sort_value: 0.8881
    sort_std: 0.0015
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.869
    - null
    metric_stds:
    - 0.0074
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    published_venue: ''
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    is_global_top: true
    global_rank: 243
    is_best: false
    sort_value: 0.869
    sort_std: 0.0074
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
  - model: JK
    model_key: jk
    model_plain: JK
    metric_values:
    - 0.7788
    - null
    metric_stds:
    - 0.0038
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7788
    sort_std: 0.0038
    true_value: 0.7788
    true_std: 0.0038
    paper_value: 0.7788
    paper_std: 0.0038
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1810.05997'
    value_gap_source_title: 'Predict then Propagate: Graph Neural Networks meet Personalized
      PageRank'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-27'
    value_gap_source_date_label: ICLR 2018
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
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 762
  - model: V. GCN
    model_key: v. gcn
    model_plain: V. GCN
    metric_values:
    - 0.7765
    - null
    metric_stds:
    - 0.004
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7765
    sort_std: 0.004
    true_value: 0.7765
    true_std: 0.004
    paper_value: 0.7765
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1810.05997'
    value_gap_source_title: 'Predict then Propagate: Graph Neural Networks meet Personalized
      PageRank'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-27'
    value_gap_source_date_label: ICLR 2018
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
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 776
  - model: N-GCN
    model_key: n-gcn
    model_plain: N-GCN
    metric_values:
    - 0.7743
    - null
    metric_stds:
    - 0.0042
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7743
    sort_std: 0.0042
    true_value: 0.7743
    true_std: 0.0042
    paper_value: 0.7743
    paper_std: 0.0042
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1810.05997'
    value_gap_source_title: 'Predict then Propagate: Graph Neural Networks meet Personalized
      PageRank'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-27'
    value_gap_source_date_label: ICLR 2018
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
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 787
  - model: Bt. FP
    model_key: bt. fp
    model_plain: Bt. FP
    metric_values:
    - 0.7294
    - null
    metric_stds:
    - 0.01
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7294
    sort_std: 0.01
    true_value: 0.7294
    true_std: 0.01
    paper_value: 0.7294
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1810.05997'
    value_gap_source_title: 'Predict then Propagate: Graph Neural Networks meet Personalized
      PageRank'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-27'
    value_gap_source_date_label: ICLR 2018
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
    published_venue: ICLR 2018
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All graphs use a bag-of-words representation of the papers'
      abstracts as features.
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 902
  metrics:
  - Accuracy
  - F1
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - F1
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
    - dataset: PubMed
      dataset_slug: pubmed
single_proposed_model: APPNP
main_figure: /figures/1810.05997/main_figure.jpegoptim.jpg
---

