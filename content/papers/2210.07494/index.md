---
title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and Rethinking'
arxiv_id: '2210.07494'
source_url: ''
authors:
- name: Keyu Duan
  orcid: null
  s2_author_id: '108237152'
  s2_url: null
- name: Zirui Liu
  orcid: null
  s2_author_id: '47781070'
  s2_url: null
- name: Peihao Wang
  orcid: null
  s2_author_id: '2118952622'
  s2_url: null
- name: Wenqing Zheng
  orcid: null
  s2_author_id: '2152934619'
  s2_url: null
- name: Kaixiong Zhou
  orcid: null
  s2_author_id: '3364022'
  s2_url: null
- name: Tianlong Chen
  orcid: null
  s2_author_id: '2034263179'
  s2_url: null
- name: Xia Hu
  orcid: null
  s2_author_id: '2148950326'
  s2_url: null
- name: Zhangyang Wang
  orcid: null
  s2_author_id: '2969311'
  s2_url: null
published_date: Oct 14, 2022
published_date_iso: '2022-10-14'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Large-scale graph training is a notoriously challenging problem for graph
  neural networks (GNNs). Due to the nature of evolving graph structures into the
  training process, vanilla GNNs usually fail to scale up, limited by the GPU memory
  space. Up to now, though numerous scalable GNN architectures have been proposed,
  we still lack a comprehensive survey and fair benchmark of this reservoir to find
  the rationale for designing scalable GNNs. To this end, we first systematically
  formulate the representative methods of large-scale graph training into several
  branches and further establish a fair and consistent benchmark for them by a greedy
  hyperparameter searching. In addition, regarding efficiency, we theoretically evaluate
  the time and space complexity of various branches and empirically compare them w.r.t
  GPU memory usage, throughput, and convergence. Furthermore, We analyze the pros
  and cons for various branches of scalable GNNs and then present a new ensembling
  training manner, named EnGCN, to address the existing issues. Remarkably, our proposed
  method has achieved new state-of-the-art (SOTA) performance on large-scale datasets.
  Our code is available at.
codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
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
  evaluated: 1
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
  - model: EnGCN
    model_key: engcn
    model_plain: EnGCN
    value: 0.9714
    std: 0.0003
    paper_value: 0.9714
    paper_std: 0.0003
    metric: F1
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
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9714
    true_std: 0.0003
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9714
    sort_std: 0.0003
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.971
    std: 0.0
    paper_value: 0.971
    paper_std: 0.0
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
    table_ref: Table 3
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.971
    true_std: 0.0
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.971
    sort_std: 0.0
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.9562
    std: 0.0005
    paper_value: 0.9562
    paper_std: 0.0005
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
    table_ref: Table 3
    source_ref: zeng2019graphsaint
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.966
    at_pub_std: 0.001
    at_pub_source_arxiv: '2004.11198'
    at_pub_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    at_pub_source_date_iso: '2020-04-23'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.00979999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.97
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.013799999999999923
    has_value_note: false
    value_note: ''
    sort_value: 0.97
    sort_std: null
    global_rank: 5
    paper_rank: 59
    rank_delta: 54
    rank_delta_abs: 54
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    comparison_source_arxiv: '2004.11198'
    is_best: false
    is_std_outlier: false
  - model: SAGN
    model_key: sagn
    model_plain: SAGN
    value: 0.9648
    std: 0.0003
    paper_value: 0.9648
    paper_std: 0.0003
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
    table_ref: Table 3
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.969
    at_pub_std: 0.0
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-04-19'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.0041999999999999815
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.969
    true_std: 0.0
    value_gap_source_arxiv: '2104.09376'
    value_gap_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    value_gap_source_is_current_paper: false
    value_gap: 0.0041999999999999815
    has_value_note: false
    value_note: ''
    sort_value: 0.969
    sort_std: 0.0
    global_rank: 7
    paper_rank: 26
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    comparison_source_arxiv: '2104.09376'
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.9595
    std: 0.0002
    paper_value: 0.9595
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
    table_ref: Table 3
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.968
    at_pub_std: 0.0
    at_pub_source_arxiv: '2004.11198'
    at_pub_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    at_pub_source_date_iso: '2020-04-23'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.008499999999999952
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.968
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.008499999999999952
    has_value_note: false
    value_note: ''
    sort_value: 0.968
    sort_std: null
    global_rank: 10
    paper_rank: 47
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    comparison_source_arxiv: '2004.11198'
    is_best: false
    is_std_outlier: false
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.9673
    std: 0.0003
    paper_value: 0.9673
    paper_std: 0.0003
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
    table_ref: Table 3
    source_ref: zhang2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9673
    true_std: 0.0003
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9673
    sort_std: 0.0003
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.965
    std: 0.0003
    paper_value: 0.965
    paper_std: 0.0003
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
    table_ref: Table 3
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.966
    at_pub_std: null
    at_pub_source_arxiv: '2105.04528'
    at_pub_source_title: Accelerating Large Scale Real-Time GNN Inference using Channel
      Pruning
    at_pub_source_date_iso: '2021-05-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
    global_rank: 19
    paper_rank: 25
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    comparison_source_arxiv: '2105.04528'
    is_best: false
    is_std_outlier: false
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    value: 0.9605
    std: 0.0
    paper_value: 0.9605
    paper_std: 0.0
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
    table_ref: Table 3
    source_ref: sun2019adagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.9539
    at_pub_std: 0.0013
    at_pub_source_arxiv: '1908.05081'
    at_pub_source_title: 'AdaGCN: Adaboosting Graph Convolutional Networks into Deep
      Models'
    at_pub_source_date_iso: '2019-08-14'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.00660000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9605
    true_std: 0.0
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9605
    sort_std: 0.0
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'AdaGCN: Adaboosting Graph Convolutional Networks into
      Deep Models'
    comparison_source_arxiv: '1908.05081'
    is_best: false
    is_std_outlier: false
  - model: ClusterGCN
    model_key: clustergcn
    model_plain: ClusterGCN
    value: 0.9568
    std: 0.0003
    paper_value: 0.9568
    paper_std: 0.0003
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
    table_ref: Table 3
    source_ref: chiang2019cluster
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.957
    at_pub_std: 0.0
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.957
    true_std: 0.0
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.957
    sort_std: 0.0
    global_rank: 56
    paper_rank: 59
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: C&S
    model_key: c&s
    model_plain: C&S
    value: 0.9533
    std: 0.0008
    paper_value: 0.9533
    paper_std: 0.0008
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
    table_ref: Table 3
    source_ref: huang2020combining
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9533
    true_std: 0.0008
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9533
    sort_std: 0.0008
    global_rank: 67
    paper_rank: 67
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
    value: 0.9351
    std: 0.0004
    paper_value: 0.9351
    paper_std: 0.0004
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
    table_ref: Table 3
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.949
    at_pub_std: null
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.013899999999999912
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: 0.0
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: 0.013899999999999912
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0
    global_rank: 85
    paper_rank: 118
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Deep Learning on Graphs: A Survey'
    comparison_source_arxiv: '1812.04202'
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.795
    std: 0.0122
    paper_value: 0.795
    paper_std: 0.0122
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
    table_ref: Table 3
    source_ref: chen2018fastgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.937
    at_pub_std: null
    at_pub_source_arxiv: '1801.10247'
    at_pub_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    at_pub_source_date_iso: '2018-01-30'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.14200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.14200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
    global_rank: 113
    paper_rank: 150
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    comparison_source_arxiv: '1801.10247'
    is_best: false
    is_std_outlier: true
  - model: LADIES
    model_key: ladies
    model_plain: LADIES
    value: 0.8696
    std: 0.0037
    paper_value: 0.8696
    paper_std: 0.0037
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
    table_ref: Table 3
    source_ref: zou2019layer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test F1 on Reddit dataset
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.932
    at_pub_std: 0.001
    at_pub_source_arxiv: '2103.05872'
    at_pub_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.06240000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.932
    true_std: 0.001
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.06240000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.001
    global_rank: 125
    paper_rank: 146
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    comparison_source_arxiv: '2103.05872'
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
- &id002
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
  - model: EnGCN
    model_key: engcn
    model_plain: EnGCN
    value: 0.8799
    std: 0.0004
    paper_value: 0.8799
    paper_std: 0.0004
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
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8799
    true_std: 0.0004
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8799
    sort_std: 0.0004
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
  - model: SAGN
    model_key: sagn
    model_plain: SAGN
    value: 0.8121
    std: 0.0007
    paper_value: 0.8121
    paper_std: 0.0007
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
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8736
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2210.14709'
    at_pub_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    at_pub_source_date_iso: 2022-10
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.0615
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: false
    value_gap: 0.0615
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 5
    paper_rank: 113
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    comparison_source_arxiv: '2210.14709'
    is_best: false
    is_std_outlier: false
  - model: GIANT-XRT+SAGN+MCR+C&S
    model_key: giant-xrt+sagn+mcr+c&s
    model_plain: GIANT-XRT+SAGN+MCR+C&S
    value: 0.8673
    std: 0.0008
    paper_value: 0.8673
    paper_std: 0.0008
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
    source_ref: zhang2021improving
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8673
    true_std: 0.0008
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8673
    sort_std: 0.0008
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
  - model: C&S
    model_key: c&s
    model_plain: C&S
    value: 0.8511
    std: 0.0007
    paper_value: 0.8511
    paper_std: 0.0007
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
    source_ref: huang2020combining
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7711
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2206.03638'
    at_pub_source_title: Alternately Optimized Graph Neural Networks
    at_pub_source_date_iso: '2022-06-08'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07999999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8511
    true_std: 0.0007
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8511
    sort_std: 0.0007
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Alternately Optimized Graph Neural Networks
    comparison_source_arxiv: '2206.03638'
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.8428
    std: 0.0014
    paper_value: 0.8428
    paper_std: 0.0014
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
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8501
    at_pub_std: 0.001
    at_pub_source_arxiv: '2111.00064'
    at_pub_source_title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood
      Prediction
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.007299999999999973
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8501
    true_std: 0.001
    value_gap_source_arxiv: '2111.00064'
    value_gap_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.007299999999999973
    has_value_note: false
    value_note: ''
    sort_value: 0.8501
    sort_std: 0.001
    global_rank: 30
    paper_rank: 41
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    comparison_source_arxiv: '2111.00064'
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.7536
    std: 0.0034
    paper_value: 0.7536
    paper_std: 0.0034
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
    source_ref: zeng2019graphsaint
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8383
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2111.00064'
    at_pub_source_title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood
      Prediction
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.0847
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8383
    true_std: 0.0014
    value_gap_source_arxiv: '2111.00064'
    value_gap_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0847
    has_value_note: false
    value_note: ''
    sort_value: 0.8383
    sort_std: 0.0014
    global_rank: 51
    paper_rank: 257
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    comparison_source_arxiv: '2111.00064'
    is_best: false
    is_std_outlier: false
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.8376
    std: 0.0019
    paper_value: 0.8376
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
    table_ref: Table 3
    source_ref: zhang2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8354
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2108.10097'
    at_pub_source_title: Graph Attention MLP with Reliable Label Utilization
    at_pub_source_date_iso: '2021-08-23'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0021999999999999797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8376
    true_std: 0.0019
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8376
    sort_std: 0.0019
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.7685
    std: 0.0056
    paper_value: 0.7685
    paper_std: 0.0056
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
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.831
    at_pub_std: 0.008
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.0625
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.008
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.0625
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.008
    global_rank: 67
    paper_rank: 236
    rank_delta: 169
    rank_delta_abs: 169
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8061
    std: 0.0016
    paper_value: 0.8061
    paper_std: 0.0016
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.801
    at_pub_std: null
    at_pub_source_arxiv: '2111.06483'
    at_pub_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    at_pub_source_date_iso: '2021-11-11'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.005099999999999993
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8287
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.022599999999999953
    has_value_note: false
    value_note: ''
    sort_value: 0.8287
    sort_std: null
    global_rank: 74
    paper_rank: 129
    rank_delta: 55
    rank_delta_abs: 55
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    comparison_source_arxiv: '2111.06483'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.6748
    std: 0.0011
    paper_value: 0.6748
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
    table_ref: Table 3
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.822
    at_pub_std: 0.009
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.1472
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.822
    true_std: 0.009
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.1472
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.009
    global_rank: 87
    paper_rank: 347
    rank_delta: 260
    rank_delta_abs: 260
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: ClusterGCN
    model_key: clustergcn
    model_plain: ClusterGCN
    value: 0.7862
    std: 0.0061
    paper_value: 0.7862
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
    table_ref: Table 3
    source_ref: chiang2019cluster
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7897
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2004.11198'
    at_pub_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    at_pub_source_date_iso: '2020-04-23'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-04-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0034999999999999476
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7897
    true_std: 0.0033
    value_gap_source_arxiv: '2004.11198'
    value_gap_source_title: 'SIGN: Scalable Inception Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.0034999999999999476
    has_value_note: false
    value_note: ''
    sort_value: 0.7897
    sort_std: 0.0033
    global_rank: 194
    paper_rank: 209
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    value: 0.7641
    std: 0.0
    paper_value: 0.7641
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
    table_ref: Table 3
    source_ref: sun2019adagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-14'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7641
    true_std: 0.0
    value_gap_source_arxiv: '2210.07494'
    value_gap_source_title: 'A Comprehensive Study on Large-Scale Graph Training:
      Benchmarking and Rethinking'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7641
    sort_std: 0.0
    global_rank: 242
    paper_rank: 242
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LADIES
    model_key: ladies
    model_plain: LADIES
    value: 0.7531
    std: 0.0056
    paper_value: 0.7531
    paper_std: 0.0056
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
    source_ref: zou2019layer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-18'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7531
    true_std: 0.0056
    value_gap_source_arxiv: '2306.10466'
    value_gap_source_title: 'Graph Ladling: Shockingly Simple Parallel GNN Training
      without Intermediate Communication'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7531
    sort_std: 0.0056
    global_rank: 260
    paper_rank: 260
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.7346
    std: 0.002
    paper_value: 0.7346
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
    source_ref: chen2018fastgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: node classification on ogbn-products test split
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-18'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7346
    true_std: 0.002
    value_gap_source_arxiv: '2306.10466'
    value_gap_source_title: 'Graph Ladling: Shockingly Simple Parallel GNN Training
      without Intermediate Communication'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7346
    sort_std: 0.002
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
- benchmark: OGB
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
main_figure: /figures/2210.07494/main_figure.jpegoptim.jpg
---

