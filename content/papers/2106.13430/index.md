---
title: Subgraph Federated Learning with Missing Neighbor Generation
arxiv_id: '2106.13430'
source_url: ''
authors:
- name: Ke Zhang
  orcid: null
  s2_author_id: '2119059495'
  s2_url: null
- name: Carl Yang
  orcid: null
  s2_author_id: '1390553618'
  s2_url: null
- name: Xiaoxiao Li
  orcid: null
  s2_author_id: '2144456293'
  s2_url: null
- name: Lichao Sun
  orcid: null
  s2_author_id: '49755259'
  s2_url: null
- name: S. Yiu
  orcid: null
  s2_author_id: '145964453'
  s2_url: null
published_date: Jun 25, 2021
published_date_iso: '2021-06-25'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Graphs have been widely used in data mining and machine learning due to
  their unique representation of real-world objects and their interactions. As graphs
  are getting bigger and bigger nowadays, it is common to see their subgraphs separately
  collected and stored in multiple local systems. Therefore, it is natural to consider
  the subgraph federated learning setting, where each local system holds a small subgraph
  that may be biased from the distribution of the whole graph. Hence, the subgraph
  federated learning aims to collaboratively train a powerful and generalizable graph
  mining model without directly sharing their graph data. In this work, towards the
  novel yet realistic setting of subgraph federated learning, we propose two major
  techniques: (1) FedSage, which trains a GraphSage model based on FedAvg to integrate
  node features, link structures, and task labels on multiple local subgraphs; (2)
  FedSage+, which trains a missing neighbor generator along FedSage to deal with missing
  links across local subgraphs. Empirical results on four real-world graph datasets
  with synthesized subgraph federated learning settings demonstrate the effectiveness
  and efficiency of our proposed techniques. At the same time, consistent theoretical
  implications are made towards their generalization ability on the global graphs.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- FedSage
- FedSage with globally shared NeighGen
mrr: 0.0042
adjusted_mrr: 0.0014
mrr_dataset_count: 1
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
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
  - model: FedSage
    model_key: fedsage
    model_plain: FedSage
    value: 0.7454
    std: 0.0038
    paper_value: 0.7454
    paper_std: 0.0038
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using the Planetoid split (fixed split) as
      per canonical task definition.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7454
    true_std: 0.0038
    value_gap_source_arxiv: '2106.13430'
    value_gap_source_title: Subgraph Federated Learning with Missing Neighbor Generation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7454
    sort_std: 0.0038
    global_rank: 239
    paper_rank: 239
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FedSage with globally shared NeighGen
    model_key: fedsage with globally shared neighgen
    model_plain: FedSage with globally shared NeighGen
    value: 0.7326
    std: 0.0055
    paper_value: 0.7326
    paper_std: 0.0055
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using the Planetoid split (fixed split) as
      per canonical task definition.
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-06-25'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7326
    true_std: 0.0055
    value_gap_source_arxiv: '2106.13430'
    value_gap_source_title: Subgraph Federated Learning with Missing Neighbor Generation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7326
    sort_std: 0.0055
    global_rank: 343
    paper_rank: 343
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: CiteSeer
      dataset_slug: citeseer
main_figure: /figures/2106.13430/main_figure.jpegoptim.jpg
---

