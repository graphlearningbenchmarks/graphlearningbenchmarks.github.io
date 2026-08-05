---
title: Rethinking Graph Regularization for Graph Neural Networks
arxiv_id: '2009.02027'
source_url: ''
authors:
- name: Han Yang
  orcid: null
  s2_author_id: '50841357'
  s2_url: null
- name: Kaili Ma
  orcid: null
  s2_author_id: '47737190'
  s2_url: null
- name: James Cheng
  orcid: null
  s2_author_id: '1717691'
  s2_url: null
published_date: Sep 4, 2020
published_date_iso: '2020-09-04'
published_venue: AAAI 2020
published_conference: AAAI 2020
published_conference_short: AAAI
published_conference_slug: aaai
abstract: The graph Laplacian regularization term is usually used in semi-supervised
  representation learning to provide graph structure information for a model $f(X)$.
  However, with the recent popularity of graph neural networks (GNNs), directly encoding
  graph structure $A$ into a model, i.e., $f(A, X)$, has become the more common approach.
  While we show that graph Laplacian regularization brings little-to-no benefit to
  existing GNNs, and propose a simple but non-trivial variant of graph Laplacian regularization,
  called Propagation-regularization (P-reg), to boost the performance of existing
  GNN models. We provide formal analyses to show that P-reg not only infuses extra
  information (that is not captured by the traditional graph Laplacian regularization)
  into GNNs, but also has the capacity equivalent to an infinite-depth graph convolutional
  network. We demonstrate that P-reg can effectively boost the performance of existing
  GNN models on both node-level and graph-level tasks across many different datasets.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN+P-reg
- GAT+P-reg
- GCN+Virtual+P-reg
- GIN+P-reg
- GIN+Virtual+P-reg
mrr: 0.0037
adjusted_mrr: 0.0037
mrr_dataset_count: 5
benchmark_categories:
- Classic
- OGB
- MoleculeNet
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id002
  dataset: CiteSeer
  rows:
  - model: SGC+TSC
    model_key: cna
    model_plain: SGC+TSC
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
  - model: SGC+TSC
    model_key: is-gib
    model_plain: SGC+TSC
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
    input_feature_source: null
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
  - model: SGC+TSC
    model_key: eerm
    model_plain: SGC+TSC
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
    input_feature_source: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7157
    std: 0.0046
    paper_value: 0.7157
    paper_std: 0.0046
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.768
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.05230000000000001
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
    value_gap: 0.1612
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 565
    rank_delta: 544
    rank_delta_abs: 544
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.72
    std: 0.0048
    paper_value: 0.72
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.805
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.08500000000000008
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
    value_gap: 0.09420000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 515
    rank_delta: 486
    rank_delta_abs: 486
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
    value: 0.7129
    std: 0.0084
    paper_value: 0.7129
    paper_std: 0.0084
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.786
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.07310000000000005
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
    value_gap: 0.09510000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 592
    rank_delta: 546
    rank_delta_abs: 546
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GCN+P-reg
    model_key: gcn+p-reg
    model_plain: GCN+P-reg
    value: 0.7483
    std: 0.0017
    paper_value: 0.7483
    paper_std: 0.0017
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7483
    true_std: 0.0017
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7483
    sort_std: 0.0017
    global_rank: 226
    paper_rank: 226
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.7381
    std: 0.0085
    paper_value: 0.7381
    paper_std: 0.0085
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.747
    true_std: 0.0059
    value_gap_source_arxiv: '2203.14082'
    value_gap_source_title: Metropolis-Hastings Data Augmentation for Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.008900000000000019
    has_value_note: false
    value_note: ''
    sort_value: 0.747
    sort_std: 0.0059
    global_rank: 230
    paper_rank: 279
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BVAT
    model_key: bvat
    model_plain: BVAT
    value: 0.7383
    std: 0.0054
    paper_value: 0.7383
    paper_std: 0.0054
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.74
    at_pub_std: 0.006
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-03-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0017000000000000348
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.74
    true_std: 0.006
    value_gap_source_arxiv: '2203.14082'
    value_gap_source_title: Metropolis-Hastings Data Augmentation for Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0017000000000000348
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.006
    global_rank: 270
    paper_rank: 279
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAT
    model_key: graphat
    model_plain: GraphAT
    value: 0.7349
    std: 0.0038
    paper_value: 0.7349
    paper_std: 0.0038
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.734
    at_pub_std: null
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7349
    true_std: 0.0038
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7349
    sort_std: 0.0038
    global_rank: 323
    paper_rank: 323
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMNN
    model_key: gmnn
    model_plain: GMNN
    value: 0.7277
    std: 0.0143
    paper_value: 0.7277
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.731
    at_pub_std: null
    at_pub_source_arxiv: '2009.00934'
    at_pub_source_title: 'SAIL: Self-Augmented Graph Contrastive Learning'
    at_pub_source_date_iso: '2020-09-02'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-02'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.0032999999999999696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.731
    true_std: null
    value_gap_source_arxiv: '2009.00934'
    value_gap_source_title: 'SAIL: Self-Augmented Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0032999999999999696
    has_value_note: false
    value_note: ''
    sort_value: 0.731
    sort_std: null
    global_rank: 366
    paper_rank: 409
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+P-reg
    model_key: gat+p-reg
    model_plain: GAT+P-reg
    value: 0.7286
    std: 0.0065
    paper_value: 0.7286
    paper_std: 0.0065
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7286
    true_std: 0.0065
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7286
    sort_std: 0.0065
    global_rank: 403
    paper_rank: 403
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.7274
    std: 0.0062
    paper_value: 0.7274
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7274
    true_std: 0.0062
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7274
    sort_std: 0.0062
    global_rank: 412
    paper_rank: 412
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepAPPNP
    model_key: deepappnp
    model_plain: DeepAPPNP
    value: 0.7137
    std: 0.0066
    paper_value: 0.7137
    paper_std: 0.0066
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7137
    true_std: 0.0066
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7137
    sort_std: 0.0066
    global_rank: 585
    paper_rank: 585
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph U-Nets
    model_key: graph u-nets
    model_plain: Graph U-Nets
    value: 0.6774
    std: 0.0148
    paper_value: 0.6774
    paper_std: 0.0148
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Uses standard split (Yang et al. 2016 fixed split).
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6774
    true_std: 0.0148
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6774
    sort_std: 0.0148
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
    value: 0.8167
    std: 0.006
    paper_value: 0.8167
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.8717
    at_pub_std: 0.0058
    at_pub_source_arxiv: '1711.08920'
    at_pub_source_title: 'SplineCNN: Fast Geometric Deep Learning with Continuous
      B-Spline Kernels'
    at_pub_source_date_iso: '2017-11-24'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05500000000000005
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
    value_gap: 0.0837
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 690
    rank_delta: 657
    rank_delta_abs: 657
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
    value: 0.8312
    std: 0.0044
    paper_value: 0.8312
    paper_std: 0.0044
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04579999999999995
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
    value_gap: 0.05919999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 529
    rank_delta: 460
    rank_delta_abs: 460
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
    value: 0.832
    std: 0.0072
    paper_value: 0.832
    paper_std: 0.0072
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.874
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.04200000000000004
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
    value_gap: 0.057700000000000085
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 514
    rank_delta: 442
    rank_delta_abs: 442
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.8354
    std: 0.0072
    paper_value: 0.8354
    paper_std: 0.0072
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.8394
    at_pub_std: 0.0057
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8394
    true_std: 0.0057
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.8394
    sort_std: 0.0057
    global_rank: 410
    paper_rank: 471
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+P-reg
    model_key: gat+p-reg
    model_plain: GAT+P-reg
    value: 0.8389
    std: 0.0031
    paper_value: 0.8389
    paper_std: 0.0031
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8389
    true_std: 0.0031
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8389
    sort_std: 0.0031
    global_rank: 419
    paper_rank: 419
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepAPPNP
    model_key: deepappnp
    model_plain: DeepAPPNP
    value: 0.8378
    std: 0.0033
    paper_value: 0.8378
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8378
    true_std: 0.0033
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8378
    sort_std: 0.0033
    global_rank: 428
    paper_rank: 428
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMNN
    model_key: gmnn
    model_plain: GMNN
    value: 0.8318
    std: 0.0085
    paper_value: 0.8318
    paper_std: 0.0085
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.837
    at_pub_std: null
    at_pub_source_arxiv: '2008.12578'
    at_pub_source_title: Graph Convolutional Neural Networks with Node Transition
      Probability-based Message Passing and DropNode Regularization
    at_pub_source_date_iso: '2020-08-28'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-02'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.005199999999999982
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.837
    true_std: null
    value_gap_source_arxiv: '2009.00934'
    value_gap_source_title: 'SAIL: Self-Augmented Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.005199999999999982
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: null
    global_rank: 432
    paper_rank: 527
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BVAT
    model_key: bvat
    model_plain: BVAT
    value: 0.8337
    std: 0.0101
    paper_value: 0.8337
    paper_std: 0.0101
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.836
    at_pub_std: 0.005
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-03-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0022999999999999687
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.005
    value_gap_source_arxiv: '2203.14082'
    value_gap_source_title: Metropolis-Hastings Data Augmentation for Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0022999999999999687
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.005
    global_rank: 454
    paper_rank: 498
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+P-reg
    model_key: gcn+p-reg
    model_plain: GCN+P-reg
    value: 0.8338
    std: 0.0086
    paper_value: 0.8338
    paper_std: 0.0086
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8338
    true_std: 0.0086
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8338
    sort_std: 0.0086
    global_rank: 498
    paper_rank: 498
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAT
    model_key: graphat
    model_plain: GraphAT
    value: 0.8246
    std: 0.006
    paper_value: 0.8246
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.825
    at_pub_std: null
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.825
    true_std: null
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.825
    sort_std: null
    global_rank: 580
    paper_rank: 587
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.8228
    std: 0.0048
    paper_value: 0.8228
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8228
    true_std: 0.0048
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8228
    sort_std: 0.0048
    global_rank: 620
    paper_rank: 620
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph U-Nets
    model_key: graph u-nets
    model_plain: Graph U-Nets
    value: 0.8131
    std: 0.0147
    paper_value: 0.8131
    paper_std: 0.0147
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8131
    true_std: 0.0147
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8131
    sort_std: 0.0147
    global_rank: 706
    paper_rank: 706
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
- &id003
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.801
    std: 0.0026
    paper_value: 0.801
    paper_std: 0.0026
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.905
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10399999999999998
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
    global_rank: 20
    paper_rank: 463
    rank_delta: 443
    rank_delta_abs: 443
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7917
    std: 0.0037
    paper_value: 0.7917
    paper_std: 0.0037
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10530000000000006
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
    value_gap: 0.13790000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 595
    rank_delta: 574
    rank_delta_abs: 574
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
    value: 0.7799
    std: 0.0047
    paper_value: 0.7799
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.11709999999999998
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
    value_gap: 0.14339999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 716
    rank_delta: 693
    rank_delta_abs: 693
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GMNN
    model_key: gmnn
    model_plain: GMNN
    value: 0.8163
    std: 0.0036
    paper_value: 0.8163
    paper_std: 0.0036
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.818
    at_pub_std: null
    at_pub_source_arxiv: '2009.00934'
    at_pub_source_title: 'SAIL: Self-Augmented Graph Contrastive Learning'
    at_pub_source_date_iso: '2020-09-02'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-02'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.0016999999999999238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.818
    true_std: null
    value_gap_source_arxiv: '2009.00934'
    value_gap_source_title: 'SAIL: Self-Augmented Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0016999999999999238
    has_value_note: false
    value_note: ''
    sort_value: 0.818
    sort_std: null
    global_rank: 353
    paper_rank: 354
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.8076
    std: 0.0084
    paper_value: 0.8076
    paper_std: 0.0084
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.811
    at_pub_std: 0.0078
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.0034000000000000696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.0078
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0034000000000000696
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.0078
    global_rank: 387
    paper_rank: 411
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+P-reg
    model_key: gcn+p-reg
    model_plain: GCN+P-reg
    value: 0.8011
    std: 0.0045
    paper_value: 0.8011
    paper_std: 0.0045
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8011
    true_std: 0.0045
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8011
    sort_std: 0.0045
    global_rank: 463
    paper_rank: 463
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BVAT
    model_key: bvat
    model_plain: BVAT
    value: 0.7797
    std: 0.0084
    paper_value: 0.7797
    paper_std: 0.0084
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.799
    at_pub_std: 0.004
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.019300000000000095
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.799
    true_std: 0.004
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.019300000000000095
    has_value_note: false
    value_note: ''
    sort_value: 0.799
    sort_std: 0.004
    global_rank: 484
    paper_rank: 716
    rank_delta: 232
    rank_delta_abs: 232
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    comparison_source_arxiv: '1909.11715'
    is_best: false
    is_std_outlier: false
  - model: DeepAPPNP
    model_key: deepappnp
    model_plain: DeepAPPNP
    value: 0.7973
    std: 0.0022
    paper_value: 0.7973
    paper_std: 0.0022
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7973
    true_std: 0.0022
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7973
    sort_std: 0.0022
    global_rank: 503
    paper_rank: 503
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.796
    std: 0.0063
    paper_value: 0.796
    paper_std: 0.0063
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.796
    true_std: 0.0063
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.0063
    global_rank: 519
    paper_rank: 519
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAT
    model_key: graphat
    model_plain: GraphAT
    value: 0.791
    std: 0.002
    paper_value: 0.791
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.791
    true_std: 0.002
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: 0.002
    global_rank: 606
    paper_rank: 606
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+P-reg
    model_key: gat+p-reg
    model_plain: GAT+P-reg
    value: 0.7839
    std: 0.0027
    paper_value: 0.7839
    paper_std: 0.0027
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7839
    true_std: 0.0027
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7839
    sort_std: 0.0027
    global_rank: 687
    paper_rank: 687
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph U-Nets
    model_key: graph u-nets
    model_plain: Graph U-Nets
    value: 0.7776
    std: 0.0084
    paper_value: 0.7776
    paper_std: 0.0084
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7776
    true_std: 0.0084
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7776
    sort_std: 0.0084
    global_rank: 734
    paper_rank: 734
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
- &id005
  dataset: Tox21
  rows:
  - model: HOD-GNN
    model_key: himp
    model_plain: HOD-GNN
    value: 0.874
    std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.874
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: gine w/ vn
    model_plain: HOD-GNN
    value: 0.872
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.872
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: naivegine+ k=3 w/ vn
    model_plain: HOD-GNN
    value: 0.87
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.87
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7475
    std: 0.0055
    paper_value: 0.7475
    paper_std: 0.0055
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.829
    at_pub_std: 0.006
    at_pub_source_arxiv: '2002.09518'
    at_pub_source_title: Memory-Based Graph Networks
    at_pub_source_date_iso: '2020-02-21'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-11-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0814999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.84
    true_std: 0.004
    value_gap_source_arxiv: '2011.15069'
    value_gap_source_title: Graph convolutions that can finally model local structure
    value_gap_source_is_current_paper: false
    value_gap: 0.09249999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: 0.004
    global_rank: 15
    paper_rank: 234
    rank_delta: 219
    rank_delta_abs: 219
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Memory-Based Graph Networks
    comparison_source_arxiv: '2002.09518'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7489
    std: 0.0066
    paper_value: 0.7489
    paper_std: 0.0066
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.829
    at_pub_std: 0.0069
    at_pub_source_arxiv: '1905.11577'
    at_pub_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    at_pub_source_date_iso: '2019-05-28'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-05-28'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.08009999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.829
    true_std: 0.0069
    value_gap_source_arxiv: '1905.11577'
    value_gap_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.08009999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.0069
    global_rank: 25
    paper_rank: 232
    rank_delta: 207
    rank_delta_abs: 207
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Interpretable Sparse Graph Representation Learning
      with Laplacian Pooling
    comparison_source_arxiv: '1905.11577'
    is_best: false
    is_std_outlier: false
  - model: GCN+Virtual+P-reg
    model_key: gcn+virtual+p-reg
    model_plain: GCN+Virtual+P-reg
    value: 0.7758
    std: 0.0039
    paper_value: 0.7758
    paper_std: 0.0039
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7758
    true_std: 0.0039
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7758
    sort_std: 0.0039
    global_rank: 130
    paper_rank: 130
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+Virtual+P-reg
    model_key: gin+virtual+p-reg
    model_plain: GIN+Virtual+P-reg
    value: 0.7751
    std: 0.0068
    paper_value: 0.7751
    paper_std: 0.0068
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7751
    true_std: 0.0068
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7751
    sort_std: 0.0068
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+Virtual
    model_key: gcn+virtual
    model_plain: GCN+Virtual
    value: 0.7742
    std: 0.0067
    paper_value: 0.7742
    paper_std: 0.0067
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7742
    true_std: 0.0067
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7742
    sort_std: 0.0067
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+Virtual
    model_key: gin+virtual
    model_plain: GIN+Virtual
    value: 0.7704
    std: 0.0083
    paper_value: 0.7704
    paper_std: 0.0083
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7704
    true_std: 0.0083
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7704
    sort_std: 0.0083
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+P-reg
    model_key: gcn+p-reg
    model_plain: GCN+P-reg
    value: 0.7586
    std: 0.0075
    paper_value: 0.7586
    paper_std: 0.0075
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7586
    true_std: 0.0075
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7586
    sort_std: 0.0075
    global_rank: 188
    paper_rank: 188
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+P-reg
    model_key: gin+p-reg
    model_plain: GIN+P-reg
    value: 0.749
    std: 0.0059
    paper_value: 0.749
    paper_std: 0.0059
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB graph classification task using standard split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.0059
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.0059
    global_rank: 232
    paper_rank: 232
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: ogbg-molhiv
  rows:
  - model: SigGate-GT
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: SigGate-GT
    value: 0.8476
    std: 0.0002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: Mixing pharmacophoric (FCFP) and structural (ECFP) fingerprints...
      GNNs contributing only 12%
    is_global_top: true
    global_rank: 1
    sort_value: 0.8476
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: hyperfusion
    model_plain: SigGate-GT
    value: 0.8475
    std: 0.0003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8475
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: pas+fps
    model_plain: SigGate-GT
    value: 0.842
    std: 0.0015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.842
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7547
    std: 0.0122
    paper_value: 0.7547
    paper_std: 0.0122
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.778
    true_std: 0.0182
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.023299999999999987
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0182
    global_rank: 120
    paper_rank: 240
    rank_delta: 120
    rank_delta_abs: 120
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+Virtual+P-reg
    model_key: gin+virtual+p-reg
    model_plain: GIN+Virtual+P-reg
    value: 0.7712
    std: 0.0114
    paper_value: 0.7712
    paper_std: 0.0114
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7712
    true_std: 0.0114
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7712
    sort_std: 0.0114
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
  - model: GIN+P-reg
    model_key: gin+p-reg
    model_plain: GIN+P-reg
    value: 0.7677
    std: 0.0141
    paper_value: 0.7677
    paper_std: 0.0141
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7677
    true_std: 0.0141
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7677
    sort_std: 0.0141
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
  - model: GIN+Virtual
    model_key: gin+virtual
    model_plain: GIN+Virtual
    value: 0.7633
    std: 0.0152
    paper_value: 0.7633
    paper_std: 0.0152
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7633
    true_std: 0.0152
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7633
    sort_std: 0.0152
    global_rank: 201
    paper_rank: 201
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
    value: 0.7608
    std: 0.0141
    paper_value: 0.7608
    paper_std: 0.0141
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.76
    at_pub_std: 0.012
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2022-08-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0008000000000000229
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.763
    true_std: 0.003
    value_gap_source_arxiv: '2208.04529'
    value_gap_source_title: Motif-based Graph Representation Learning with Application
      to Chemical Molecules
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.763
    sort_std: 0.003
    global_rank: 203
    paper_rank: 216
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+P-reg
    model_key: gcn+p-reg
    model_plain: GCN+P-reg
    value: 0.7603
    std: 0.0125
    paper_value: 0.7603
    paper_std: 0.0125
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7603
    true_std: 0.0125
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7603
    sort_std: 0.0125
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
  - model: GCN+Virtual+P-reg
    model_key: gcn+virtual+p-reg
    model_plain: GCN+Virtual+P-reg
    value: 0.7581
    std: 0.0161
    paper_value: 0.7581
    paper_std: 0.0161
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7581
    true_std: 0.0161
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7581
    sort_std: 0.0161
    global_rank: 227
    paper_rank: 227
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+Virtual
    model_key: gcn+virtual
    model_plain: GCN+Virtual
    value: 0.7567
    std: 0.0154
    paper_value: 0.7567
    paper_std: 0.0154
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Sep 4, 2020
    date_display: Sep 2020
    date_iso: '2020-09-04'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7567
    true_std: 0.0154
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7567
    sort_std: 0.0154
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
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
- benchmark: MoleculeNet
  datasets:
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
main_figure: /figures/2009.02027/main_figure.jpegoptim.jpg
---

