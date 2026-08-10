---
title: 3D Molecular Geometry Analysis with 2D Graphs
arxiv_id: '2305.13315'
source_url: ''
authors:
- name: Zhao Xu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Yaochen Xie
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Youzhi Luo
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Xuan Zhang
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Xinyi Xu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Meng Liu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Kaleb Dickerson
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Cheng Deng
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Maho Nakata
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: null
  s2_url: null
published_date: May 1, 2023
published_date_iso: '2023-05-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Ground-state 3D geometries of molecules are essential for many molecular
  analysis tasks. Modern quantum mechanical methods can compute accurate 3D geometries
  but are computationally prohibitive. Currently, an efficient alternative to computing
  ground-state 3D molecular geometries from 2D graphs is lacking. Here, we propose
  a novel deep learning framework to predict 3D geometries from molecular graphs.
  To this end, we develop an equilibrium message passing neural network (EMPNN) to
  better capture ground-state geometries from molecular graphs. To provide a testbed
  for 3D molecular geometry analysis, we develop a benchmark that includes a large-scale
  molecular geometry dataset, data splits, and evaluation protocols. Experimental
  results show that EMPNN can efficiently predict more accurate ground-state 3D geometries
  than RDKit and other deep learning methods. Results also show that the proposed
  framework outperforms self-supervised learning methods on property prediction tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GAP-EMPNN
mrr: 0.0205
adjusted_mrr: 0.0137
mrr_dataset_count: 2
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 2
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: Graphormer-SPIS
    model_key: graphormer-spis
    model_plain: Graphormer-SPIS
    value: 0.484
    std: 0.005
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.484
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPD
    model_key: graphormer-spd
    model_plain: Graphormer-SPD
    value: 0.492
    std: 0.004
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.492
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: conan-FGW
    model_key: conan-fgw
    model_plain: conan-FGW
    value: 0.514
    std: 0.019
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.514
    sort_std: 0.019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.564
    std: 0.015
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 7
    sort_value: 0.564
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAP-EMPNN
    model_key: gap-empnn
    model_plain: GAP-EMPNN
    value: 0.997
    std: 0.027
    paper_value: 0.997
    paper_std: 0.027
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.997
    true_std: 0.027
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.997
    sort_std: 0.027
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 1.109
    std: null
    paper_value: 1.109
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.091
    at_pub_std: 0.021
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.018000000000000016
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 1.091
    true_std: 0.021
    value_gap_source_arxiv: '2209.15101'
    value_gap_source_title: Improving Molecular Pretraining with Complementary Featurizations
    value_gap_source_is_current_paper: false
    value_gap: 0.018000000000000016
    has_value_note: false
    value_note: ''
    sort_value: 1.091
    sort_std: 0.021
    global_rank: 99
    paper_rank: 102
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AM
    model_key: am
    model_plain: AM
    value: 1.112
    std: null
    paper_value: 1.112
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.112
    at_pub_std: 0.048
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.112
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.112
    sort_std: null
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 1.12
    std: null
    paper_value: 1.12
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.12
    at_pub_std: 0.019
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.12
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.12
    sort_std: null
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CP
    model_key: cp
    model_plain: CP
    value: 1.196
    std: null
    paper_value: 1.196
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.196
    at_pub_std: 0.037
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.196
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.196
    sort_std: null
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
- &id002
  dataset: Lipophilicity
  rows:
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.556
    std: 0.023
    metric: RMSE
    higher_is_better: false
    is_baseline: true
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
    sort_value: 0.556
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ProtoS-L2
    model_key: protos-l2
    model_plain: ProtoS-L2
    value: 0.58
    std: 0.016
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.065
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_display: Jun 2020
    date_iso: '2020-06-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.58
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ProtoW-L2
    model_key: protow-l2
    model_plain: ProtoW-L2
    value: 0.604
    std: 0.014
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.04804'
    title: Optimal Transport Graph Neural Networks
    date: Jun 8, 2020
    date_display: Jun 2020
    date_iso: '2020-06-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.604
    sort_std: 0.014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.655
    std: 0.036
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 7
    sort_value: 0.655
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CP
    model_key: cp
    model_plain: CP
    value: 0.702
    std: null
    paper_value: 0.702
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.702
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.702
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 0.708
    std: null
    paper_value: 0.708
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: 0.007
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.708
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: null
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.718
    std: null
    paper_value: 0.718
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.718
    at_pub_std: 0.016
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.718
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: null
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AM
    model_key: am
    model_plain: AM
    value: 0.73
    std: null
    paper_value: 0.73
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.73
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: null
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAP-EMPNN
    model_key: gap-empnn
    model_plain: GAP-EMPNN
    value: 0.732
    std: 0.005
    paper_value: 0.732
    paper_std: 0.005
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
    date: May 1, 2023
    date_display: May 2023
    date_iso: '2023-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.732
    true_std: 0.005
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.732
    sort_std: 0.005
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: ESOL
      dataset_slug: esol
    - dataset: Lipophilicity
      dataset_slug: lipophilicity
single_proposed_model: GAP-EMPNN
main_figure: /figures/2305.13315/main_figure.jpegoptim.jpg
---

