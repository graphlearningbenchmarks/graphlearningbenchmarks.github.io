---
title: Graph Information Bottleneck for Subgraph Recognition
arxiv_id: '2010.05563'
source_url: ''
authors:
- name: Junchi Yu
  orcid: null
  s2_author_id: '28822585'
  s2_url: null
- name: Tingyang Xu
  orcid: null
  s2_author_id: '1754673'
  s2_url: null
- name: Yu Rong
  orcid: null
  s2_author_id: '48537464'
  s2_url: null
- name: Yatao Bian
  orcid: null
  s2_author_id: '2419616'
  s2_url: null
- name: Junzhou Huang
  orcid: null
  s2_author_id: '1768190'
  s2_url: null
- name: Ran He
  orcid: null
  s2_author_id: '143712929'
  s2_url: null
published_date: Oct 12, 2020
published_date_iso: '2020-10-12'
published_venue: ICLR 2020
published_conference: ICLR 2020
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Given the input graph and its label/property, several key problems of graph
  learning, such as finding interpretable subgraphs, graph denoising and graph compression,
  can be attributed to the fundamental problem of recognizing a subgraph of the original
  one. This subgraph shall be as informative as possible, yet contains less redundant
  and noisy structure. This problem setting is closely related to the well-known information
  bottleneck (IB) principle, which, however, has less been studied for the irregular
  graph data and graph neural networks (GNNs). In this paper, we propose a framework
  of Graph Information Bottleneck (GIB) for the subgraph recognition problem in deep
  graph learning. Under this framework, one can recognize the maximally informative
  yet compressive subgraph, named IB-subgraph. However, the GIB objective is notoriously
  hard to optimize, mostly due to the intractability of the mutual information of
  irregular graph data and the unstable optimization process. In order to tackle these
  challenges, we propose: i) a GIB objective based-on a mutual information estimator
  for the irregular graph data; ii) a bi-level optimization scheme to maximize the
  GIB objective; iii) a connectivity loss to stabilize the optimization process. We
  evaluate the properties of the IB-subgraph in three application scenarios: improvement
  of graph classification, graph interpretation and graph denoising. Extensive experiments
  demonstrate that the information-theoretic IB-subgraph enjoys superior graph properties.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id003
  dataset: IMDB-BINARY
  rows:
  - model: DMoNPool-TIP
    model_key: gcfl
    model_plain: DMoNPool-TIP
    value: 0.8299
    std: 0.052
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8299
    sort_std: 0.052
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMoNPool-TIP
    model_key: gat +del-f
    model_plain: DMoNPool-TIP
    value: 0.7863
    std: 0.0054
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7863
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMoNPool-TIP
    model_key: graph transformer +del-f
    model_plain: DMoNPool-TIP
    value: 0.7828
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7828
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.709
    std: 0.041
    paper_value: 0.709
    paper_std: 0.041
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.723
    at_pub_std: 0.053
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.014000000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.766
    true_std: 0.0237
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.05700000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.766
    sort_std: 0.0237
    global_rank: 11
    paper_rank: 132
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.732
    std: 0.048
    paper_value: 0.732
    paper_std: 0.048
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.751
    at_pub_std: 0.051
    at_pub_source_arxiv: '2005.01214'
    at_pub_source_title: Graph Homomorphism Convolution
    at_pub_source_date_iso: '2020-05-03'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.019000000000000017
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7641
    true_std: 0.0093
    value_gap_source_arxiv: '2402.16402'
    value_gap_source_title: Graph Learning with Distributional Edge Layouts
    value_gap_source_is_current_paper: false
    value_gap: 0.03210000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7641
    sort_std: 0.0093
    global_rank: 14
    paper_rank: 74
    rank_delta: 60
    rank_delta_abs: 60
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
    value: 0.707
    std: 0.037
    paper_value: 0.707
    paper_std: 0.037
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.74
    at_pub_std: 0.034
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.03300000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.742
    true_std: 0.024
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.03500000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.742
    sort_std: 0.024
    global_rank: 47
    paper_rank: 132
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.713
    std: 0.042
    paper_value: 0.713
    paper_std: 0.042
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.705
    at_pub_std: 0.023
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2021-08-24'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7407
    true_std: 0.0453
    value_gap_source_arxiv: '2108.10587'
    value_gap_source_title: Pooling Architecture Search for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.027700000000000058
    has_value_note: false
    value_note: ''
    sort_value: 0.7407
    sort_std: 0.0453
    global_rank: 53
    paper_rank: 121
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN+GIB
    model_key: gin+gib
    model_plain: GIN+GIB
    value: 0.737
    std: 0.07
    paper_value: 0.737
    paper_std: 0.07
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.737
    true_std: 0.07
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: 0.07
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.709
    std: 0.053
    paper_value: 0.709
    paper_std: 0.053
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7315
    true_std: 0.033
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.022500000000000075
    has_value_note: false
    value_note: ''
    sort_value: 0.7315
    sort_std: 0.033
    global_rank: 78
    paper_rank: 132
    rank_delta: 54
    rank_delta_abs: 54
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+GIB
    model_key: gat+gib
    model_plain: GAT+GIB
    value: 0.729
    std: 0.046
    paper_value: 0.729
    paper_std: 0.046
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: 0.046
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.046
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
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.728
    std: 0.044
    paper_value: 0.728
    paper_std: 0.044
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.728
    true_std: 0.044
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.728
    sort_std: 0.044
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttPool
    model_key: attpool
    model_plain: AttPool
    value: 0.722
    std: 0.047
    paper_value: 0.722
    paper_std: 0.047
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.722
    true_std: 0.047
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.722
    sort_std: 0.047
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
  - model: GCN+GIB
    model_key: gcn+gib
    model_plain: GCN+GIB
    value: 0.722
    std: 0.039
    paper_value: 0.722
    paper_std: 0.039
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.722
    true_std: 0.039
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.722
    sort_std: 0.039
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.712
    std: 0.047
    paper_value: 0.712
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7212
    true_std: 0.0112
    value_gap_source_arxiv: '2206.13510'
    value_gap_source_title: Structural Entropy Guided Graph Hierarchical Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.009199999999999986
    has_value_note: false
    value_note: ''
    sort_value: 0.7212
    sort_std: 0.0112
    global_rank: 104
    paper_rank: 121
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+GIB
    model_key: graphsage+gib
    model_plain: GraphSAGE+GIB
    value: 0.719
    std: 0.052
    paper_value: 0.719
    paper_std: 0.052
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.719
    true_std: 0.052
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.719
    sort_std: 0.052
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASAPool
    model_key: asapool
    model_plain: ASAPool
    value: 0.715
    std: 0.044
    paper_value: 0.715
    paper_std: 0.044
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.044
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.044
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
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.825
    std: 0.068
    paper_value: 0.825
    paper_std: 0.068
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.894
    at_pub_std: 0.056
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.06900000000000006
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.1080000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 34
    paper_rank: 546
    rank_delta: 512
    rank_delta_abs: 512
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.743
    std: 0.077
    paper_value: 0.743
    paper_std: 0.077
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.857
    at_pub_std: 0.047
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-05-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.11399999999999999
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.078
    value_gap_source_arxiv: '2205.12245'
    value_gap_source_title: Asynchronous Neural Networks for Learning in Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.16100000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.078
    global_rank: 140
    paper_rank: 726
    rank_delta: 586
    rank_delta_abs: 586
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.738
    std: 0.074
    paper_value: 0.738
    paper_std: 0.074
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.894
    at_pub_std: 0.061
    at_pub_source_arxiv: '1909.11855'
    at_pub_source_title: Universal Graph Transformer Self-Attention Networks
    at_pub_source_date_iso: '2019-09-26'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.15600000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.901
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.16300000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.058
    global_rank: 164
    paper_rank: 739
    rank_delta: 575
    rank_delta_abs: 575
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Universal Graph Transformer Self-Attention Networks
    comparison_source_arxiv: '1909.11855'
    is_best: false
    is_std_outlier: false
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.844
    std: 0.141
    paper_value: 0.844
    paper_std: 0.141
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.773
    at_pub_std: 0.089
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07099999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: 0.0224
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.05600000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.0224
    global_rank: 170
    paper_rank: 468
    rank_delta: 298
    rank_delta_abs: 298
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.839
    std: 0.097
    paper_value: 0.839
    paper_std: 0.097
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.85
    at_pub_std: 0.103
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-08-21'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.046
    value_gap_source_arxiv: '2408.11370'
    value_gap_source_title: 'Graph Classification via Reference Distribution Learning:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: 0.05500000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.046
    global_rank: 218
    paper_rank: 492
    rank_delta: 274
    rank_delta_abs: 274
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
    value: 0.743
    std: 0.11
    paper_value: 0.743
    paper_std: 0.11
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.857
    at_pub_std: 0.066
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.11399999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.891
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.14800000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.058
    global_rank: 250
    paper_rank: 726
    rank_delta: 476
    rank_delta_abs: 476
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+GIB
    model_key: gin+gib
    model_plain: GIN+GIB
    value: 0.839
    std: 0.064
    paper_value: 0.839
    paper_std: 0.064
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.064
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.064
    global_rank: 495
    paper_rank: 495
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.759
    std: 0.077
    paper_value: 0.759
    paper_std: 0.077
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8101
    true_std: 0.0082
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.051100000000000034
    has_value_note: false
    value_note: ''
    sort_value: 0.8101
    sort_std: 0.0082
    global_rank: 595
    paper_rank: 707
    rank_delta: 112
    rank_delta_abs: 112
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+GIB
    model_key: gcn+gib
    model_plain: GCN+GIB
    value: 0.776
    std: 0.075
    paper_value: 0.776
    paper_std: 0.075
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.776
    true_std: 0.075
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.776
    sort_std: 0.075
    global_rank: 680
    paper_rank: 680
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+GIB
    model_key: graphsage+gib
    model_plain: GraphSAGE+GIB
    value: 0.76
    std: 0.074
    paper_value: 0.76
    paper_std: 0.074
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76
    true_std: 0.074
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.074
    global_rank: 705
    paper_rank: 705
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+GIB
    model_key: gat+gib
    model_plain: GAT+GIB
    value: 0.749
    std: 0.097
    paper_value: 0.749
    paper_std: 0.097
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.097
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.097
    global_rank: 723
    paper_rank: 723
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASAPool
    model_key: asapool
    model_plain: ASAPool
    value: 0.743
    std: 0.077
    paper_value: 0.743
    paper_std: 0.077
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.743
    true_std: 0.077
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.077
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
  - model: AttPool
    model_key: attpool
    model_plain: AttPool
    value: 0.721
    std: 0.086
    paper_value: 0.721
    paper_std: 0.086
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.721
    true_std: 0.086
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.721
    sort_std: 0.086
    global_rank: 755
    paper_rank: 755
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
  dataset: PROTEINS
  rows:
  - model: Graphormer-SPIS
    model_key: gmn
    model_plain: Graphormer-SPIS
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
    global_rank: 1
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: ci-gnn
    model_plain: Graphormer-SPIS
    value: 0.82
    std: 0.02
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.01642'
    title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network for Interpretable
      Brain Network-Based Psychiatric Diagnosis'
    date: Jan 4, 2023
    date_display: Jan 2023
    date_iso: '2023-01-04'
    venue: Neural Networks
    codebase_url: https://github.com/ZKZ-Brain/CI-GNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.82
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: diffpool+gpl
    model_plain: Graphormer-SPIS
    value: 0.8196
    std: 0.0286
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Applied intelligence (Boston)
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8196
    sort_std: 0.0286
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.727
    std: 0.046
    paper_value: 0.727
    paper_std: 0.046
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.7625
    at_pub_std: null
    at_pub_source_arxiv: '2002.09518'
    at_pub_source_title: Memory-Based Graph Networks
    at_pub_source_date_iso: '2020-02-21'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.035499999999999976
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8161
    true_std: 0.0232
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.08910000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8161
    sort_std: 0.0232
    global_rank: 4
    paper_rank: 385
    rank_delta: 381
    rank_delta_abs: 381
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.707
    std: 0.056
    paper_value: 0.707
    paper_std: 0.056
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.762
    at_pub_std: 0.028
    at_pub_source_arxiv: '1905.12560'
    at_pub_source_title: On the Equivalence between Graph Isomorphism Testing and
      Function Approximation with GNNs
    at_pub_source_date_iso: '2019-05-29'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.05500000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.788
    true_std: 0.041
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.041
    global_rank: 27
    paper_rank: 444
    rank_delta: 417
    rank_delta_abs: 417
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.714
    std: 0.04
    paper_value: 0.714
    paper_std: 0.04
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.747
    at_pub_std: 0.022
    at_pub_source_arxiv: '1909.11855'
    at_pub_source_title: Universal Graph Transformer Self-Attention Networks
    at_pub_source_date_iso: '2019-09-26'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2023-01-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03300000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.78
    true_std: 0.03
    value_gap_source_arxiv: '2301.01642'
    value_gap_source_title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network
      for Interpretable Brain Network-Based Psychiatric Diagnosis'
    value_gap_source_is_current_paper: false
    value_gap: 0.06600000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.78
    sort_std: 0.03
    global_rank: 47
    paper_rank: 430
    rank_delta: 383
    rank_delta_abs: 383
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.721
    std: 0.042
    paper_value: 0.721
    paper_std: 0.042
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.759
    at_pub_std: 0.032
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.038000000000000034
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7667
    true_std: 0.0305
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.045700000000000074
    has_value_note: false
    value_note: ''
    sort_value: 0.7667
    sort_std: 0.0305
    global_rank: 93
    paper_rank: 409
    rank_delta: 316
    rank_delta_abs: 316
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
    value: 0.719
    std: 0.041
    paper_value: 0.719
    paper_std: 0.041
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.76
    at_pub_std: 0.032
    at_pub_source_arxiv: '1909.11855'
    at_pub_source_title: Universal Graph Transformer Self-Attention Networks
    at_pub_source_date_iso: '2019-09-26'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.041000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7665
    true_std: 0.0314
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.04749999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7665
    sort_std: 0.0314
    global_rank: 94
    paper_rank: 415
    rank_delta: 321
    rank_delta_abs: 321
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SortPool
    model_key: sortpool
    model_plain: SortPool
    value: 0.747
    std: 0.044
    paper_value: 0.747
    paper_std: 0.044
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: 0.7554
    at_pub_std: null
    at_pub_source_arxiv: '2002.09518'
    at_pub_source_title: Memory-Based Graph Networks
    at_pub_source_date_iso: '2020-02-21'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.008399999999999963
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7598
    true_std: 0.0176
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.012800000000000034
    has_value_note: false
    value_note: ''
    sort_value: 0.7598
    sort_std: 0.0176
    global_rank: 156
    paper_rank: 284
    rank_delta: 128
    rank_delta_abs: 128
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.723
    std: 0.044
    paper_value: 0.723
    paper_std: 0.044
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.756
    true_std: 0.024
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.03300000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.024
    global_rank: 193
    paper_rank: 404
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+GIB
    model_key: gin+gib
    model_plain: GIN+GIB
    value: 0.749
    std: 0.051
    paper_value: 0.749
    paper_std: 0.051
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.051
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.051
    global_rank: 271
    paper_rank: 271
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+GIB
    model_key: gcn+gib
    model_plain: GCN+GIB
    value: 0.748
    std: 0.046
    paper_value: 0.748
    paper_std: 0.046
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.748
    true_std: 0.046
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.748
    sort_std: 0.046
    global_rank: 281
    paper_rank: 281
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+GIB
    model_key: gat+gib
    model_plain: GAT+GIB
    value: 0.737
    std: 0.044
    paper_value: 0.737
    paper_std: 0.044
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.737
    true_std: 0.044
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: 0.044
    global_rank: 341
    paper_rank: 341
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+GIB
    model_key: graphsage+gib
    model_plain: GraphSAGE+GIB
    value: 0.734
    std: 0.043
    paper_value: 0.734
    paper_std: 0.043
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.043
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.043
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
  - model: AttPool
    model_key: attpool
    model_plain: AttPool
    value: 0.728
    std: 0.041
    paper_value: 0.728
    paper_std: 0.041
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-10-12'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.728
    true_std: 0.041
    value_gap_source_arxiv: '2010.05563'
    value_gap_source_title: Graph Information Bottleneck for Subgraph Recognition
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.728
    sort_std: 0.041
    global_rank: 383
    paper_rank: 383
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ASAPool
    model_key: asapool
    model_plain: ASAPool
    value: 0.721
    std: 0.043
    paper_value: 0.721
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 12, 2020
    date_display: Oct 2020
    date_iso: '2020-10-12'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7232
    true_std: 0.0291
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.7232
    sort_std: 0.0291
    global_rank: 403
    paper_rank: 409
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: IMDB-BINARY
      dataset_slug: imdb-binary
main_figure: /figures/2010.05563/main_figure.jpegoptim.jpg
---

