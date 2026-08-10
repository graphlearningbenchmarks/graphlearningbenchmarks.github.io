---
title: Revisiting the Necessity of Graph Learning and Common Graph Benchmarks
arxiv_id: '2412.06173'
source_url: ''
authors:
- name: Isay Katsman
  orcid: null
  s2_author_id: '31897469'
  s2_url: null
- name: Ethan Lou
  orcid: null
  s2_author_id: '2334472668'
  s2_url: null
- name: Anna Gilbert
  orcid: null
  s2_author_id: '2330191345'
  s2_url: null
published_date: Dec 9, 2024
published_date_iso: '2024-12-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph machine learning has enjoyed a meteoric rise in popularity since
  the introduction of deep learning in graph contexts. This is no surprise due to
  the ubiquity of graph data in large scale industrial settings. Tacitly assumed in
  all graph learning tasks is the separation of the graph structure and node features:
  node features strictly encode individual data while the graph structure consists
  only of pairwise interactions. The driving belief is that node features are (by
  themselves) insufficient for these tasks, so benchmark performance accurately reflects
  improvements in graph learning. In our paper, we challenge this orthodoxy by showing
  that, surprisingly, node features are oftentimes more-than-sufficient for many common
  graph benchmarks, breaking this critical assumption. When comparing against a well-tuned
  feature-only MLP baseline on seven of the most commonly used graph learning datasets,
  one gains little benefit from using graph structure on five datasets. We posit that
  these datasets do not benefit considerably from graph learning because the features
  themselves already contain enough graph information to obviate or substantially
  reduce the need for the graph. To illustrate this point, we perform a feature study
  on these datasets and show how the features are responsible for closing the gap
  between MLP and graph-method performance. Further, in service of introducing better
  empirical measures of progress for graph neural networks, we present a challenging
  parametric family of principled synthetic datasets that necessitate graph information
  for nontrivial performance. Lastly, we section out a subset of real-world datasets
  that are not trivially solved by an MLP and hence serve as reasonable benchmarks
  for graph neural networks.'
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
  evaluated: 7
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id005
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
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
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.826
    std: 0.024
    paper_value: 0.826
    paper_std: 0.024
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.916
    at_pub_std: 0.016
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09000000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.11520000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 439
    rank_delta: 437
    rank_delta_abs: 437
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.78
    std: 0.19
    paper_value: 0.78
    paper_std: 0.19
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.924
    at_pub_std: 0.013
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.14400000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.15979999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 499
    rank_delta: 496
    rank_delta_abs: 496
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
    value: 0.9351
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
    global_rank: 8
    sort_value: 0.9351
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.916
    std: 0.003
    paper_value: 0.916
    paper_std: 0.003
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Shirzad 2023
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9147
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0013000000000000789
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.918
    true_std: 0.0035
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.0035
    global_rank: 39
    paper_rank: 50
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGT
    model_key: cgt
    model_plain: CGT
    value: 0.915
    std: 0.006
    paper_value: 0.915
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hoang 2023
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.915
    true_std: 0.006
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.006
    global_rank: 54
    paper_rank: 54
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
    value: 0.826
    std: 0.006
    paper_value: 0.826
    paper_std: 0.006
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8463
    at_pub_std: null
    at_pub_source_arxiv: '2407.11907'
    at_pub_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.020300000000000096
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8463
    true_std: null
    value_gap_source_arxiv: '2407.11907'
    value_gap_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    value_gap_source_is_current_paper: false
    value_gap: 0.020300000000000096
    has_value_note: false
    value_note: ''
    sort_value: 0.8463
    sort_std: null
    global_rank: 365
    paper_rank: 439
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphFM: A generalist graph transformer that learns
      transferable representations across diverse domains'
    comparison_source_arxiv: '2407.11907'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.845
    std: 0.012
    paper_value: 0.845
    paper_std: 0.012
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.845
    at_pub_std: 0.012
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.012
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.012
    global_rank: 369
    paper_rank: 369
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.835
    std: 0.022
    paper_value: 0.835
    paper_std: 0.022
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Monti 2016
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.835
    at_pub_std: 0.022
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2026-05-20'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.022
    value_gap_source_arxiv: '2605.21247'
    value_gap_source_title: Graph Navier–Stokes Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.022
    global_rank: 413
    paper_rank: 413
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-mean
    model_key: sage-mean
    model_plain: SAGE-mean
    value: 0.824
    std: 0.018
    paper_value: 0.824
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.824
    true_std: 0.018
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.824
    sort_std: 0.018
    global_rank: 446
    paper_rank: 446
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-meanpool
    model_key: sage-meanpool
    model_plain: SAGE-meanpool
    value: 0.799
    std: 0.023
    paper_value: 0.799
    paper_std: 0.023
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.799
    true_std: 0.023
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.023
    global_rank: 485
    paper_rank: 485
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp NL
    model_key: labelprop nl
    model_plain: LabelProp NL
    value: 0.75
    std: 0.029
    paper_value: 0.75
    paper_std: 0.029
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.75
    at_pub_std: 0.029
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.75
    true_std: 0.029
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.75
    sort_std: 0.029
    global_rank: 512
    paper_rank: 512
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.708
    std: 0.081
    paper_value: 0.708
    paper_std: 0.081
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: 0.081
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.708
    true_std: 0.081
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: 0.081
    global_rank: 533
    paper_rank: 533
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LogReg
    model_key: logreg
    model_plain: LogReg
    value: 0.641
    std: 0.057
    paper_value: 0.641
    paper_std: 0.057
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Computers (standard split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.641
    at_pub_std: 0.057
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.641
    true_std: 0.057
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.641
    sort_std: 0.057
    global_rank: 545
    paper_rank: 545
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
- &id004
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
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
    global_rank: 1
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
    value: 0.857
    std: 0.203
    paper_value: 0.857
    paper_std: 0.203
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9498
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0928
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.1099
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 554
    rank_delta: 552
    rank_delta_abs: 552
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
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
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.912
    std: 0.012
    paper_value: 0.912
    paper_std: 0.012
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9476
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.035599999999999965
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.05119999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 431
    rank_delta: 422
    rank_delta_abs: 422
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: CGT
    model_key: cgt
    model_plain: CGT
    value: 0.958
    std: 0.008
    paper_value: 0.958
    paper_std: 0.008
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hoang 2023
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9573
    at_pub_std: 0.0084
    at_pub_source_arxiv: '2412.04064'
    at_pub_source_title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    at_pub_source_date_iso: '2024-12-05'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0006999999999999229
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.008
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.008
    global_rank: 21
    paper_rank: 21
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
    value: 0.953
    std: 0.004
    paper_value: 0.953
    paper_std: 0.004
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Shirzad 2023
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9536
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2411.16278'
    at_pub_source_title: Even Sparser Graph Transformers
    at_pub_source_date_iso: '2024-11-25'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0006000000000000449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9569
    true_std: 0.0039
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0039000000000000146
    has_value_note: false
    value_note: ''
    sort_value: 0.9569
    sort_std: 0.0039
    global_rank: 26
    paper_rank: 50
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.92
    std: 0.008
    paper_value: 0.92
    paper_std: 0.008
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9269
    at_pub_std: null
    at_pub_source_arxiv: '2012.03476'
    at_pub_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    at_pub_source_date_iso: '2020-12-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.006899999999999906
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9269
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.006899999999999906
    has_value_note: false
    value_note: ''
    sort_value: 0.9269
    sort_std: null
    global_rank: 290
    paper_rank: 372
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-mean
    model_key: sage-mean
    model_plain: SAGE-mean
    value: 0.914
    std: 0.013
    paper_value: 0.914
    paper_std: 0.013
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.914
    true_std: 0.013
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: 0.013
    global_rank: 418
    paper_rank: 418
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
    value: 0.88
    std: 0.01
    paper_value: 0.88
    paper_std: 0.01
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9128
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03279999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.03279999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0063
    global_rank: 426
    paper_rank: 539
    rank_delta: 113
    rank_delta_abs: 113
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.912
    std: 0.013
    paper_value: 0.912
    paper_std: 0.013
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Monti 2016
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9124
    at_pub_std: 0.013
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9124
    true_std: 0.013
    value_gap_source_arxiv: '2302.08727'
    value_gap_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9124
    sort_std: 0.013
    global_rank: 429
    paper_rank: 431
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-meanpool
    model_key: sage-meanpool
    model_plain: SAGE-meanpool
    value: 0.907
    std: 0.016
    paper_value: 0.907
    paper_std: 0.016
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.907
    true_std: 0.016
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.907
    sort_std: 0.016
    global_rank: 456
    paper_rank: 456
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-maxpool
    model_key: sage-maxpool
    model_plain: SAGE-maxpool
    value: 0.904
    std: 0.013
    paper_value: 0.904
    paper_std: 0.013
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.013
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.013
    global_rank: 477
    paper_rank: 477
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp NL
    model_key: labelprop nl
    model_plain: LabelProp NL
    value: 0.839
    std: 0.027
    paper_value: 0.839
    paper_std: 0.027
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.839
    at_pub_std: 0.027
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.027
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.027
    global_rank: 572
    paper_rank: 572
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LogReg
    model_key: logreg
    model_plain: LogReg
    value: 0.73
    std: 0.065
    paper_value: 0.73
    paper_std: 0.065
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.73
    at_pub_std: 0.065
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.73
    true_std: 0.065
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: 0.065
    global_rank: 607
    paper_rank: 607
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.726
    std: 0.111
    paper_value: 0.726
    paper_std: 0.111
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Amazon Photo split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.726
    at_pub_std: 0.111
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: 0.111
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.111
    global_rank: 608
    paper_rank: 608
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
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
- &id003
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8774
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.711
    std: 0.007
    paper_value: 0.711
    paper_std: 0.007
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
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8769
    at_pub_std: 0.004
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.16590000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.16590000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 612
    rank_delta: 591
    rank_delta_abs: 591
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.718
    std: 0.004
    paper_value: 0.718
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
    input_feature_source: raw_features
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Klicpera 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8142
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.09620000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8142
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09620000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 533
    rank_delta: 504
    rank_delta_abs: 504
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: ACM-Snowball-3
    model_key: acm-snowball-3
    model_plain: ACM-Snowball-3
    value: 0.813
    std: 0.01
    paper_value: 0.813
    paper_std: 0.01
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
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Luan 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.813
    true_std: 0.01
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.813
    sort_std: 0.01
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.708
    std: 0.005
    paper_value: 0.708
    paper_std: 0.005
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
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.808
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.10000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 632
    rank_delta: 586
    rank_delta_abs: 586
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: SSP
    model_key: ssp
    model_plain: SSP
    value: 0.805
    std: 0.001
    paper_value: 0.805
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Izadi 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.001
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.001
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.713
    std: 0.002
    paper_value: 0.713
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
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Wu 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7965
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08350000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7965
    true_std: 0.0102
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.08350000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0102
    global_rank: 68
    paper_rank: 587
    rank_delta: 519
    rank_delta_abs: 519
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.696
    std: 0.014
    paper_value: 0.696
    paper_std: 0.014
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
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Defferrard 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7933
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.09730000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7933
    true_std: 0.0057
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.09730000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0057
    global_rank: 75
    paper_rank: 698
    rank_delta: 623
    rank_delta_abs: 623
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.733
    std: 0.006
    paper_value: 0.733
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
    input_feature_source: raw_features
    feature_source_evidence: standard graph task results
    table_ref: "Table \ref{tab:citationdatasets}"
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.786
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.05300000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.786
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.786
    sort_std: null
    global_rank: 92
    paper_rank: 340
    rank_delta: 248
    rank_delta_abs: 248
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.66
    std: 0.005
    paper_value: 0.66
    paper_std: 0.005
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
    input_feature_source: raw_features
    feature_source_evidence: MLP (tuned) ... operating solely on node features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.719
    at_pub_std: 0.0169
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05899999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7289
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.06889999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 819
    rank_delta: 418
    rank_delta_abs: 418
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
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
- &id007
  dataset: Coauthor-CS
  rows:
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.969
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-fa
    model_key: gwn-fa
    model_plain: GWN-fa
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-sym
    model_key: gwn-sym
    model_plain: GWN-sym
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9593
    std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: 0.9593
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.958
    std: 0.002
    paper_value: 0.958
    paper_std: 0.002
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Shirzad 2023
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.002
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.002
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.911
    std: 0.005
    paper_value: 0.911
    paper_std: 0.005
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.936
    at_pub_std: 0.015
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.025000000000000022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9514
    true_std: 0.0025
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04039999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0025
    global_rank: 14
    paper_rank: 161
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Convolutional Neural Networks and Label
      Propagation
    comparison_source_arxiv: '2002.06755'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.905
    std: 0.006
    paper_value: 0.905
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.938
    at_pub_std: 0.004
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.03299999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9437
    true_std: 0.0028
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03869999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9437
    sort_std: 0.0028
    global_rank: 23
    paper_rank: 170
    rank_delta: 147
    rank_delta_abs: 147
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Convolutional Neural Networks and Label
      Propagation
    comparison_source_arxiv: '2002.06755'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.928
    std: 0.009
    paper_value: 0.928
    paper_std: 0.009
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9278
    at_pub_std: 0.009
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.928
    true_std: 0.009
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.009
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.928
    std: 0.002
    paper_value: 0.928
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.917
    at_pub_std: 0.014
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.928
    true_std: 0.002
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.002
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-mean
    model_key: sage-mean
    model_plain: SAGE-mean
    value: 0.913
    std: 0.028
    paper_value: 0.913
    paper_std: 0.028
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.913
    true_std: 0.028
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.028
    global_rank: 157
    paper_rank: 157
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.908
    std: 0.006
    paper_value: 0.908
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Monti 2016
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9082
    at_pub_std: 0.016
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9082
    true_std: 0.016
    value_gap_source_arxiv: '2302.08727'
    value_gap_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.9082
    sort_std: 0.016
    global_rank: 169
    paper_rank: 169
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-meanpool
    model_key: sage-meanpool
    model_plain: SAGE-meanpool
    value: 0.896
    std: 0.009
    paper_value: 0.896
    paper_std: 0.009
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.896
    true_std: 0.009
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.896
    sort_std: 0.009
    global_rank: 183
    paper_rank: 183
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LogReg
    model_key: logreg
    model_plain: LogReg
    value: 0.864
    std: 0.009
    paper_value: 0.864
    paper_std: 0.009
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.864
    at_pub_std: 0.009
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.864
    true_std: 0.009
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: 0.009
    global_rank: 198
    paper_rank: 198
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-maxpool
    model_key: sage-maxpool
    model_plain: SAGE-maxpool
    value: 0.85
    std: 0.011
    paper_value: 0.85
    paper_std: 0.011
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.011
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.011
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp NL
    model_key: labelprop nl
    model_plain: LabelProp NL
    value: 0.767
    std: 0.014
    paper_value: 0.767
    paper_std: 0.014
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.767
    at_pub_std: 0.014
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.767
    true_std: 0.014
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.767
    sort_std: 0.014
    global_rank: 215
    paper_rank: 215
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.736
    std: 0.039
    paper_value: 0.736
    paper_std: 0.039
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy on Coauthor CS split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.736
    at_pub_std: 0.039
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.736
    true_std: 0.039
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.736
    sort_std: 0.039
    global_rank: 220
    paper_rank: 220
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
- &id006
  dataset: Coauthor-Physics
  rows:
  - model: GrokFormer
    model_key: grokformer
    model_plain: GrokFormer
    value: 0.9831
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9831
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PolyFormer
    model_key: polyformer
    model_plain: PolyFormer
    value: 0.9808
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9808
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9796
    std: 0.0081
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9796
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.925
    std: 0.009
    paper_value: 0.925
    paper_std: 0.009
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9782
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.053199999999999914
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9782
    true_std: 0.0028
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.053199999999999914
    has_value_note: false
    value_note: ''
    sort_value: 0.9782
    sort_std: 0.0028
    global_rank: 6
    paper_rank: 283
    rank_delta: 277
    rank_delta_abs: 277
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.928
    std: 0.01
    paper_value: 0.928
    paper_std: 0.01
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9774
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0494
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9774
    true_std: 0.0035
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0494
    has_value_note: false
    value_note: ''
    sort_value: 0.9774
    sort_std: 0.0035
    global_rank: 9
    paper_rank: 273
    rank_delta: 264
    rank_delta_abs: 264
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9739
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 18
    sort_value: 0.9739
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.972
    std: 0.001
    paper_value: 0.972
    paper_std: 0.001
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Shirzad 2023
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9689
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0030999999999999917
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.972
    true_std: 0.001
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.972
    sort_std: 0.001
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.948
    std: 0.004
    paper_value: 0.948
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: a thoroughly tuned multi-layer perceptron (MLP) operating
      solely on node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9563
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.008300000000000085
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9597
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.011700000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.9597
    sort_std: 0.0007
    global_rank: 83
    paper_rank: 191
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.94
    std: 0.006
    paper_value: 0.94
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9401
    at_pub_std: 0.006
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00010000000000010001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9401
    true_std: 0.006
    value_gap_source_arxiv: '2302.08727'
    value_gap_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000010001
    has_value_note: false
    value_note: ''
    sort_value: 0.9401
    sort_std: 0.006
    global_rank: 222
    paper_rank: 223
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-mean
    model_key: sage-mean
    model_plain: SAGE-mean
    value: 0.93
    std: 0.008
    paper_value: 0.93
    paper_std: 0.008
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.93
    true_std: 0.008
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.93
    sort_std: 0.008
    global_rank: 272
    paper_rank: 272
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-meanpool
    model_key: sage-meanpool
    model_plain: SAGE-meanpool
    value: 0.926
    std: 0.01
    paper_value: 0.926
    paper_std: 0.01
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.926
    true_std: 0.01
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.926
    sort_std: 0.01
    global_rank: 279
    paper_rank: 279
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.925
    std: 0.009
    paper_value: 0.925
    paper_std: 0.009
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Monti 2016
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.925
    at_pub_std: 0.009
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.925
    true_std: 0.009
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.925
    sort_std: 0.009
    global_rank: 284
    paper_rank: 284
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE-maxpool
    model_key: sage-maxpool
    model_plain: SAGE-maxpool
    value: 0.903
    std: 0.012
    paper_value: 0.903
    paper_std: 0.012
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
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Hamilton 2017
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.012
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.012
    global_rank: 304
    paper_rank: 304
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp NL
    model_key: labelprop nl
    model_plain: LabelProp NL
    value: 0.868
    std: 0.014
    paper_value: 0.868
    paper_std: 0.014
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.868
    at_pub_std: 0.014
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.868
    true_std: 0.014
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.014
    global_rank: 307
    paper_rank: 307
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LogReg
    model_key: logreg
    model_plain: LogReg
    value: 0.867
    std: 0.015
    paper_value: 0.867
    paper_std: 0.015
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.867
    at_pub_std: 0.015
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.867
    true_std: 0.015
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.867
    sort_std: 0.015
    global_rank: 308
    paper_rank: 308
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.866
    std: 0.02
    paper_value: 0.866
    paper_std: 0.02
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features can sufficiently
      close the gap
    table_ref: "Table \ref{tab:codatasets}"
    source_ref: Thomas 2009
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Coauthor Physics split from DGL
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.866
    at_pub_std: 0.02
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.866
    true_std: 0.02
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.866
    sort_std: 0.02
    global_rank: 309
    paper_rank: 309
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
  - model: SSP
    model_key: ssp
    model_plain: SSP
    value: 0.902
    std: 0.006
    paper_value: 0.902
    paper_std: 0.006
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
    input_feature_source: raw_features
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Izadi 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9016
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2412.04064'
    at_pub_source_title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    at_pub_source_date_iso: '2024-12-05'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.902
    true_std: 0.006
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.902
    sort_std: 0.006
    global_rank: 29
    paper_rank: 29
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
    value: 0.813
    std: 0.008
    paper_value: 0.813
    paper_std: 0.008
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08740000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08740000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 668
    rank_delta: 637
    rank_delta_abs: 637
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: ACM-Snowball-3
    model_key: acm-snowball-3
    model_plain: ACM-Snowball-3
    value: 0.896
    std: 0.016
    paper_value: 0.896
    paper_std: 0.016
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Luan 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8959
    at_pub_std: null
    at_pub_source_arxiv: '2310.16421'
    at_pub_source_title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.896
    true_std: 0.016
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.896
    sort_std: 0.016
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
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
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.833
    std: 0.005
    paper_value: 0.833
    paper_std: 0.005
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Klicpera 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8904
    at_pub_std: 0.015
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.05740000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8904
    true_std: 0.015
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.05740000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 65
    paper_rank: 460
    rank_delta: 395
    rank_delta_abs: 395
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.831
    std: 0.004
    paper_value: 0.831
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
    input_feature_source: raw_features
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05800000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.058700000000000085
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 489
    rank_delta: 422
    rank_delta_abs: 422
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.844
    std: 0.005
    paper_value: 0.844
    paper_std: 0.005
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.884
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.040000000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.884
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: null
    global_rank: 100
    paper_rank: 321
    rank_delta: 221
    rank_delta_abs: 221
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.805
    std: 0.011
    paper_value: 0.805
    paper_std: 0.011
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Defferrard 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8832
    at_pub_std: 0.02
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07819999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.02
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.07819999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.02
    global_rank: 104
    paper_rank: 714
    rank_delta: 610
    rank_delta_abs: 610
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.817
    std: 0.001
    paper_value: 0.817
    paper_std: 0.001
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
    feature_source_evidence: standard graph learning task
    table_ref: Table 2
    source_ref: Wu 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05130000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.05130000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8683
    sort_std: 0.0128
    global_rank: 202
    paper_rank: 642
    rank_delta: 440
    rank_delta_abs: 440
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.694
    std: 0.013
    paper_value: 0.694
    paper_std: 0.013
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
    input_feature_source: raw_features
    feature_source_evidence: MLP operating solely on node features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0828000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0828000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 909
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.801
    std: 0.002
    paper_value: 0.801
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
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Klicpera 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9355
    at_pub_std: 0.006
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.13449999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9355
    true_std: 0.006
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.13449999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9355
    sort_std: 0.006
    global_rank: 17
    paper_rank: 491
    rank_delta: 474
    rank_delta_abs: 474
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.788
    std: 0.006
    paper_value: 0.788
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
    input_feature_source: raw_features
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Kipf 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10899999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: 0.0015
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.14159999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 675
    rank_delta: 656
    rank_delta_abs: 656
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.791
    std: 0.004
    paper_value: 0.791
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
    input_feature_source: raw_features
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Velickovic 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10599999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: 0.0018
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.13229999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 628
    rank_delta: 605
    rank_delta_abs: 605
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: SSP
    model_key: ssp
    model_plain: SSP
    value: 0.878
    std: 0.002
    paper_value: 0.878
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Izadi 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9178
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03979999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9178
    true_std: 0.0116
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.03979999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9178
    sort_std: 0.0116
    global_rank: 25
    paper_rank: 192
    rank_delta: 167
    rank_delta_abs: 167
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: ACM-Snowball-3
    model_key: acm-snowball-3
    model_plain: ACM-Snowball-3
    value: 0.914
    std: 0.004
    paper_value: 0.914
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
    input_feature_source: raw_features
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Luan 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9144
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2412.04064'
    at_pub_source_title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    at_pub_source_date_iso: '2024-12-05'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-12-05'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9144
    true_std: 0.0059
    value_gap_source_arxiv: '2412.04064'
    value_gap_source_title: Graph Neural Networks Need Cluster-Normalize-Activate
      Modules
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9144
    sort_std: 0.0059
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8881
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
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 134
    sort_value: 0.8881
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.789
    std: 0.001
    paper_value: 0.789
    paper_std: 0.001
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
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Wu 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8832
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09419999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.781
    std: 0.006
    paper_value: 0.781
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
    input_feature_source: raw_features
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Defferrard 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8782
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.09719999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8782
    true_std: 0.0024
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.09719999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8782
    sort_std: 0.0024
    global_rank: 190
    paper_rank: 734
    rank_delta: 544
    rank_delta_abs: 544
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.868
    std: 0.004
    paper_value: 0.868
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: MLP (tuned) ... operating solely on node features
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 246
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.805
    std: 0.005
    paper_value: 0.805
    paper_std: 0.005
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
    feature_source_evidence: Graph NN ... node classification
    table_ref: Table 2
    source_ref: Liu 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.864
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.05899999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.864
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05899999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: null
    global_rank: 259
    paper_rank: 453
    rank_delta: 194
    rank_delta_abs: 194
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
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
  - *id003
  - *id004
  - *id005
  - *id006
  - *id007
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
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
main_figure: /figures/2412.06173/main_figure.jpegoptim.jpg
---

