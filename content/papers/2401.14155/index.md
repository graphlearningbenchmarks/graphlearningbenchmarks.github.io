---
title: Alleviating Structural Distribution Shift in Graph Anomaly Detection
arxiv_id: '2401.14155'
source_url: ''
authors:
- name: Yuan Gao
  orcid: null
  s2_author_id: '143792907'
  s2_url: null
- name: Xiang Wang
  orcid: null
  s2_author_id: '2144796537'
  s2_url: null
- name: Xiangnan He
  orcid: null
  s2_author_id: '7792071'
  s2_url: null
- name: Zhenguang Liu
  orcid: null
  s2_author_id: '2145312301'
  s2_url: null
- name: Huamin Feng
  orcid: null
  s2_author_id: '1986484'
  s2_url: null
- name: Yongdong Zhang
  orcid: null
  s2_author_id: '2164724337'
  s2_url: null
published_date: Feb 27, 2023
published_date_iso: '2023-02-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph anomaly detection (GAD) is a challenging binary classification problem
  due to its different structural distribution between anomalies and normal nodes
  --- abnormal nodes are a minority, therefore holding high heterophily and low homophily
  compared to normal nodes. Furthermore, due to various time factors and the annotation
  preferences of human experts, the heterophily and homophily can change across training
  and testing data, which is called structural distribution shift (SDS) in this paper.
  The mainstream methods are built on graph neural networks (GNNs), benefiting the
  classification of normals from aggregating homophilous neighbors, yet ignoring the
  SDS issue for anomalies and suffering from poor generalization. This work solves
  the problem from a feature view. We observe that the degree of SDS varies between
  anomalies and normal nodes. Hence to address the issue, the key lies in resisting
  high heterophily for anomalies meanwhile benefiting the learning of normals from
  homophily. Since different labels correspond to the difference of critical anomaly
  features which make great contributions to the GAD, we tease out the anomaly features
  on which we constrain to mitigate the effect of heterophilous neighbors and make
  them invariant. However, the prior distribution of anomaly features is dynamic and
  hard to estimate, we thus devise a prototype vector to infer and update this distribution
  during training. For normal nodes, we constrain the remaining features to preserve
  the connectivity of nodes and reinforce the influence of the homophilous neighborhood.
  We term our proposed framework as Graph Decomposition Network (GDN). Extensive experiments
  are conducted on two benchmark datasets, and the proposed framework achieves a remarkable
  performance boost in GAD, especially in an SDS environment where anomalies have
  largely different structural distribution across training and testing environments.
  Codes are open-sourced in.
codebase_url: https://github.com/blacksingular/wsdm_GDN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon2M
  rows:
  - model: GraphConsis
    model_key: gfd
    model_plain: GraphConsis
    value: 0.9757
    std: 0.0012
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9757
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphConsis
    model_key: bwgnn
    model_plain: GraphConsis
    value: 0.9742
    std: 0.0048
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9742
    sort_std: 0.0048
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphConsis
    model_key: gdn
    model_plain: GraphConsis
    value: 0.9709
    std: 0.0016
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9709
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+GDN
    model_key: gcn+gdn
    model_plain: GCN+GDN
    value: 0.8904
    std: null
    paper_value: 0.8904
    paper_std: null
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard AUC evaluation on Amazon dataset as per Table 2 caption.
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8904
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8667
    std: null
    paper_value: 0.8667
    paper_std: null
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard AUC evaluation on Amazon dataset as per Table 2 caption.
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.911
    at_pub_std: 0.006
    at_pub_source_arxiv: '2104.07477'
    at_pub_source_title: Lorentzian Graph Convolutional Networks
    at_pub_source_date_iso: '2021-04-15'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.044300000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8667
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8667
    sort_std: null
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Lorentzian Graph Convolutional Networks
    comparison_source_arxiv: '2104.07477'
    is_best: false
    is_std_outlier: false
  - model: SAGE+GDN
    model_key: sage+gdn
    model_plain: SAGE+GDN
    value: 0.8216
    std: null
    paper_value: 0.8216
    paper_std: null
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard AUC evaluation on Amazon dataset as per Table 2 caption.
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8216
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: null
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7535
    std: null
    paper_value: 0.7535
    paper_std: null
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard AUC evaluation on Amazon dataset as per Table 2 caption.
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7535
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7535
    sort_std: null
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
---

