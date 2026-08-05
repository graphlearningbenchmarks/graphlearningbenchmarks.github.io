---
title: Fully-inductive Node Classification on Arbitrary Graphs
arxiv_id: '2405.20445'
source_url: ''
authors:
- name: Jianan Zhao
  orcid: null
  s2_author_id: '2282988161'
  s2_url: null
- name: Hesham Mostafa
  orcid: null
  s2_author_id: '2256992354'
  s2_url: null
- name: Mikhail Galkin
  orcid: null
  s2_author_id: '2066369448'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2253393509'
  s2_url: null
- name: Zhaocheng Zhu
  orcid: null
  s2_author_id: '9031926'
  s2_url: null
- name: Jian Tang
  orcid: null
  s2_author_id: '2255480226'
  s2_url: null
published_date: May 30, 2024
published_date_iso: '2024-05-30'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: One fundamental challenge in graph machine learning is generalizing to new
  graphs. Many existing methods following the inductive setup can generalize to test
  graphs with new structures, but assuming the feature and label spaces remain the
  same as the training ones. This paper introduces a fully-inductive setup, where
  models should perform inference on arbitrary test graphs with new structures, feature
  and label spaces. We propose GraphAny as the first attempt at this challenging setup.
  GraphAny models inference on a new graph as an analytical solution to a LinearGNN,
  which can be naturally applied to graphs with any feature and label spaces. To further
  build a stronger model with learning capacity, we fuse multiple LinearGNN predictions
  with learned inductive attention scores. Specifically, the attention module is carefully
  parameterized as a function of the entropy-normalized distance features between
  pairs of LinearGNN predictions to ensure generalization to new graphs. Empirically,
  GraphAny trained on a single Wisconsin dataset with only 120 labeled nodes can generalize
  to 30 new graphs with an average accuracy of 67.26\
codebase_url: https://github.com/DeepGraphLearning/GraphAny
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphAny
mrr: 0.0051
adjusted_mrr: 0.0051
mrr_dataset_count: 3
benchmark_categories:
- Classic
- OGB
- Heterophily Benchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.814
    std: 0.007
    paper_value: 0.814
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08640000000000003
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
    value_gap: 0.08640000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 700
    rank_delta: 667
    rank_delta_abs: 667
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.817
    std: 0.0143
    paper_value: 0.817
    paper_std: 0.0143
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.07200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0727000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 680
    rank_delta: 608
    rank_delta_abs: 608
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: LinearSGC2
    model_key: linearsgc2
    model_plain: LinearSGC2
    value: 0.782
    std: 0.0
    paper_value: 0.782
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.0
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.0
    global_rank: 827
    paper_rank: 827
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
    value: 0.4842
    std: 0.0063
    paper_value: 0.4842
    paper_std: 0.0063
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2926
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
    value_gap: 0.2926
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 840
    paper_rank: 1031
    rank_delta: 191
    rank_delta_abs: 191
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: LinearSGC1
    model_key: linearsgc1
    model_plain: LinearSGC1
    value: 0.743
    std: 0.0
    paper_value: 0.743
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.743
    true_std: 0.0
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.0
    global_rank: 894
    paper_rank: 894
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.528
    std: 0.0
    paper_value: 0.528
    paper_std: 0.0
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7237
    true_std: 0.0033
    value_gap_source_arxiv: '2601.21369'
    value_gap_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.19569999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7237
    sort_std: 0.0033
    global_rank: 914
    paper_rank: 1017
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.603
    std: 0.0
    paper_value: 0.603
    paper_std: 0.0
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.603
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.0
    global_rank: 991
    paper_rank: 991
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LinearHGC2
    model_key: linearhgc2
    model_plain: LinearHGC2
    value: 0.238
    std: 0.0
    paper_value: 0.238
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.238
    true_std: 0.0
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.238
    sort_std: 0.0
    global_rank: 1066
    paper_rank: 1066
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LinearHGC1
    model_key: linearhgc1
    model_plain: LinearHGC1
    value: 0.225
    std: 0.0
    paper_value: 0.225
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification accuracy.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.225
    true_std: 0.0
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.225
    sort_std: 0.0
    global_rank: 1068
    paper_rank: 1068
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
  dataset: Questions
  rows:
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9733
    std: null
    paper_value: 0.9733
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 3 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification task on Questions dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9733
    true_std: 0.0006
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9733
    sort_std: 0.0006
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
  - model: CR-TAS
    model_key: ags-gnn
    model_plain: CR-TAS
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
  - model: CR-TAS
    model_key: meangnn
    model_plain: CR-TAS
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
    value: 0.9715
    std: null
    paper_value: 0.9715
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 3 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification task on Questions dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7609
    at_pub_std: null
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.2106
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9715
    true_std: 0.0004
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9715
    sort_std: 0.0004
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9711
    std: null
    paper_value: 0.9711
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 3 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification task on Questions dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7743
    at_pub_std: null
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.19679999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9713
    true_std: 0.0005
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.9713
    sort_std: 0.0005
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GraphAny
    model_key: graphany
    model_plain: GraphAny
    value: 0.971
    std: null
    paper_value: 0.971
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: true
    override_reason: Table 3 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification task on Questions dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.971
    true_std: null
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.971
    sort_std: null
    global_rank: 7
    paper_rank: 7
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
  dataset: Reddit
  rows:
  - model: Cluster-GCN (2019)
    model_key: node sampled soup
    model_plain: Cluster-GCN (2019)
    value: 0.9728
    std: 0.0008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_display: Jun 2023
    date_iso: '2023-06-18'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/VITA-Group/graph_ladling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9728
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Cluster-GCN (2019)
    model_key: engcn
    model_plain: Cluster-GCN (2019)
    value: 0.9714
    std: 0.0003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9714
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cluster-GCN (2019)
    model_key: sagn+sle
    model_plain: Cluster-GCN (2019)
    value: 0.971
    std: 0.0
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.971
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9276
    std: 0.0046
    paper_value: 0.9276
    paper_std: 0.0046
    metric: F1
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.96
    at_pub_std: 0.001
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.032399999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.96
    true_std: 0.001
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.032399999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.96
    sort_std: 0.001
    global_rank: 45
    paper_rank: 131
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    comparison_source_arxiv: '2205.10803'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9489
    std: 0.0002
    paper_value: 0.9489
    paper_std: 0.0002
    metric: F1
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.953
    at_pub_std: 0.001
    at_pub_source_arxiv: '2205.10803'
    at_pub_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    at_pub_source_date_iso: '2022-05-22'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-05-22'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.0040999999999999925
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.953
    true_std: 0.001
    value_gap_source_arxiv: '2205.10803'
    value_gap_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.0040999999999999925
    has_value_note: false
    value_note: ''
    sort_value: 0.953
    sort_std: 0.001
    global_rank: 69
    paper_rank: 87
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    comparison_source_arxiv: '2205.10803'
    is_best: false
    is_std_outlier: false
  - model: GraphAny
    model_key: graphany
    model_plain: GraphAny
    value: 0.91
    std: 0.0024
    paper_value: 0.91
    paper_std: 0.0024
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset using GraphAny variant trained on Wisconsin
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.91
    true_std: 0.0024
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.91
    sort_std: 0.0024
    global_rank: 143
    paper_rank: 143
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
    value: 0.7216
    std: 0.0015
    paper_value: 0.7216
    paper_std: 0.0015
    metric: F1
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
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7435
    true_std: 0.0016
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.02190000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7435
    sort_std: 0.0016
    global_rank: 153
    paper_rank: 156
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7912
    std: 0.0045
    paper_value: 0.7912
    paper_std: 0.0045
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard WikiCS node classification task.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.9302
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.139
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.139
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 78
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rse + rgcn (70b)
    model_plain: GPM
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPM
    model_key: rse + sehgnn (70b)
    model_plain: GPM
    value: 0.8796
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 3
    sort_value: 0.8796
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7927
    std: 0.002
    paper_value: 0.7927
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
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard WikiCS node classification task.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.8279
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2405.18581'
    at_pub_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    at_pub_source_date_iso: '2024-05-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03520000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8279
    true_std: 0.0016
    value_gap_source_arxiv: '2405.18581'
    value_gap_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.03520000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8279
    sort_std: 0.0016
    global_rank: 23
    paper_rank: 73
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unleashing the Potential of Text-attributed Graphs:
      Automatic Relation Decomposition via Large Language Models'
    comparison_source_arxiv: '2405.18581'
    is_best: false
    is_std_outlier: false
  - model: GraphAny
    model_key: graphany
    model_plain: GraphAny
    value: 0.7501
    std: 0.0054
    paper_value: 0.7501
    paper_std: 0.0054
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard WikiCS node classification task using
      GraphAny trained on Products.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7501
    true_std: 0.0054
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7501
    sort_std: 0.0054
    global_rank: 180
    paper_rank: 180
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
    value: 0.7272
    std: 0.0043
    paper_value: 0.7272
    paper_std: 0.0043
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
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard WikiCS node classification task.
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7198
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.007399999999999962
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.734
    true_std: 0.006
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.006800000000000028
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.006
    global_rank: 191
    paper_rank: 193
    rank_delta: 2
    rank_delta_abs: 2
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
- &id005
  dataset: ogbn-arxiv
  rows:
  - model: EGP (GCN)
    model_key: ofa
    model_plain: EGP (GCN)
    value: 0.7764
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2407.19941'
    title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
      Graphs from Structural Perspective
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: null
    codebase_url: https://github.com/cy623/BooG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7764
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EGP (GCN)
    model_key: giant-xrt
    model_plain: EGP (GCN)
    value: 0.7612
    std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_display: Oct 2021
    date_iso: '2021-10-29'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amzn/pecos
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7612
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGP (GCN)
    model_key: gegcn
    model_plain: EGP (GCN)
    value: 0.7576
    std: 0.0064
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_display: Mar 2026
    date_iso: '2026-03-27'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrates Ricci flow with deep graph models... multi-scale
      structural information is then incorporated into a GCN
    is_global_top: true
    global_rank: 3
    sort_value: 0.7576
    sort_std: 0.0064
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7365
    std: 0.0011
    paper_value: 0.7365
    paper_std: 0.0011
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
    protocol_note: Accuracy on the standard OGB-Arxiv split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7206
    at_pub_std: null
    at_pub_source_arxiv: '2010.00238'
    at_pub_source_title: Multi-grained Semantics-aware Graph Neural Networks
    at_pub_source_date_iso: '2020-10-01'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.015900000000000025
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7391
    true_std: null
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0025999999999999357
    has_value_note: false
    value_note: ''
    sort_value: 0.7391
    sort_std: null
    global_rank: 13
    paper_rank: 16
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multi-grained Semantics-aware Graph Neural Networks
    comparison_source_arxiv: '2010.00238'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7174
    std: 0.0029
    paper_value: 0.7174
    paper_std: 0.0029
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
    protocol_note: Accuracy on the standard OGB-Arxiv split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.7192
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2403.12529'
    at_pub_source_title: Contextualized Messages Boost Graph Representations
    at_pub_source_date_iso: '2024-03-19'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-03-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0017999999999999128
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.73
    true_std: 0.0017
    value_gap_source_arxiv: '2603.26178'
    value_gap_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    value_gap_source_is_current_paper: false
    value_gap: 0.012599999999999945
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: 0.0017
    global_rank: 25
    paper_rank: 63
    rank_delta: 38
    rank_delta_abs: 38
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
    value: 0.555
    std: 0.0023
    paper_value: 0.555
    paper_std: 0.0023
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard OGB-Arxiv split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.563
    at_pub_std: 0.003
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.007999999999999896
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6831
    true_std: null
    value_gap_source_arxiv: '2407.19941'
    value_gap_source_title: Boosting Cross-Domain and Cross-Task Generalization for
      Text-Attributed Graphs from Structural Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.1281
    has_value_note: false
    value_note: ''
    sort_value: 0.6831
    sort_std: null
    global_rank: 104
    paper_rank: 122
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    comparison_source_arxiv: '2312.02619'
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
  dataset: ogbn-products
  rows:
  - model: LargeGT-full
    model_key: advsyngnn
    model_plain: LargeGT-full
    value: 0.8931
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
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8931
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: gofa-f
    model_plain: LargeGT-full
    value: 0.8834
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.09709'
    title: 'GOFA: A Generative One-For-All Model for Joint Graph Language Modeling'
    date: Jul 12, 2024
    date_display: Jul 2024
    date_iso: '2024-07-12'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/JiaruiFeng/GOFA
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8834
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: llms
    model_plain: LargeGT-full
    value: 0.882
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2412.16441'
    title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
      Task-Trees'
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Zehong-Wang/GIT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.882
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7945
    std: 0.0059
    paper_value: 0.7945
    paper_std: 0.0059
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
    protocol_note: Accuracy on the standard ogbn-products split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.801
    at_pub_std: 0.006
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.006500000000000061
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8722
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.07769999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8722
    sort_std: 0.0005
    global_rank: 9
    paper_rank: 163
    rank_delta: 154
    rank_delta_abs: 154
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7579
    std: 0.0012
    paper_value: 0.7579
    paper_std: 0.0012
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
    protocol_note: Accuracy on the standard ogbn-products split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.824
    at_pub_std: 0.004
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.06609999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8691
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.11119999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8691
    sort_std: 0.0005
    global_rank: 12
    paper_rank: 250
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6106
    std: 0.0008
    paper_value: 0.6106
    paper_std: 0.0008
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard ogbn-products split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.8418
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2112.04319'
    at_pub_source_title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    at_pub_source_date_iso: '2021-12-08'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-11-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.23119999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6605
    true_std: 0.002
    value_gap_source_arxiv: '2211.16199'
    value_gap_source_title: Latent Graph Inference using Product Manifolds
    value_gap_source_is_current_paper: false
    value_gap: 0.049899999999999944
    has_value_note: false
    value_note: ''
    sort_value: 0.6605
    sort_std: 0.002
    global_rank: 353
    paper_rank: 371
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SCR: Training Graph Neural Networks with Consistency
      Regularization'
    comparison_source_arxiv: '2112.04319'
    is_best: false
    is_std_outlier: false
  - model: GraphAny
    model_key: graphany
    model_plain: GraphAny
    value: 0.6119
    std: 0.0023
    paper_value: 0.6119
    paper_std: 0.0023
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard ogbn-products split
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6119
    true_std: 0.0023
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6119
    sort_std: 0.0023
    global_rank: 370
    paper_rank: 370
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: OGB
  datasets:
  - *id004
  - *id005
- benchmark: Heterophily Benchmark
  datasets:
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: Reddit
      dataset_slug: reddit
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
    - dataset: ogbn-arxiv
      dataset_slug: ogbn-arxiv
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Questions
      dataset_slug: questions
single_proposed_model: GraphAny
main_figure: /figures/2405.20445/main_figure.jpegoptim.jpg
---

