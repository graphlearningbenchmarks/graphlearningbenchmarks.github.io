---
title: Learning Graph-Level Representation for Drug Discovery
arxiv_id: '1709.03741'
source_url: ''
authors:
- name: Junying Li
  orcid: null
  s2_author_id: '2108934075'
  s2_url: null
- name: Deng Cai
  orcid: null
  s2_author_id: '1724421'
  s2_url: null
- name: Xiaofei He
  orcid: null
  s2_author_id: '3945955'
  s2_url: null
published_date: Sep 12, 2017
published_date_iso: '2017-09-12'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Predicating macroscopic influences of drugs on human body, like efficacy
  and toxicity, is a central problem of small-molecule based drug discovery. Molecules
  can be represented as an undirected graph, and we can utilize graph convolution
  networks to predication molecular properties. However, graph convolutional networks
  and other graph neural networks all focus on learning node-level representation
  rather than graph-level representation. Previous works simply sum all feature vectors
  for all nodes in the graph to obtain the graph feature vector for drug predication.
  In this paper, we introduce a dummy super node that is connected with all nodes
  in the graph by a directed edge as the representation of the graph and modify the
  graph operation to help the dummy super node learn graph-level feature. Thus, we
  can handle graph-level classification and regression in the same way as node-level
  classification and regression. In addition, we apply focal loss to address class
  imbalance in drug datasets. The experiments on MoleculeNet show that our method
  can effectively improve the performance of molecular properties predication.
codebase_url: https://github.com/ZJULearning/graph_level_drug_discovery
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- dummy super node
mrr: 0.1429
adjusted_mrr: 0.0476
mrr_dataset_count: 1
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: FreeSolv
  rows:
  - model: SE(3)-I MPPH
    model_key: se(3)-i mpph
    model_plain: SE(3)-I MPPH
    value: 0.354
    std: 0.053
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrating SE(3)-invariance into Vietoris-Rips persistent
      homology
    is_global_top: true
    global_rank: 1
    sort_value: 0.354
    sort_std: 0.053
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECFP-4 + RF
    model_key: ecfp-4 + rf
    model_plain: ECFP-4 + RF
    value: 0.56
    std: 0.066
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_display: Dec 2023
    date_iso: '2023-12-12'
    venue: NeurIPS 2023 AI for Science Workshop
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: trained on ECFP-4 fingerprints
    is_global_top: true
    global_rank: 2
    sort_value: 0.56
    sort_std: 0.066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPSE + GPS
    model_key: gpse + gps
    model_plain: GPSE + GPS
    value: 0.682
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.07107'
    title: Graph Positional and Structural Encoder
    date: Jul 14, 2023
    date_display: Jul 2023
    date_iso: '2023-07-14'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.682
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: dummy super node
    model_key: dummy super node
    model_plain: dummy super node
    value: 0.933
    std: null
    paper_value: 0.933
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 12, 2017
    date_display: Sep 2017
    date_iso: '2017-09-12'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-09-12'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.933
    true_std: null
    value_gap_source_arxiv: '1709.03741'
    value_gap_source_title: Learning Graph-Level Representation for Drug Discovery
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: null
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
  - model: GraphConv
    model_key: graphconv
    model_plain: GraphConv
    value: 0.963
    std: null
    paper_value: 0.963
    paper_std: null
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 12, 2017
    date_display: Sep 2017
    date_iso: '2017-09-12'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-09-12'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.963
    true_std: null
    value_gap_source_arxiv: '1709.03741'
    value_gap_source_title: Learning Graph-Level Representation for Drug Discovery
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.963
    sort_std: null
    global_rank: 9
    paper_rank: 9
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
    value: 2.346
    std: 0.122
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_display: Jun 2021
    date_iso: '2021-06-11'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 69
    sort_value: 2.346
    sort_std: 0.122
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: MoleculeNet
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: FreeSolv
      dataset_slug: freesolv
single_proposed_model: dummy super node
main_figure: /figures/1709.03741/main_figure.jpegoptim.jpg
---

