---
title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
arxiv_id: '2110.03753'
source_url: ''
authors:
- name: Lingxiao Zhao
  orcid: null
  s2_author_id: '21613538'
  s2_url: null
- name: Wei Jin
  orcid: null
  s2_author_id: '144767914'
  s2_url: null
- name: L. Akoglu
  orcid: null
  s2_author_id: '3255268'
  s2_url: null
- name: Neil Shah
  orcid: null
  s2_author_id: '145474474'
  s2_url: null
published_date: Oct 7, 2021
published_date_iso: '2021-10-07'
published_venue: ICLR 2021
published_conference: ICLR 2021
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Message Passing Neural Networks (MPNNs) are a common type of Graph Neural
  Network (GNN), in which each node''s representation is computed recursively by aggregating
  representations (messages) from its immediate neighbors akin to a star-shaped pattern.
  MPNNs are appealing for being efficient and scalable, how-ever their expressiveness
  is upper-bounded by the 1st-order Weisfeiler-Lehman isomorphism test (1-WL). In
  response, prior works propose highly expressive models at the cost of scalability
  and sometimes generalization performance. Our work stands between these two regimes:
  we introduce a general framework to uplift any MPNN to be more expressive, with
  limited scalability overhead and greatly improved practical performance. We achieve
  this by extending local aggregation in MPNNs from star patterns to general subgraph
  patterns (e.g.,k-egonets):in our framework, each node representation is computed
  as the encoding of a surrounding induced subgraph rather than encoding of immediate
  neighbors only (i.e. a star). We choose the subgraph encoder to be a GNN (mainly
  MPNNs, considering scalability) to design a general framework that serves as a wrapper
  to up-lift any GNN. We call our proposed method GNN-AK(GNN As Kernel), as the framework
  resembles a convolutional neural network by replacing the kernel with GNNs. Theoretically,
  we show that our framework is strictly more powerful than 1&2-WL, and is not less
  powerful than 3-WL. We also design subgraph sampling strategies which greatly reduce
  memory footprint and improve speed while maintaining performance. Our method sets
  new state-of-the-art performance by large margins for several well-known graph ML
  tasks; specifically, 0.08 MAE on ZINC,74.79% and 86.887% accuracy on CIFAR10 and
  PATTERN respectively.'
codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
- GNNBenchmark
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 4
  total: 11
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id005
  dataset: CIFAR10
  rows:
  - model: RandAlign
    model_key: randalign
    model_plain: RandAlign
    value: 0.7942
    std: 0.00072
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: Apr 15, 2024
    date_display: Apr 2024
    date_iso: '2024-04-15'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7942
    sort_std: 0.00072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: differential encoding
    model_key: differential encoding
    model_plain: differential encoding
    value: 0.79067
    std: 0.00269
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    venue: IEEE Transactions on Big Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.79067
    sort_std: 0.00269
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPGT
    model_key: ppgt
    model_plain: PPGT
    value: 0.7856
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7856
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA*-AK+-S
    model_key: pna*-ak+-s
    model_plain: PNA*-AK+-S
    value: 0.7479
    std: 0.0018
    paper_value: 0.7479
    paper_std: 0.0018
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7479
    true_std: 0.0018
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7479
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA*
    model_key: pna
    model_plain: PNA*
    value: 0.7311
    std: 0.0011
    paper_value: 0.7311
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7311
    true_std: 0.0011
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: 0.0011
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
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.7284
    std: 0.0042
    paper_value: 0.7284
    paper_std: 0.0042
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
    source_ref: ICML 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7284
    true_std: 0.0042
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7284
    sort_std: 0.0042
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-AK+
    model_key: gcn-ak+
    model_plain: GCN-AK+
    value: 0.727
    std: 0.0029
    paper_value: 0.727
    paper_std: 0.0029
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.727
    true_std: 0.0029
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.727
    sort_std: 0.0029
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.7219
    std: 0.0013
    paper_value: 0.7219
    paper_std: 0.0013
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7239
    true_std: 0.0038
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.7239
    sort_std: 0.0038
    global_rank: 43
    paper_rank: 49
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-AK+-S
    model_key: gin-ak+-s
    model_plain: GIN-AK+-S
    value: 0.7239
    std: 0.0038
    paper_value: 0.7239
    paper_std: 0.0038
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7239
    true_std: 0.0038
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7239
    sort_std: 0.0038
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-AK+-S
    model_key: gcn-ak+-s
    model_plain: GCN-AK+-S
    value: 0.7193
    std: 0.0047
    paper_value: 0.7193
    paper_std: 0.0047
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7193
    true_std: 0.0047
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7193
    sort_std: 0.0047
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.6937
    std: 0.0048
    paper_value: 0.6937
    paper_std: 0.0048
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
    source_ref: Dwivedi et al. 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.7133
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.019600000000000062
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7133
    true_std: 0.0039
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.019600000000000062
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: 0.0039
    global_rank: 61
    paper_rank: 75
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.6731
    std: 0.0031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 93
    sort_value: 0.6731
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.669
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2107.04755'
    title: 'Beyond Low-pass Filtering: Graph Convolutional Networks with Automatic
      Filtering'
    date: Jul 10, 2021
    date_display: Jul 2021
    date_iso: '2021-07-10'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/nnzhan/AutoGCN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 95
    sort_value: 0.669
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNN-AK+
    model_key: gnn-ak+
    model_plain: GNN-AK+
    value: 0.5982
    std: 0.0033
    paper_value: 0.5982
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
    source_ref: Xu et al. 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5982
    true_std: 0.0033
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5982
    sort_std: 0.0033
    global_rank: 126
    paper_rank: 126
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
    value: 0.5839
    std: 0.0073
    paper_value: 0.5839
    paper_std: 0.0073
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
    source_ref: Kipf & Welling 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on CIFAR10 test split
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.5571
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.026799999999999935
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5839
    true_std: 0.0073
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5839
    sort_std: 0.0073
    global_rank: 128
    paper_rank: 128
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5634
    std: 0.00181
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 130
    sort_value: 0.5634
    sort_std: 0.00181
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
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
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.927
    std: 0.061
    paper_value: 0.927
    paper_std: 0.061
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
    table_ref: Table 9
    source_ref: bodnar2021b
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.927
    at_pub_std: 0.061
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.944
    true_std: 0.037
    value_gap_source_arxiv: '2306.03561'
    value_gap_source_title: 'CIN++: Enhancing Topological Message Passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.016999999999999904
    has_value_note: false
    value_note: ''
    sort_value: 0.944
    sort_std: 0.037
    global_rank: 28
    paper_rank: 53
    rank_delta: 25
    rank_delta_abs: 25
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
    value: 0.933
    std: 0.029
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.00911'
    title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    date: Dec 2, 2021
    date_display: Dec 2021
    date_iso: '2021-12-02'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 43
    sort_value: 0.933
    sort_std: 0.029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSN
    model_key: gsn
    model_plain: GSN
    value: 0.922
    std: 0.075
    paper_value: 0.922
    paper_std: 0.075
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.922
    at_pub_std: 0.075
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.922
    true_std: 0.075
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.075
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GNN-AK+
    model_key: gnn-ak+
    model_plain: GNN-AK+
    value: 0.913
    std: 0.07
    paper_value: 0.913
    paper_std: 0.07
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.913
    true_std: 0.07
    value_gap_source_arxiv: '2404.13344'
    value_gap_source_title: 'GRANOLA: Adaptive Normalization for Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.07
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPGNs
    model_key: ppgns
    model_plain: PPGNs
    value: 0.906
    std: 0.087
    paper_value: 0.906
    paper_std: 0.087
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.906
    at_pub_std: 0.087
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.906
    true_std: 0.087
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.906
    sort_std: 0.087
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL kernel
    model_key: wl kernel
    model_plain: WL kernel
    value: 0.904
    std: 0.057
    paper_value: 0.904
    paper_std: 0.057
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '2005.01214'
    at_pub_source_title: Graph Homomorphism Convolution
    at_pub_source_date_iso: '2020-05-03'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2024-09-27'
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
    true_std: 0.057
    value_gap_source_arxiv: '2409.19117'
    value_gap_source_title: 'Range-aware Positional Encoding via High-order Pretraining:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 176
    paper_rank: 176
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Natural GN
    model_key: natural gn
    model_plain: Natural GN
    value: 0.894
    std: 0.016
    paper_value: 0.894
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.894
    at_pub_std: 0.016
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.016
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.016
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.858
    std: 0.018
    paper_value: 0.858
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.8583
    at_pub_std: null
    at_pub_source_arxiv: '1901.08296'
    at_pub_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    at_pub_source_date_iso: '2018-12-14'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8583
    true_std: 0.0116
    value_gap_source_arxiv: '2412.17856'
    value_gap_source_title: Graph Structure Refinement with Energy-based Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.8583
    sort_std: 0.0116
    global_rank: 455
    paper_rank: 455
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PK
    model_key: pk
    model_plain: PK
    value: 0.76
    std: 0.027
    paper_value: 0.76
    paper_std: 0.027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.845
    at_pub_std: 0.006
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2014-10-13'
    value_gap_source_date_label: '2014'
    gap_vs_at_pub: 0.08499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.845
    true_std: 0.006
    value_gap_source_arxiv: '1410.3314'
    value_gap_source_title: Propagation Kernels
    value_gap_source_is_current_paper: false
    value_gap: 0.08499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.006
    global_rank: 508
    paper_rank: 767
    rank_delta: 259
    rank_delta_abs: 259
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Propagation Kernels
    comparison_source_arxiv: '1410.3314'
    is_best: false
    is_std_outlier: false
  - model: IGN
    model_key: ign
    model_plain: IGN
    value: 0.839
    std: 0.13
    paper_value: 0.839
    paper_std: 0.13
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.839
    at_pub_std: 0.13
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.13
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.13
    global_rank: 543
    paper_rank: 543
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GK (k=3)
    model_key: gk (k=3)
    model_plain: GK (k=3)
    value: 0.814
    std: 0.017
    paper_value: 0.814
    paper_std: 0.017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.814
    at_pub_std: 0.017
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2024-09-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.017
    value_gap_source_arxiv: '2409.19117'
    value_gap_source_title: 'Range-aware Positional Encoding via High-order Pretraining:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.017
    global_rank: 645
    paper_rank: 645
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RWK
    model_key: rwk
    model_plain: RWK
    value: 0.792
    std: 0.021
    paper_value: 0.792
    paper_std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation; reported average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.792
    at_pub_std: 0.021
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2024-09-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.792
    true_std: 0.021
    value_gap_source_arxiv: '2409.19117'
    value_gap_source_title: 'Range-aware Positional Encoding via High-order Pretraining:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.021
    global_rank: 712
    paper_rank: 712
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: NCI1
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.9934
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 2
    sort_value: 0.9934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9727
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL kernel
    model_key: wl kernel
    model_plain: WL kernel
    value: 0.86
    std: 0.018
    paper_value: 0.86
    paper_std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.86
    at_pub_std: 0.018
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2024-09-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2409.19117'
    value_gap_source_title: 'Range-aware Positional Encoding via High-order Pretraining:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
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
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.836
    std: 0.014
    paper_value: 0.836
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: Bodnar et al. 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.836
    at_pub_std: 0.014
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.853
    true_std: 0.012
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: 0.017000000000000015
    has_value_note: false
    value_note: ''
    sort_value: 0.853
    sort_std: 0.012
    global_rank: 20
    paper_rank: 52
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNN-AK+
    model_key: gnn-ak+
    model_plain: GNN-AK+
    value: 0.85
    std: 0.02
    paper_value: 0.85
    paper_std: 0.02
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.02
    value_gap_source_arxiv: '2404.13344'
    value_gap_source_title: 'GRANOLA: Adaptive Normalization for Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.02
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSN
    model_key: gsn
    model_plain: GSN
    value: 0.835
    std: 0.02
    paper_value: 0.835
    paper_std: 0.02
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.835
    at_pub_std: 0.02
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.02
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.02
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPGNs
    model_key: ppgns
    model_plain: PPGNs
    value: 0.832
    std: 0.011
    paper_value: 0.832
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.832
    at_pub_std: 0.011
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.832
    true_std: 0.011
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: 0.011
    global_rank: 72
    paper_rank: 72
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
    value: 0.8303
    std: 0.0137
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.01794'
    title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
      through In-depth Benchmarking'
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Armagaan/gnn-x-bench
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 82
    sort_value: 0.8303
    sort_std: 0.0137
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIN
    model_key: sin
    model_plain: SIN
    value: 0.827
    std: 0.021
    paper_value: 0.827
    paper_std: 0.021
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.828
    at_pub_std: 0.022
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.828
    true_std: 0.022
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.828
    sort_std: 0.022
    global_rank: 92
    paper_rank: 101
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Natural GN
    model_key: natural gn
    model_plain: Natural GN
    value: 0.824
    std: 0.013
    paper_value: 0.824
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.824
    at_pub_std: 0.013
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.824
    true_std: 0.013
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.824
    sort_std: 0.013
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.744
    std: 0.005
    paper_value: 0.744
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.765
    at_pub_std: 0.019
    at_pub_source_arxiv: '2009.10564'
    at_pub_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    at_pub_source_date_iso: '2020-09-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.02100000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.765
    true_std: 0.019
    value_gap_source_arxiv: '2009.10564'
    value_gap_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.02100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.765
    sort_std: 0.019
    global_rank: 411
    paper_rank: 471
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGN
    model_key: ign
    model_plain: IGN
    value: 0.743
    std: 0.027
    paper_value: 0.743
    paper_std: 0.027
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.743
    at_pub_std: 0.027
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7433
    true_std: 0.0271
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.7433
    sort_std: 0.0271
    global_rank: 475
    paper_rank: 477
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCNN
    model_key: dcnn
    model_plain: DCNN
    value: 0.566
    std: 0.01
    paper_value: 0.566
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation, reporting average accuracy
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.6261
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2018-12-14'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: 0.06010000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6261
    true_std: null
    value_gap_source_arxiv: '1901.08296'
    value_gap_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    value_gap_source_is_current_paper: false
    value_gap: 0.06010000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.6261
    sort_std: null
    global_rank: 598
    paper_rank: 626
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: PROTEINS
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.941
    std: 0.033
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.941
    sort_std: 0.033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRDL
    model_key: grdl
    model_plain: GRDL
    value: 0.826
    std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.11370'
    title: 'Graph Classification via Reference Distribution Learning: Theory and Practice'
    date: Aug 21, 2024
    date_display: Aug 2024
    date_iso: '2024-08-21'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.826
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8225
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
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.77
    std: 0.043
    paper_value: 0.77
    paper_std: 0.043
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
    table_ref: Table 9
    source_ref: bodnar2021b
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.77
    at_pub_std: 0.043
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.039
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: 0.03500000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.039
    global_rank: 14
    paper_rank: 97
    rank_delta: 83
    rank_delta_abs: 83
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
    value: 0.788
    std: 0.041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.08671'
    title: 'Permutation-Invariant graph partitioning: How graph neural networks capture
      structural interactions?'
    date: Dec 14, 2023
    date_display: Dec 2023
    date_iso: '2023-12-14'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 38
    sort_value: 0.788
    sort_std: 0.041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPGNs
    model_key: ppgns
    model_plain: PPGNs
    value: 0.772
    std: 0.047
    paper_value: 0.772
    paper_std: 0.047
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.772
    at_pub_std: 0.047
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.772
    true_std: 0.047
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: 0.047
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNN-AK+
    model_key: gnn-ak+
    model_plain: GNN-AK+
    value: 0.771
    std: 0.057
    paper_value: 0.771
    paper_std: 0.057
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.771
    true_std: 0.057
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.771
    sort_std: 0.057
    global_rank: 94
    paper_rank: 94
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGN
    model_key: ign
    model_plain: IGN
    value: 0.766
    std: 0.055
    paper_value: 0.766
    paper_std: 0.055
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.766
    at_pub_std: 0.055
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.766
    true_std: 0.055
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.766
    sort_std: 0.055
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSN
    model_key: gsn
    model_plain: GSN
    value: 0.766
    std: 0.05
    paper_value: 0.766
    paper_std: 0.05
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.766
    at_pub_std: 0.05
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.766
    true_std: 0.05
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.766
    sort_std: 0.05
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIN
    model_key: sin
    model_plain: SIN
    value: 0.764
    std: 0.033
    paper_value: 0.764
    paper_std: 0.033
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.764
    at_pub_std: 0.033
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.765
    true_std: 0.034
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.765
    sort_std: 0.034
    global_rank: 126
    paper_rank: 138
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.755
    std: 0.009
    paper_value: 0.755
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.7626
    at_pub_std: null
    at_pub_source_arxiv: '2109.11338'
    at_pub_source_title: Orthogonal Graph Neural Networks
    at_pub_source_date_iso: '2021-09-23'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-09-23'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.00759999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7626
    true_std: null
    value_gap_source_arxiv: '2109.11338'
    value_gap_source_title: Orthogonal Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00759999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7626
    sort_std: null
    global_rank: 154
    paper_rank: 215
    rank_delta: 61
    rank_delta_abs: 61
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
    value: 0.76
    std: 0.032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.76
    sort_std: 0.032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL kernel
    model_key: wl kernel
    model_plain: WL kernel
    value: 0.75
    std: 0.031
    paper_value: 0.75
    paper_std: 0.031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.75
    at_pub_std: 0.031
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.75
    true_std: 0.031
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.75
    sort_std: 0.031
    global_rank: 278
    paper_rank: 278
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PK
    model_key: pk
    model_plain: PK
    value: 0.737
    std: 0.007
    paper_value: 0.737
    paper_std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.737
    at_pub_std: 0.007
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2024-10-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.737
    true_std: 0.007
    value_gap_source_arxiv: '2410.08524'
    value_gap_source_title: 'IGNN-Solver: A Graph Neural Solver for Implicit Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: 0.007
    global_rank: 363
    paper_rank: 363
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Natural GN
    model_key: natural gn
    model_plain: Natural GN
    value: 0.717
    std: 0.01
    paper_value: 0.717
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
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.717
    at_pub_std: 0.01
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.717
    true_std: 0.01
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.717
    sort_std: 0.01
    global_rank: 465
    paper_rank: 465
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GK (k=3)
    model_key: gk (k=3)
    model_plain: GK (k=3)
    value: 0.714
    std: 0.0031
    paper_value: 0.714
    paper_std: 0.0031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.714
    at_pub_std: 0.003
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.714
    true_std: 0.003
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.003
    global_rank: 475
    paper_rank: 475
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCNN
    model_key: dcnn
    model_plain: DCNN
    value: 0.613
    std: 0.016
    paper_value: 0.613
    paper_std: 0.016
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
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.613
    at_pub_std: 0.016
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.613
    true_std: 0.016
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.613
    sort_std: 0.016
    global_rank: 551
    paper_rank: 551
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RWK
    model_key: rwk
    model_plain: RWK
    value: 0.596
    std: 0.001
    paper_value: 0.596
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 9
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on PROTEINS
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.596
    at_pub_std: 0.001
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.596
    true_std: 0.001
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.596
    sort_std: 0.001
    global_rank: 560
    paper_rank: 560
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: RDT-B
  rows:
  - model: OEPG
    model_key: oepg
    model_plain: OEPG
    value: 0.963
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.963
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.958
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.958
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GNN-AK+
    model_key: gnn-ak+
    model_plain: GNN-AK+
    value: 0.948
    std: 0.008
    paper_value: 0.948
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
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on RDT-B
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.948
    true_std: 0.008
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.008
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.924
    std: 0.021
    paper_value: 0.924
    paper_std: 0.021
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
    table_ref: Table 5
    source_ref: bodnar2021b
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on RDT-B
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.924
    at_pub_std: 0.021
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.924
    true_std: 0.021
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.924
    sort_std: 0.021
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.924
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 12
    sort_value: 0.924
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIN
    model_key: sin
    model_plain: SIN
    value: 0.922
    std: 0.01
    paper_value: 0.922
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
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on RDT-B
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.922
    at_pub_std: 0.01
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.922
    true_std: 0.01
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.01
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL kernel
    model_key: wl kernel
    model_plain: WL kernel
    value: 0.81
    std: 0.031
    paper_value: 0.81
    paper_std: 0.031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy on RDT-B
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.81
    at_pub_std: 0.031
    at_pub_source_arxiv: '2103.03212'
    at_pub_source_title: 'Weisfeiler and Lehman Go Topological: Message Passing Simplicial
      Networks'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: 0.031
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: 0.031
    global_rank: 72
    paper_rank: 72
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
- benchmark: GNNBenchmark
  datasets:
  - *id005
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: RDT-B
      dataset_slug: rdt-b
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CIFAR10
      dataset_slug: cifar10
main_figure: /figures/2110.03753/main_figure.jpegoptim.jpg
---

