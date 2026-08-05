---
title: 'GaGSL: Global-augmented Graph Structure Learning via Graph Information Bottleneck'
arxiv_id: '2411.04356'
source_url: ''
authors:
- name: Shuangjie Li
  orcid: null
  s2_author_id: '2292577917'
  s2_url: null
- name: Jia Song
  orcid: null
  s2_author_id: '2314575441'
  s2_url: null
- name: Baoming Zhang
  orcid: null
  s2_author_id: '2118875037'
  s2_url: null
- name: Gaoli Ruan
  orcid: null
  s2_author_id: '2329369885'
  s2_url: null
- name: Junyuan Xie
  orcid: null
  s2_author_id: '2329717304'
  s2_url: null
- name: Chongjun Wang
  orcid: null
  s2_author_id: '2292665107'
  s2_url: null
published_date: Nov 7, 2024
published_date_iso: '2024-11-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) are prominent for their effectiveness in processing
  graph data for semi-supervised node classification tasks. Most works of GNNs assume
  that the observed structure accurately represents the underlying node relationships.
  However, the graph structure is inevitably noisy or incomplete in reality, which
  can degrade the quality of graph representations. Therefore, it is imperative to
  learn a clean graph structure that balances performance and robustness. In this
  paper, we propose a novel method named Global-augmented Graph Structure Learning
  (GaGSL), guided by the Graph Information Bottleneck (GIB) principle. The key idea
  behind GaGSL is to learn a compact and informative graph structure for node classification
  tasks. Specifically, to mitigate the bias caused by relying solely on the original
  structure, we first obtain augmented features and augmented structure through global
  feature augmentation and global structure augmentation. We then input the augmented
  features and augmented structure into a structure estimator with different parameters
  for optimization and re-definition of the graph structure, respectively. The redefined
  structures are combined to form the final graph structure. Finally, we employ GIB
  based on mutual information to guide the optimization of the graph structure to
  obtain the minimum sufficient graph structure. Comprehensive evaluations across
  a range of datasets reveal the outstanding performance and robustness of GaGSL compared
  with the state-of-the-art methods.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GaGSL
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
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
- &id002
  dataset: CiteSeer
  is_multi_metric: true
  rows:
  - model: IDGL
    model_key: idgl
    model_plain: IDGL
    metric_values:
    - null
    - 0.914
    - 0.694
    - 0.719
    metric_stds:
    - null
    - 0.004
    - 0.004
    - 0.003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.914
    sort_std: 0.004
    true_value: 0.914
    true_std: 0.004
    paper_value: 0.914
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: GaGSL
    model_key: gagsl
    model_plain: GaGSL
    metric_values:
    - null
    - 0.906
    - 0.688
    - 0.721
    metric_stds:
    - null
    - 0.005
    - 0.009
    - 0.011
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.906
    sort_std: 0.005
    true_value: 0.906
    true_std: 0.005
    paper_value: 0.906
    paper_std: 0.005
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: GEN
    model_key: gen
    model_plain: GEN
    metric_values:
    - null
    - 0.901
    - 0.694
    - 0.727
    metric_stds:
    - null
    - 0.017
    - 0.014
    - 0.013
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.901
    sort_std: 0.017
    true_value: 0.901
    true_std: 0.017
    paper_value: 0.901
    paper_std: 0.017
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: SGC
    model_key: sgc
    model_plain: SGC
    metric_values:
    - null
    - 0.899
    - 0.664
    - 0.706
    metric_stds:
    - null
    - 0.002
    - 0.005
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.899
    sort_std: 0.002
    true_value: 0.899
    true_std: 0.002
    paper_value: 0.899
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - null
    - 0.894
    - 0.633
    - 0.662
    metric_stds:
    - null
    - 0.002
    - 0.012
    - 0.012
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.894
    sort_std: 0.002
    true_value: 0.894
    true_std: 0.002
    paper_value: 0.894
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: PRI-GSL
    model_key: pri-gsl
    model_plain: PRI-GSL
    metric_values:
    - null
    - 0.886
    - 0.645
    - 0.676
    metric_stds:
    - null
    - 0.002
    - 0.004
    - 0.006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.886
    sort_std: 0.002
    true_value: 0.886
    true_std: 0.002
    paper_value: 0.886
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: Pro-GNN
    model_key: pro-gnn
    model_plain: Pro-GNN
    metric_values:
    - null
    - 0.885
    - 0.631
    - 0.656
    metric_stds:
    - null
    - 0.003
    - 0.007
    - 0.008
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.885
    sort_std: 0.003
    true_value: 0.885
    true_std: 0.003
    paper_value: 0.885
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.875
    - 0.632
    - 0.671
    metric_stds:
    - null
    - 0.012
    - 0.004
    - 0.003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.875
    sort_std: 0.012
    true_value: 0.875
    true_std: 0.012
    paper_value: 0.875
    paper_std: 0.012
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  metrics:
  - Accuracy
  - AUC
  - F1-macro
  - F1-micro
  primary_metric: Accuracy
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  - F1-macro
  - F1-micro
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Cora
  is_multi_metric: true
  rows:
  - model: GaGSL
    model_key: gagsl
    model_plain: GaGSL
    metric_values:
    - null
    - 0.973
    - 0.823
    - 0.838
    metric_stds:
    - null
    - 0.003
    - 0.011
    - 0.012
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.973
    sort_std: 0.003
    true_value: 0.973
    true_std: 0.003
    paper_value: 0.973
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: IDGL
    model_key: idgl
    model_plain: IDGL
    metric_values:
    - null
    - 0.97
    - 0.804
    - 0.822
    metric_stds:
    - null
    - 0.003
    - 0.013
    - 0.026
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.97
    sort_std: 0.003
    true_value: 0.97
    true_std: 0.003
    paper_value: 0.97
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: Pro-GNN
    model_key: pro-gnn
    model_plain: Pro-GNN
    metric_values:
    - null
    - 0.969
    - 0.788
    - 0.798
    metric_stds:
    - null
    - 0.009
    - 0.026
    - 0.026
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.969
    sort_std: 0.009
    true_value: 0.969
    true_std: 0.009
    paper_value: 0.969
    paper_std: 0.009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: SGC
    model_key: sgc
    model_plain: SGC
    metric_values:
    - null
    - 0.961
    - 0.784
    - 0.794
    metric_stds:
    - null
    - 0.001
    - 0.002
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.961
    sort_std: 0.001
    true_value: 0.961
    true_std: 0.001
    paper_value: 0.961
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: PRI-GSL
    model_key: pri-gsl
    model_plain: PRI-GSL
    metric_values:
    - null
    - 0.958
    - 0.75
    - 0.767
    metric_stds:
    - null
    - 0.003
    - 0.004
    - 0.007
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.958
    sort_std: 0.003
    true_value: 0.958
    true_std: 0.003
    paper_value: 0.958
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: GEN
    model_key: gen
    model_plain: GEN
    metric_values:
    - null
    - 0.94
    - 0.801
    - 0.914
    metric_stds:
    - null
    - 0.019
    - 0.013
    - 0.02
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.94
    sort_std: 0.019
    true_value: 0.94
    true_std: 0.019
    paper_value: 0.94
    paper_std: 0.019
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.937
    - 0.743
    - 0.751
    metric_stds:
    - null
    - 0.007
    - 0.018
    - 0.023
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.937
    sort_std: 0.007
    true_value: 0.937
    true_std: 0.007
    paper_value: 0.937
    paper_std: 0.007
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - null
    - 0.925
    - 0.703
    - 0.714
    metric_stds:
    - null
    - 0.007
    - 0.009
    - 0.011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.925
    sort_std: 0.007
    true_value: 0.925
    true_std: 0.007
    paper_value: 0.925
    paper_std: 0.007
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2411.04356'
    value_gap_source_title: 'GaGSL: Global-augmented Graph Structure Learning via
      Graph Information Bottleneck'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-07'
    value_gap_source_date_label: '2024'
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
    published_venue: ''
    date: Nov 7, 2024
    date_display: Nov 2024
    date_iso: '2024-11-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  metrics:
  - Accuracy
  - AUC
  - F1-macro
  - F1-micro
  primary_metric: Accuracy
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  - F1-macro
  - F1-micro
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: CiteSeer
      dataset_slug: citeseer
single_proposed_model: GaGSL
main_figure: /figures/2411.04356/main_figure.jpegoptim.jpg
---

