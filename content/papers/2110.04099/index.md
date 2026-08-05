---
title: Topology-Imbalance Learning for Semi-Supervised Node Classification
arxiv_id: '2110.04099'
source_url: ''
authors:
- name: Deli Chen
  orcid: null
  s2_author_id: '2111900876'
  s2_url: null
- name: Yankai Lin
  orcid: null
  s2_author_id: '2149202150'
  s2_url: null
- name: Guangxiang Zhao
  orcid: null
  s2_author_id: '1390788836'
  s2_url: null
- name: Xuancheng Ren
  orcid: null
  s2_author_id: '19169659'
  s2_url: null
- name: Peng Li
  orcid: null
  s2_author_id: '50492525'
  s2_url: null
- name: Jie Zhou
  orcid: null
  s2_author_id: '2108485135'
  s2_url: null
- name: Xu Sun
  orcid: null
  s2_author_id: '11774802'
  s2_url: null
published_date: Oct 8, 2021
published_date_iso: '2021-10-08'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: The class imbalance problem, as an important issue in learning node representations,
  has drawn increasing attention from the community. Although the imbalance considered
  by existing studies roots from the unequal quantity of labeled examples in different
  classes (quantity imbalance), we argue that graph data expose a unique source of
  imbalance from the asymmetric topological properties of the labeled nodes, i.e.,
  labeled nodes are not equal in terms of their structural role in the graph (topology
  imbalance). In this work, we first probe the previously unknown topology-imbalance
  issue, including its characteristics, causes, and threats to semi-supervised node
  classification learning. We then provide a unified view to jointly analyzing the
  quantity- and topology- imbalance issues by considering the node influence shift
  phenomenon with the Label Propagation algorithm. In light of our analysis, we devise
  an influence conflict detection--based metric Totoro to measure the degree of graph
  topology imbalance and propose a model-agnostic method ReNode to address the topology-imbalance
  issue by re-weighting the influence of labeled nodes adaptively based on their relative
  positions to class boundaries. Systematic experiments demonstrate the effectiveness
  and generalizability of our method in relieving topology-imbalance issue and promoting
  semi-supervised node classification. The further analysis unveils varied sensitivity
  of different graph neural networks (GNNs) to topology imbalance, which may serve
  as a new perspective in evaluating GNN architectures..
codebase_url: https://github.com/victorchen96/ReNode
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  dataset: Amazon-Computers
  rows:
  - model: PPNP w/ RN
    model_key: ppnp w/ rn
    model_plain: PPNP w/ RN
    value: 0.79
    std: 0.011
    paper_value: 0.79
    paper_std: 0.011
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.79
    true_std: 0.011
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: 0.011
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
  - model: GAT w/ RN
    model_key: gat w/ rn
    model_plain: GAT w/ RN
    value: 0.788
    std: 0.019
    paper_value: 0.788
    paper_std: 0.019
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.019
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.019
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC w/ RN
    model_key: sgc w/ rn
    model_plain: SGC w/ RN
    value: 0.782
    std: 0.018
    paper_value: 0.782
    paper_std: 0.018
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.018
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.018
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
  - model: SAGE w/ RN
    model_key: sage w/ rn
    model_plain: SAGE w/ RN
    value: 0.749
    std: 0.03
    paper_value: 0.749
    paper_std: 0.03
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.03
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.03
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN w/ RN
    model_key: gcn w/ rn
    model_plain: GCN w/ RN
    value: 0.747
    std: 0.022
    paper_value: 0.747
    paper_std: 0.022
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.747
    true_std: 0.022
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.747
    sort_std: 0.022
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CHEB w/ RN
    model_key: cheb w/ rn
    model_plain: CHEB w/ RN
    value: 0.705
    std: 0.04
    paper_value: 0.705
    paper_std: 0.04
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.705
    true_std: 0.04
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.705
    sort_std: 0.04
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Weighted-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Weighted-F1
  metric: Weighted-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Amazon-Photo
  rows:
  - model: PPNP w/ RN
    model_key: ppnp w/ rn
    model_plain: PPNP w/ RN
    value: 0.897
    std: 0.01
    paper_value: 0.897
    paper_std: 0.01
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: 0.01
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: 0.01
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
  - model: GAT w/ RN
    model_key: gat w/ rn
    model_plain: GAT w/ RN
    value: 0.891
    std: 0.02
    paper_value: 0.891
    paper_std: 0.02
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.891
    true_std: 0.02
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.02
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN w/ RN
    model_key: gcn w/ rn
    model_plain: GCN w/ RN
    value: 0.877
    std: 0.002
    paper_value: 0.877
    paper_std: 0.002
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.877
    true_std: 0.002
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: 0.002
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
  - model: SGC w/ RN
    model_key: sgc w/ rn
    model_plain: SGC w/ RN
    value: 0.874
    std: 0.015
    paper_value: 0.874
    paper_std: 0.015
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.874
    true_std: 0.015
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.874
    sort_std: 0.015
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAGE w/ RN
    model_key: sage w/ rn
    model_plain: SAGE w/ RN
    value: 0.865
    std: 0.017
    paper_value: 0.865
    paper_std: 0.017
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.865
    true_std: 0.017
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.017
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CHEB w/ RN
    model_key: cheb w/ rn
    model_plain: CHEB w/ RN
    value: 0.848
    std: 0.024
    paper_value: 0.848
    paper_std: 0.024
    metric: Weighted-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Pure topology-imbalance issue evaluation
    date: Oct 8, 2021
    date_display: Oct 2021
    date_iso: '2021-10-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.848
    true_std: 0.024
    value_gap_source_arxiv: '2110.04099'
    value_gap_source_title: Topology-Imbalance Learning for Semi-Supervised Node Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.848
    sort_std: 0.024
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Weighted-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Weighted-F1
  metric: Weighted-F1
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
main_figure: /figures/2110.04099/main_figure.jpegoptim.jpg
---

