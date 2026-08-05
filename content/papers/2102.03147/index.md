---
title: Learning Conjoint Attentions for Graph Neural Nets
arxiv_id: '2102.03147'
source_url: ''
authors:
- name: Tiantian He
  orcid: null
  s2_author_id: '2834580'
  s2_url: null
- name: Y. Ong
  orcid: null
  s2_author_id: '144848119'
  s2_url: null
- name: Lu Bai
  orcid: null
  s2_author_id: '145515614'
  s2_url: null
published_date: Feb 5, 2021
published_date_iso: '2021-02-05'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: In this paper, we present Conjoint Attentions (CAs), a class of novel learning-to-attend
  strategies for graph neural networks (GNNs). Besides considering the layer-wise
  node features propagated within the GNN, CAs can additionally incorporate various
  structural interventions, such as node cluster embedding, and higher-order structural
  correlations that can be learned outside of GNN, when computing attention scores.
  The node features that are regarded as significant by the conjoint criteria are
  therefore more likely to be propagated in the GNN. Given the novel Conjoint Attention
  strategies, we then propose Graph conjoint attention networks (CATs) that can learn
  representations embedded with significant latent features deemed by the Conjoint
  Attentions. Besides, we theoretically validate the discriminative capacity of CATs.
  CATs utilizing the proposed conjoint attention strategies have been extensively
  tested in well-established benchmarking datasets and comprehensively compared with
  state-of-the-art baselines. The obtained notable performance demonstrates the effectiveness
  of the proposed conjoint attentions.
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
- OGB
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
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
    value: 0.8142
    std: 0.0019
    paper_value: 0.8142
    paper_std: 0.0019
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.8717
    at_pub_std: 0.0058
    at_pub_source_arxiv: '1711.08920'
    at_pub_source_title: 'SplineCNN: Fast Geometric Deep Learning with Continuous
      B-Spline Kernels'
    at_pub_source_date_iso: '2017-11-24'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.057499999999999996
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
    value_gap: 0.08619999999999994
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
    comparison_source_title: 'SplineCNN: Fast Geometric Deep Learning with Continuous
      B-Spline Kernels'
    comparison_source_arxiv: '1711.08920'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.828
    std: 0.0032
    paper_value: 0.828
    paper_std: 0.0032
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.049000000000000044
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
    value_gap: 0.06240000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 552
    rank_delta: 483
    rank_delta_abs: 483
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
    value: 0.8384
    std: 0.0061
    paper_value: 0.8384
    paper_std: 0.0061
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.05059999999999998
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
    value_gap: 0.05130000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 419
    rank_delta: 347
    rank_delta_abs: 347
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8112
    std: 0.0041
    paper_value: 0.8112
    paper_std: 0.0041
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.841
    at_pub_std: 0.016
    at_pub_source_arxiv: '2006.03814'
    at_pub_source_title: The Impact of Global Structural Information in Graph Neural
      Networks Applications
    at_pub_source_date_iso: '2020-06-06'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.029799999999999938
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8889
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07769999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8889
    sort_std: null
    global_rank: 79
    paper_rank: 724
    rank_delta: 645
    rank_delta_abs: 645
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: The Impact of Global Structural Information in Graph
      Neural Networks Applications
    comparison_source_arxiv: '2006.03814'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.7834
    std: 0.0002
    paper_value: 0.7834
    paper_std: 0.0002
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.887
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.10360000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.887
    true_std: 0.0
    value_gap_source_arxiv: '2009.09232'
    value_gap_source_title: Learned Low Precision Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10360000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.0
    global_rank: 88
    paper_rank: 824
    rank_delta: 736
    rank_delta_abs: 736
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.819
    std: 0.0001
    paper_value: 0.819
    paper_std: 0.0001
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.81
    at_pub_std: 0.0
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.008999999999999897
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8797
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06070000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: null
    global_rank: 138
    paper_rank: 655
    rank_delta: 517
    rank_delta_abs: 517
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Deep Learning on Graphs: A Survey'
    comparison_source_arxiv: '1812.04202'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8158
    std: 0.0062
    paper_value: 0.8158
    paper_std: 0.0062
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.866
    true_std: 0.0091
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.05020000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.866
    sort_std: 0.0091
    global_rank: 227
    paper_rank: 694
    rank_delta: 467
    rank_delta_abs: 467
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-E-MF
    model_key: cat-e-mf
    model_plain: CAT-E-MF
    value: 0.8556
    std: 0.0019
    paper_value: 0.8556
    paper_std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings (MF)
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8556
    true_std: 0.0019
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8556
    sort_std: 0.0019
    global_rank: 285
    paper_rank: 285
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-I-SC
    model_key: cat-i-sc
    model_plain: CAT-I-SC
    value: 0.855
    std: 0.0022
    paper_value: 0.855
    paper_std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., self-representation coefficients (SC)
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.855
    true_std: 0.0022
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.855
    sort_std: 0.0022
    global_rank: 288
    paper_rank: 288
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-E-SC
    model_key: cat-e-sc
    model_plain: CAT-E-SC
    value: 0.854
    std: 0.0036
    paper_value: 0.854
    paper_std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., self-representation coefficients (SC)
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.0036
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.0036
    global_rank: 295
    paper_rank: 295
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-I-MF
    model_key: cat-i-mf
    model_plain: CAT-I-MF
    value: 0.8538
    std: 0.0016
    paper_value: 0.8538
    paper_std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings (MF)
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8538
    true_std: 0.0016
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8538
    sort_std: 0.0016
    global_rank: 300
    paper_rank: 300
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-I-FS
    model_key: cat-i-fs
    model_plain: CAT-I-FS
    value: 0.8486
    std: 0.003
    paper_value: 0.8486
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: using input feature similarity
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8486
    true_std: 0.003
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8486
    sort_std: 0.003
    global_rank: 335
    paper_rank: 335
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-NetMF
    model_key: gat-netmf
    model_plain: GAT-NetMF
    value: 0.8444
    std: 0.0019
    paper_value: 0.8444
    paper_std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Matrix factorization-based network embedding (NetMF)
      used to learn structural node representations and concatenate them with X
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8444
    true_std: 0.0019
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8444
    sort_std: 0.0019
    global_rank: 358
    paper_rank: 358
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-E-FS
    model_key: cat-e-fs
    model_plain: CAT-E-FS
    value: 0.8415
    std: 0.0023
    paper_value: 0.8415
    paper_std: 0.0023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: using input feature similarity
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8415
    true_std: 0.0023
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8415
    sort_std: 0.0023
    global_rank: 389
    paper_rank: 389
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-k-Lap
    model_key: gat-k-lap
    model_plain: GAT-k-Lap
    value: 0.841
    std: 0.0024
    paper_value: 0.841
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
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: k-eigenvectors of graph Laplacian (k-Lap) used to learn
      structural node representations and concatenate them with X
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.841
    true_std: 0.0024
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.841
    sort_std: 0.0024
    global_rank: 398
    paper_rank: 398
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-Deep
    model_key: gat-deep
    model_plain: GAT-Deep
    value: 0.8368
    std: 0.0067
    paper_value: 0.8368
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
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Deepwalk used to learn structural node representations
      and concatenate them with X
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8368
    true_std: 0.0067
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8368
    sort_std: 0.0067
    global_rank: 443
    paper_rank: 443
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARMA
    model_key: arma
    model_plain: ARMA
    value: 0.8006
    std: 0.0057
    paper_value: 0.8006
    paper_std: 0.0057
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
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.833
    at_pub_std: null
    at_pub_source_arxiv: '2003.07450'
    at_pub_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    at_pub_source_date_iso: '2020-03-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.032399999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.834
    true_std: null
    value_gap_source_arxiv: '2209.15454'
    value_gap_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    value_gap_source_is_current_paper: false
    value_gap: 0.033399999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.834
    sort_std: null
    global_rank: 492
    paper_rank: 774
    rank_delta: 282
    rank_delta_abs: 282
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    comparison_source_arxiv: '2003.07450'
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.8196
    std: 0.005
    paper_value: 0.8196
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 labeled nodes per class for training, 1000
      nodes for testing.'
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.817
    at_pub_std: 0.005
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2021-06-21'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.0026000000000000467
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.007
    value_gap_source_arxiv: '2106.10934'
    value_gap_source_title: 'GRAND: Graph Neural Diffusion'
    value_gap_source_is_current_paper: false
    value_gap: 0.0023999999999999577
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.007
    global_rank: 626
    paper_rank: 654
    rank_delta: 28
    rank_delta_abs: 28
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
- &id002
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
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
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7966
    std: 0.0039
    paper_value: 0.7966
    paper_std: 0.0039
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10040000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.133
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 506
    rank_delta: 485
    rank_delta_abs: 485
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
    value: 0.815
    std: 0.0047
    paper_value: 0.815
    paper_std: 0.0047
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.08200000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.10830000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 361
    rank_delta: 338
    rank_delta_abs: 338
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.7988
    std: 0.0001
    paper_value: 0.7988
    paper_std: 0.0001
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.916
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.11720000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.916
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.11720000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: null
    global_rank: 27
    paper_rank: 490
    rank_delta: 463
    rank_delta_abs: 463
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8242
    std: 0.0004
    paper_value: 0.8242
    paper_std: 0.0004
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.79
    at_pub_std: 0.001
    at_pub_source_arxiv: '2010.15421'
    at_pub_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    at_pub_source_date_iso: '2020-10-29'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03420000000000001
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.0055
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.05899999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.0055
    global_rank: 159
    paper_rank: 332
    rank_delta: 173
    rank_delta_abs: 173
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    comparison_source_arxiv: '2010.15421'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8076
    std: 0.0033
    paper_value: 0.8076
    paper_std: 0.0033
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.871
    at_pub_std: null
    at_pub_source_arxiv: '2010.00238'
    at_pub_source_title: Multi-grained Semantics-aware Graph Neural Networks
    at_pub_source_date_iso: '2020-10-01'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-08-21'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06340000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: null
    value_gap_source_arxiv: '2308.10737'
    value_gap_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07340000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: null
    global_rank: 176
    paper_rank: 411
    rank_delta: 235
    rank_delta_abs: 235
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-grained Semantics-aware Graph Neural Networks
    comparison_source_arxiv: '2010.00238'
    is_best: false
    is_std_outlier: false
  - model: CAT-I-SC
    model_key: cat-i-sc
    model_plain: CAT-I-SC
    value: 0.8428
    std: 0.002
    paper_value: 0.8428
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8428
    true_std: 0.002
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8428
    sort_std: 0.002
    global_rank: 287
    paper_rank: 287
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-E-SC
    model_key: cat-e-sc
    model_plain: CAT-E-SC
    value: 0.8402
    std: 0.0024
    paper_value: 0.8402
    paper_std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8402
    true_std: 0.0024
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8402
    sort_std: 0.0024
    global_rank: 292
    paper_rank: 292
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-I-MF
    model_key: cat-i-mf
    model_plain: CAT-I-MF
    value: 0.839
    std: 0.0024
    paper_value: 0.839
    paper_std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.0024
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.0024
    global_rank: 297
    paper_rank: 297
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAT-E-MF
    model_key: cat-e-mf
    model_plain: CAT-E-MF
    value: 0.836
    std: 0.0017
    paper_value: 0.836
    paper_std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: incorporation of purposeful interventions brought by
      factors external to the neural net, e.g., node cluster embeddings
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.0017
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0017
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
  - model: GAT-k-Lap
    model_key: gat-k-lap
    model_plain: GAT-k-Lap
    value: 0.8256
    std: 0.003
    paper_value: 0.8256
    paper_std: 0.003
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8256
    true_std: 0.003
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8256
    sort_std: 0.003
    global_rank: 331
    paper_rank: 331
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-NetMF
    model_key: gat-netmf
    model_plain: GAT-NetMF
    value: 0.819
    std: 0.0033
    paper_value: 0.819
    paper_std: 0.0033
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-05'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.819
    true_std: 0.0033
    value_gap_source_arxiv: '2102.03147'
    value_gap_source_title: Learning Conjoint Attentions for Graph Neural Nets
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.0033
    global_rank: 348
    paper_rank: 348
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
    value: 0.7978
    std: 0.0033
    paper_value: 0.7978
    paper_std: 0.0033
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
    protocol_note: Semi-supervised node classification on Planetoid split (20 labeled
      nodes per class, 1000 test nodes).
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.7881
    at_pub_std: 0.004
    at_pub_source_arxiv: '1710.10370'
    at_pub_source_title: Topology Adaptive Graph Convolutional Networks
    at_pub_source_date_iso: '2017-10-28'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.009699999999999931
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8006
    true_std: 0.0055
    value_gap_source_arxiv: '2210.07715'
    value_gap_source_title: 'Not All Neighbors Are Worth Attending to: Graph Selective
      Attention Networks for Semi-supervised Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0028000000000000247
    has_value_note: false
    value_note: ''
    sort_value: 0.8006
    sort_std: 0.0055
    global_rank: 470
    paper_rank: 502
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Topology Adaptive Graph Convolutional Networks
    comparison_source_arxiv: '1710.10370'
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
- &id003
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.6402
    std: 0.0018
    paper_value: 0.6402
    paper_std: 0.0018
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
    protocol_note: node classification task using the official OGB-Arxiv split (papers
      up to 2017 for training, 2018/2019 for test/val)
    date: Feb 5, 2021
    date_display: Feb 2021
    date_iso: '2021-02-05'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.7176
    at_pub_std: null
    at_pub_source_arxiv: '2010.00238'
    at_pub_source_title: Multi-grained Semantics-aware Graph Neural Networks
    at_pub_source_date_iso: '2020-10-01'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-10-01'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.07740000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7176
    true_std: null
    value_gap_source_arxiv: '2010.00238'
    value_gap_source_title: Multi-grained Semantics-aware Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07740000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7176
    sort_std: null
    global_rank: 62
    paper_rank: 118
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-grained Semantics-aware Graph Neural Networks
    comparison_source_arxiv: '2010.00238'
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
- benchmark: OGB
  datasets:
  - *id003
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
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-arxiv
      dataset_slug: ogbn-arxiv
main_figure: /figures/2102.03147/main_figure.jpegoptim.jpg
---

