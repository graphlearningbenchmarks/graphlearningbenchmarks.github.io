---
title: Partitioning Message Passing for Graph Fraud Detection
arxiv_id: '2412.00020'
source_url: ''
authors:
- name: Wei Zhuo
  orcid: null
  s2_author_id: '2301927164'
  s2_url: null
- name: Zemin Liu
  orcid: null
  s2_author_id: '2253842540'
  s2_url: null
- name: Bryan Hooi
  orcid: null
  s2_author_id: '2313619173'
  s2_url: null
- name: Bingsheng He
  orcid: null
  s2_author_id: '2261324804'
  s2_url: null
- name: Guang Tan
  orcid: null
  s2_author_id: '2146720616'
  s2_url: null
- name: Rizal Fathony
  orcid: null
  s2_author_id: '7320311'
  s2_url: null
- name: Jia Chen
  orcid: null
  s2_author_id: '2313689306'
  s2_url: null
published_date: Nov 16, 2024
published_date_iso: '2024-11-16'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Label imbalance and homophily-heterophily mixture are the fundamental problems
  encountered when applying Graph Neural Networks (GNNs) to Graph Fraud Detection
  (GFD) tasks. Existing GNN-based GFD models are designed to augment graph structure
  to accommodate the inductive bias of GNNs towards homophily, by excluding heterophilic
  neighbors during message passing. In our work, we argue that the key to applying
  GNNs for GFD is not to exclude but to distinguish neighbors with different labels.
  Grounded in this perspective, we introduce Partitioning Message Passing (PMP), an
  intuitive yet effective message passing paradigm expressly crafted for GFD. Specifically,
  in the neighbor aggregation stage of PMP, neighbors with different classes are aggregated
  with distinct node-specific aggregation functions. By this means, the center node
  can adaptively adjust the information aggregated from its heterophilic and homophilic
  neighbors, thus avoiding the model gradient being dominated by benign nodes which
  occupy the majority of the population. We theoretically establish a connection between
  the spatial formulation of PMP and spectral analysis to characterize that PMP operates
  an adaptive node-specific spectral graph filter, which demonstrates the capability
  of PMP to handle heterophily-homophily mixed graphs. Extensive experimental results
  show that PMP can significantly boost the performance on GFD tasks. Our code is
  available at.
codebase_url: https://github.com/Xtra-Computing/PMP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GFD
mrr: 0.0
adjusted_mrr: 0.0
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
  - model: GFD
    model_key: gfd
    model_plain: GFD
    value: 0.9757
    std: 0.0012
    paper_value: 0.9757
    paper_std: 0.0012
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9757
    true_std: 0.0012
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9757
    sort_std: 0.0012
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
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.9742
    std: 0.0048
    paper_value: 0.9742
    paper_std: 0.0048
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
    table_ref: Table 1
    source_ref: tang2022rethinking
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9742
    true_std: 0.0048
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9742
    sort_std: 0.0048
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
  - model: GDN
    model_key: gdn
    model_plain: GDN
    value: 0.9709
    std: 0.0016
    paper_value: 0.9709
    paper_std: 0.0016
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
    table_ref: Table 1
    source_ref: gao2023alleviating
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9709
    true_std: 0.0016
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9709
    sort_std: 0.0016
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
  - model: GHRN
    model_key: ghrn
    model_plain: GHRN
    value: 0.9707
    std: 0.0073
    paper_value: 0.9707
    paper_std: 0.0073
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
    table_ref: Table 1
    source_ref: gao2023ghrn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9707
    true_std: 0.0073
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9707
    sort_std: 0.0073
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
  - model: H2-FDetector
    model_key: h2-fdetector
    model_plain: H2-FDetector
    value: 0.9603
    std: 0.0069
    paper_value: 0.9603
    paper_std: 0.0069
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
    table_ref: Table 1
    source_ref: h2fdetector_webconf22
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9603
    true_std: 0.0069
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9603
    sort_std: 0.0069
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
  - model: PC-GNN
    model_key: pc-gnn
    model_plain: PC-GNN
    value: 0.9586
    std: 0.0014
    paper_value: 0.9586
    paper_std: 0.0014
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
    table_ref: Table 1
    source_ref: liu2021pick
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9586
    true_std: 0.0014
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9586
    sort_std: 0.0014
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.95
    std: 0.0081
    paper_value: 0.95
    paper_std: 0.0081
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
    table_ref: Table 1
    source_ref: bo2021beyond
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.95
    true_std: 0.0081
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: 0.0081
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.9372
    std: 0.0068
    paper_value: 0.9372
    paper_std: 0.0068
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
    table_ref: Table 1
    source_ref: chien2021adaptive
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9372
    true_std: 0.0068
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9372
    sort_std: 0.0068
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9316
    std: 0.0087
    paper_value: 0.9316
    paper_std: 0.0087
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
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.904
    at_pub_std: 0.003
    at_pub_source_arxiv: '2104.07477'
    at_pub_source_title: Lorentzian Graph Convolutional Networks
    at_pub_source_date_iso: '2021-04-15'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.027599999999999958
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9316
    true_std: 0.0087
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9316
    sort_std: 0.0087
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Lorentzian Graph Convolutional Networks
    comparison_source_arxiv: '2104.07477'
    is_best: false
    is_std_outlier: false
  - model: CARE-GNN
    model_key: care-gnn
    model_plain: CARE-GNN
    value: 0.9067
    std: 0.0149
    paper_value: 0.9067
    paper_std: 0.0149
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
    table_ref: Table 1
    source_ref: dou2020enhancing
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.8973
    at_pub_std: null
    at_pub_source_arxiv: '2008.08692'
    at_pub_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    at_pub_source_date_iso: '2020-08-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.009399999999999964
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9067
    true_std: 0.0149
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9067
    sort_std: 0.0149
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8369
    std: 0.0125
    paper_value: 0.8369
    paper_std: 0.0125
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
    table_ref: Table 1
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.911
    at_pub_std: 0.006
    at_pub_source_arxiv: '2104.07477'
    at_pub_source_title: Lorentzian Graph Convolutional Networks
    at_pub_source_date_iso: '2021-04-15'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07410000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8667
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.02980000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8667
    sort_std: null
    global_rank: 15
    paper_rank: 16
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Lorentzian Graph Convolutional Networks
    comparison_source_arxiv: '2104.07477'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8102
    std: 0.0179
    paper_value: 0.8102
    paper_std: 0.0179
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
    table_ref: Table 1
    source_ref: velickovic2018graph
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 40% training ratio supervised setting
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.913
    at_pub_std: 0.006
    at_pub_source_arxiv: '2104.07477'
    at_pub_source_title: Lorentzian Graph Convolutional Networks
    at_pub_source_date_iso: '2021-04-15'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1028
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8102
    true_std: 0.0179
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8102
    sort_std: 0.0179
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Lorentzian Graph Convolutional Networks
    comparison_source_arxiv: '2104.07477'
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
single_proposed_model: GFD
---

