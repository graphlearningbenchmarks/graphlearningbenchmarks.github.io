---
title: 'Redesigning graph filter-based GNNs to relax the homophily assumption This
  work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00, PID2023-149457OB-I00,
  FPU20/05554, the Community of Madrid (Madrid ELLIS Unit), and the NSF under award
  CCF-2340481. Research was sponsored by the Army Research Office and was accomplished
  under Grant Number W911NF-17-S-0002. The views and conclusions contained in this
  document are those of the authors and should not be interpreted as representing
  the official policies, either expressed or implied, of the Army Research Office
  or the U.S. Army or the U.S. Government. The U.S. Government is authorized to reproduce
  and distribute reprints for Government purposes notwithstanding any copyright notation
  herein. Emails: samuel.rey.escudero@urjc.es, nav@rice.edu, victor.tenorio@urjc.es,
  segarra@rice.edu, antonio.garcia.marques@urjc.es'
arxiv_id: '2409.08676'
source_url: ''
authors:
- name: Samuel Rey
  orcid: null
  s2_author_id: '1605975703'
  s2_url: null
- name: Madeline Navarro
  orcid: null
  s2_author_id: '1936823928'
  s2_url: null
- name: Victor M. Tenorio
  orcid: null
  s2_author_id: '2058351334'
  s2_url: null
- name: Santiago Segarra
  orcid: null
  s2_author_id: '2239197971'
  s2_url: null
- name: Antonio G. Marques
  orcid: null
  s2_author_id: '2241339650'
  s2_url: null
published_date: Sep 13, 2024
published_date_iso: '2024-09-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) have become a workhorse approach for learning
  from data defined over irregular domains, typically by implicitly assuming that
  the data structure is represented by a homophilic graph. However, recent works have
  revealed that many relevant applications involve heterophilic data where the performance
  of GNNs can be notably compromised. To address this challenge, we present a simple
  yet effective architecture designed to mitigate the limitations of the homophily
  assumption. The proposed architecture reinterprets the role of graph filters in
  convolutional GNNs, resulting in a more general architecture while incorporating
  a stronger inductive bias than GNNs based on filter banks. The proposed convolutional
  layer enhances the expressive capacity of the architecture enabling it to learn
  from both homophilic and heterophilic data and preventing the issue of oversmoothing.
  From a theoretical standpoint, we show that the proposed architecture is permutation
  equivariant. Finally, we show that the proposed GNNs compares favorably relative
  to several state-of-the-art baselines in both homophilic and heterophilic datasets,
  showcasing its promising potential.
codebase_url: https://github.com/reysam93/adaptive_agg_gcn
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AAGCN
- AAGCN-N_A
- AAGCN-N_H
mrr: 0.004
adjusted_mrr: 0.0027
mrr_dataset_count: 2
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Cornell
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.948
    std: 0.038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/AaltoML/heterophily-imp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.948
    sort_std: 0.038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9429
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.754
    std: 0.056
    paper_value: 0.754
    paper_std: 0.056
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9136
    at_pub_std: 0.007
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15959999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9136
    true_std: 0.007
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.15959999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 27
    paper_rank: 292
    rank_delta: 265
    rank_delta_abs: 265
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.646
    std: 0.063
    paper_value: 0.646
    paper_std: 0.063
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
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: 0.061
    at_pub_source_arxiv: '2102.11391'
    at_pub_source_title: 'MagNet: A Neural Network for Directed Graphs'
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15400000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8269
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.18089999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8269
    sort_std: null
    global_rank: 177
    paper_rank: 409
    rank_delta: 232
    rank_delta_abs: 232
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MagNet: A Neural Network for Directed Graphs'
    comparison_source_arxiv: '2102.11391'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8196
    std: 0.0739
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 200
    sort_value: 0.8196
    sort_std: 0.0739
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.549
    std: 0.047
    paper_value: 0.549
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
    table_ref: Table 1
    source_ref: velivckovic2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.819
    at_pub_std: 0.054
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2699999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: 0.054
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2699999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.054
    global_rank: 201
    paper_rank: 517
    rank_delta: 316
    rank_delta_abs: 316
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.389
    std: 0.095
    paper_value: 0.389
    paper_std: 0.095
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8015
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2405.16185'
    at_pub_source_title: Differentiable Cluster Graph Neural Network
    at_pub_source_date_iso: '2024-05-25'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-07-01'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.4125
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8082
    true_std: 0.036
    value_gap_source_arxiv: '2602.05358'
    value_gap_source_title: Bayesian Neighborhood Adaptation for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.4192
    has_value_note: false
    value_note: ''
    sort_value: 0.8082
    sort_std: 0.036
    global_rank: 217
    paper_rank: 651
    rank_delta: 434
    rank_delta_abs: 434
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Differentiable Cluster Graph Neural Network
    comparison_source_arxiv: '2405.16185'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.446
    std: 0.085
    paper_value: 0.446
    paper_std: 0.085
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
    table_ref: Table 1
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.78
    at_pub_std: 0.019
    at_pub_source_arxiv: '2309.02769'
    at_pub_source_title: 'Unifying over-smoothing and over-squashing in graph neural
      networks: A physics informed approach and beyond'
    at_pub_source_date_iso: '2023-09-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.334
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.78
    true_std: 0.019
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.334
    has_value_note: false
    value_note: ''
    sort_value: 0.78
    sort_std: 0.019
    global_rank: 257
    paper_rank: 622
    rank_delta: 365
    rank_delta_abs: 365
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unifying over-smoothing and over-squashing in graph
      neural networks: A physics informed approach and beyond'
    comparison_source_arxiv: '2309.02769'
    is_best: false
    is_std_outlier: false
  - model: AAGCN
    model_key: aagcn
    model_plain: AAGCN
    value: 0.776
    std: 0.068
    paper_value: 0.776
    paper_std: 0.068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.776
    true_std: 0.068
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.776
    sort_std: 0.068
    global_rank: 264
    paper_rank: 264
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AAGCN-N_H
    model_key: aagcn-n_h
    model_plain: AAGCN-N_H
    value: 0.773
    std: 0.044
    paper_value: 0.773
    paper_std: 0.044
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.773
    true_std: 0.044
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.773
    sort_std: 0.044
    global_rank: 272
    paper_rank: 272
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AAGCN-N_A
    model_key: aagcn-n_a
    model_plain: AAGCN-N_A
    value: 0.762
    std: 0.034
    paper_value: 0.762
    paper_std: 0.034
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.762
    true_std: 0.034
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.034
    global_rank: 286
    paper_rank: 286
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FB-GCN-N_A
    model_key: fb-gcn-n_a
    model_plain: FB-GCN-N_A
    value: 0.751
    std: 0.043
    paper_value: 0.751
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
    table_ref: Table 1
    source_ref: ruiz2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.751
    true_std: 0.043
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: 0.043
    global_rank: 299
    paper_rank: 299
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FB-GCN
    model_key: fb-gcn
    model_plain: FB-GCN
    value: 0.743
    std: 0.044
    paper_value: 0.743
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
    table_ref: Table 1
    source_ref: ruiz2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6216
    at_pub_std: 0.0946
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12139999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.743
    true_std: 0.044
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.044
    global_rank: 311
    paper_rank: 311
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-N_A
    model_key: gcn-n_a
    model_plain: GCN-N_A
    value: 0.411
    std: 0.051
    paper_value: 0.411
    paper_std: 0.051
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph split.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.411
    true_std: 0.051
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.411
    sort_std: 0.051
    global_rank: 643
    paper_rank: 643
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
  dataset: Texas
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.814
    std: 0.057
    paper_value: 0.814
    paper_std: 0.057
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.923
    at_pub_std: 0.007
    at_pub_source_arxiv: '2401.14580'
    at_pub_source_title: 'Design your own universe: a physics-informed agnostic method
      for enhancing graph neural networks'
    at_pub_source_date_iso: '2024-01-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1090000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.007
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.1090000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.007
    global_rank: 47
    paper_rank: 295
    rank_delta: 248
    rank_delta_abs: 248
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    comparison_source_arxiv: '2401.14580'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9001
    std: 0.023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 76
    sort_value: 0.9001
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AAGCN-N_H
    model_key: aagcn-n_h
    model_plain: AAGCN-N_H
    value: 0.857
    std: 0.051
    paper_value: 0.857
    paper_std: 0.051
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.857
    true_std: 0.051
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.857
    sort_std: 0.051
    global_rank: 174
    paper_rank: 174
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AAGCN-N_A
    model_key: aagcn-n_a
    model_plain: AAGCN-N_A
    value: 0.855
    std: 0.051
    paper_value: 0.855
    paper_std: 0.051
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.855
    true_std: 0.051
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.855
    sort_std: 0.051
    global_rank: 181
    paper_rank: 181
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
    value: 0.784
    std: 0.042
    paper_value: 0.784
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
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.843
    at_pub_std: 0.055
    at_pub_source_arxiv: '2102.11391'
    at_pub_source_title: 'MagNet: A Neural Network for Directed Graphs'
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.05899999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.843
    true_std: 0.055
    value_gap_source_arxiv: '2102.11391'
    value_gap_source_title: 'MagNet: A Neural Network for Directed Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.05899999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.843
    sort_std: 0.055
    global_rank: 224
    paper_rank: 358
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AAGCN
    model_key: aagcn
    model_plain: AAGCN
    value: 0.838
    std: 0.055
    paper_value: 0.838
    paper_std: 0.055
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.838
    true_std: 0.055
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.838
    sort_std: 0.055
    global_rank: 235
    paper_rank: 235
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
    value: 0.643
    std: 0.063
    paper_value: 0.643
    paper_std: 0.063
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
    table_ref: Table 1
    source_ref: velivckovic2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: 0.0311
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15700000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.0645
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.17320000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.0645
    global_rank: 288
    paper_rank: 572
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: FB-GCN-N_A
    model_key: fb-gcn-n_a
    model_plain: FB-GCN-N_A
    value: 0.797
    std: 0.022
    paper_value: 0.797
    paper_std: 0.022
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
    table_ref: Table 1
    source_ref: ruiz2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.797
    true_std: 0.022
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.022
    global_rank: 338
    paper_rank: 338
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
    value: 0.576
    std: 0.048
    paper_value: 0.576
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7869
    at_pub_std: 0.0647
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.2109000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7933
    true_std: 0.0447
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.21730000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0447
    global_rank: 348
    paper_rank: 675
    rank_delta: 327
    rank_delta_abs: 327
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: FB-GCN
    model_key: fb-gcn
    model_plain: FB-GCN
    value: 0.757
    std: 0.048
    paper_value: 0.757
    paper_std: 0.048
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
    table_ref: Table 1
    source_ref: ruiz2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6216
    at_pub_std: 0.1
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.13539999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.757
    true_std: 0.048
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.757
    sort_std: 0.048
    global_rank: 412
    paper_rank: 412
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.649
    std: 0.055
    paper_value: 0.649
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.746
    at_pub_std: 0.008
    at_pub_source_arxiv: '2309.02769'
    at_pub_source_title: 'Unifying over-smoothing and over-squashing in graph neural
      networks: A physics informed approach and beyond'
    at_pub_source_date_iso: '2023-09-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.746
    true_std: 0.008
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.09699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.008
    global_rank: 435
    paper_rank: 561
    rank_delta: 126
    rank_delta_abs: 126
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unifying over-smoothing and over-squashing in graph
      neural networks: A physics informed approach and beyond'
    comparison_source_arxiv: '2309.02769'
    is_best: false
    is_std_outlier: false
  - model: GCN-N_A
    model_key: gcn-n_a
    model_plain: GCN-N_A
    value: 0.592
    std: 0.055
    paper_value: 0.592
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic WebKB subgraph.
    date: Sep 13, 2024
    date_display: Sep 2024
    date_iso: '2024-09-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.055
    value_gap_source_arxiv: '2409.08676'
    value_gap_source_title: 'Redesigning graph filter-based GNNs to relax the homophily
      assumption This work was supported in part by the Spanish AEI Grants PID2022-136887NB-I00,
      PID2023-149457OB-I00, FPU20/05554, the Community of Madrid (Madrid ELLIS Unit),
      and the NSF under award CCF-2340481. Research was sponsored by the Army Research
      Office and was accomplished under Grant Number W911NF-17-S-0002. The views and
      conclusions contained in this document are those of the authors and should not
      be interpreted as representing the official policies, either expressed or implied,
      of the Army Research Office or the U.S. Army or the U.S. Government. The U.S.
      Government is authorized to reproduce and distribute reprints for Government
      purposes notwithstanding any copyright notation herein. Emails: samuel.rey.escudero@urjc.es,
      nav@rice.edu, victor.tenorio@urjc.es, segarra@rice.edu, antonio.garcia.marques@urjc.es'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.055
    global_rank: 649
    paper_rank: 649
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
main_figure: /figures/2409.08676/main_figure.jpegoptim.jpg
---

