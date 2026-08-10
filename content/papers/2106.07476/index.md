---
title: Training Graph Neural Networks with 1000 Layers
arxiv_id: '2106.07476'
source_url: ''
authors:
- name: Guohao Li
  orcid: null
  s2_author_id: '1669997484'
  s2_url: null
- name: Matthias Müller
  orcid: null
  s2_author_id: '1391027880'
  s2_url: null
- name: Bernard Ghanem
  orcid: null
  s2_author_id: '2931652'
  s2_url: null
- name: V. Koltun
  orcid: null
  s2_author_id: '145231047'
  s2_url: null
published_date: Jun 14, 2021
published_date_iso: '2021-06-14'
published_venue: ICML 2021
published_conference: ICML 2021
published_conference_short: ICML
published_conference_slug: icml
abstract: Deep graph neural networks (GNNs) have achieved excellent results on various
  tasks on increasingly large graph datasets with millions of nodes and edges. However,
  memory complexity has become a major obstacle when training deep GNNs for practical
  applications due to the immense number of nodes, edges, and intermediate activations.
  To improve the scalability of GNNs, prior works propose smart graph sampling or
  partitioning strategies to train GNNs with a smaller set of nodes or sub-graphs.
  In this work, we study reversible connections, group convolutions, weight tying,
  and equilibrium models to advance the memory and parameter efficiency of GNNs. We
  find that reversible connections in combination with deep network architectures
  enable the training of overparameterized GNNs that significantly outperform existing
  methods on multiple datasets. Our models RevGNN-Deep (1001 layers with 80 channels
  each) and RevGNN-Wide (448 layers with 224 channels each) were both trained on a
  single commodity GPU and achieve an ROC-AUC of 87.74 ± 0.13 and 88.24 ± 0.15 on
  the ogbn-proteins dataset. To the best of our knowledge, RevGNN-Deep is the deepest
  GNN in the literature by one order of magnitude.
codebase_url: https://github.com/ShunliRen/dgl
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- RevGNN-Deep
- RevGNN
mrr: 0.125
adjusted_mrr: 0.0417
mrr_dataset_count: 1
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
  dataset: ogbn-proteins
  rows:
  - model: LD
    model_key: ld
    model_plain: LD
    value: 0.8942
    std: 0.0007
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8942
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: X_WO/LD
    model_key: x_wo/ld
    model_plain: X_WO/LD
    value: 0.8915
    std: 0.0012
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8915
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoG
    model_key: mog
    model_plain: MoG
    value: 0.8904
    std: 0.0072
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.14260'
    title: Graph Sparsification via Mixture of Graphs
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/yanweiyue/MoG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8904
    sort_std: 0.0072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RevGNN
    model_key: revgnn
    model_plain: RevGNN
    value: 0.8824
    std: 0.0015
    paper_value: 0.8824
    paper_std: 0.0015
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8824
    true_std: 0.0015
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8824
    sort_std: 0.0015
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
  - model: RevGNN-Deep
    model_key: revgnn-deep
    model_plain: RevGNN-Deep
    value: 0.8774
    std: 0.0013
    paper_value: 0.8774
    paper_std: 0.0013
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 20.03
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
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8774
    true_std: 0.0013
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8774
    sort_std: 0.0013
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
  - model: UniMP+CEF
    model_key: unimp+cef
    model_plain: UniMP+CEF
    value: 0.8691
    std: 0.0018
    paper_value: 0.8691
    paper_std: 0.0018
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1.96
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Shi et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8691
    true_std: 0.0018
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8691
    sort_std: 0.0018
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8682
    std: 0.0021
    paper_value: 0.8682
    paper_std: 0.0021
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.48
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Veličković et al. 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8682
    true_std: 0.0021
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8682
    sort_std: 0.0021
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniMP
    model_key: unimp
    model_plain: UniMP
    value: 0.8642
    std: 0.0008
    paper_value: 0.8642
    paper_std: 0.0008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1.91
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Shi et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: 0.8642
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2009.03509'
    at_pub_source_title: 'Masked Label Prediction: Unified Message Passing Model for
      Semi-Supervised Classification'
    at_pub_source_date_iso: '2020-09-08'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8642
    true_std: 0.0008
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8642
    sort_std: 0.0008
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeeperGCN
    model_key: deepergcn
    model_plain: DeeperGCN
    value: 0.8616
    std: 0.0016
    paper_value: 0.8616
    paper_std: 0.0016
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.37
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Li et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: 0.858
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2009.03509'
    at_pub_source_title: 'Masked Label Prediction: Unified Message Passing Model for
      Semi-Supervised Classification'
    at_pub_source_date_iso: '2020-09-08'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2021-06-14'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.0036000000000000476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8616
    true_std: 0.0016
    value_gap_source_arxiv: '2106.07476'
    value_gap_source_title: Training Graph Neural Networks with 1000 Layers
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8616
    sort_std: 0.0016
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Masked Label Prediction: Unified Message Passing Model
      for Semi-Supervised Classification'
    comparison_source_arxiv: '2009.03509'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7768
    std: 0.002
    paper_value: 0.7768
    paper_std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.193
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Hamilton et al. 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.843
    true_std: null
    value_gap_source_arxiv: '2409.05573'
    value_gap_source_title: Learning to Model Graph Structural Information on MLPs
      via Graph Structure Self-Contrasting
    value_gap_source_is_current_paper: false
    value_gap: 0.06619999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.843
    sort_std: null
    global_rank: 17
    paper_rank: 43
    rank_delta: 26
    rank_delta_abs: 26
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
    value: 0.7251
    std: 0.0035
    paper_value: 0.7251
    paper_std: 0.0035
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0969
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Kipf et al. 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC-AUC on the standard ogbn-proteins split using random partitioning
      (10 train/5 test) as described in the text.
    date: Jun 14, 2021
    date_display: Jun 2021
    date_iso: '2021-06-14'
    published_venue: ICML 2021
    published_conference: ICML 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.832
    true_std: null
    value_gap_source_arxiv: '2409.05573'
    value_gap_source_title: Learning to Model Graph Structural Information on MLPs
      via Graph Structure Self-Contrasting
    value_gap_source_is_current_paper: false
    value_gap: 0.1069
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: null
    global_rank: 18
    paper_rank: 57
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7677
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_display: Oct 2021
    date_iso: '2021-10-14'
    venue: null
    codebase_url: https://github.com/yuehaowang/SoGCN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 49
    sort_value: 0.7677
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
    - dataset: ogbn-proteins
      dataset_slug: ogbn-proteins
main_figure: /figures/2106.07476/main_figure.jpegoptim.jpg
---

