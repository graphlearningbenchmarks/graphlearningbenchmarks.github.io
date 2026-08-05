---
title: 'NOSMOG: Learning Noise-robust and Structure-aware MLPs on Graphs'
arxiv_id: '2208.10010'
source_url: ''
authors:
- name: Yijun Tian
  orcid: null
  s2_author_id: '46879986'
  s2_url: null
- name: Chuxu Zhang
  orcid: null
  s2_author_id: '2117879943'
  s2_url: null
- name: Zhichun Guo
  orcid: null
  s2_author_id: '2109411071'
  s2_url: null
- name: Xiangliang Zhang
  orcid: null
  s2_author_id: '2928371'
  s2_url: null
- name: N. Chawla
  orcid: null
  s2_author_id: '144539424'
  s2_url: null
published_date: Aug 22, 2022
published_date_iso: '2022-08-22'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'While Graph Neural Networks (GNNs) have demonstrated their efficacy in
  dealing with non-Euclidean structural data, they are difficult to be deployed in
  real applications due to the scalability constraint imposed by multi-hop data dependency.
  Existing methods attempt to address this scalability issue by training multi-layer
  perceptrons (MLPs) exclusively on node content features using labels derived from
  trained GNNs. Even though the performance of MLPs can be significantly improved,
  two issues prevent MLPs from outperforming GNNs and being used in practice: the
  ignorance of graph structural information and the sensitivity to node feature noises.
  In this paper, we propose to learn ise-robust tructure-aware LPs n raphs (NOSMOG)
  to overcome the challenges. Specifically, we first complement node content with
  position features to help MLPs capture graph structural information. We then design
  a novel representational similarity distillation strategy to inject structural node
  similarities into MLPs. Finally, we introduce the adversarial feature augmentation
  to ensure stable learning against feature noises and further improve performance.
  Extensive experiments demonstrate that NOSMOG outperforms GNNs and the state-of-the-art
  method in both transductive and inductive settings across seven datasets, while
  maintaining a competitive inference efficiency. Codes are available at.'
codebase_url: https://github.com/meettyj/NOSMOG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NOSMOG
mrr: 0.0027
adjusted_mrr: 0.0018
mrr_dataset_count: 2
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
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.7122
    std: 0.015
    paper_value: 0.7122
    paper_std: 0.015
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting on CiteSeer (Planetoid split) using Accuracy.
    date: Aug 22, 2022
    date_display: Aug 2022
    date_iso: '2022-08-22'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7177
    at_pub_std: 0.020099999999999996
    at_pub_source_arxiv: '2110.08727'
    at_pub_source_title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks
      via Distillation'
    at_pub_source_date_iso: '2021-10-17'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-07-13'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.005499999999999949
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.74
    true_std: 0.0002
    value_gap_source_arxiv: '2307.06631'
    value_gap_source_title: Frameless Graph Knowledge Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.027799999999999936
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.0002
    global_rank: 272
    paper_rank: 595
    rank_delta: 323
    rank_delta_abs: 323
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NOSMOG
    model_key: nosmog
    model_plain: NOSMOG
    value: 0.7378
    std: 0.0154
    paper_value: 0.7378
    paper_std: 0.0154
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: mixed
    feature_source_evidence: incorporation of position features (DeepWalk) and node
      content features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting on CiteSeer (Planetoid split) using Accuracy.
    date: Aug 22, 2022
    date_display: Aug 2022
    date_iso: '2022-08-22'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-08-22'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7378
    true_std: 0.0154
    value_gap_source_arxiv: '2208.10010'
    value_gap_source_title: 'NOSMOG: Learning Noise-robust and Structure-aware MLPs
      on Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7378
    sort_std: 0.0154
    global_rank: 287
    paper_rank: 287
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
    value: 0.7049
    std: 0.0153
    paper_value: 0.7049
    paper_std: 0.0153
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting on CiteSeer (Planetoid split) using Accuracy.
    date: Aug 22, 2022
    date_display: Aug 2022
    date_iso: '2022-08-22'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7171
    at_pub_std: null
    at_pub_source_arxiv: '2103.02885'
    at_pub_source_title: 'Extract the Knowledge of Graph Neural Networks and Go Beyond
      it: An Effective Knowledge Distillation Framework'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.012199999999999989
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7361
    true_std: 0.019
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.031200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7361
    sort_std: 0.019
    global_rank: 299
    paper_rank: 653
    rank_delta: 354
    rank_delta_abs: 354
    rank_delta_direction: worse
    has_value_gap: true
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
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.8026
    std: 0.0166
    paper_value: 0.8026
    paper_std: 0.0166
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
    input_feature_source: raw_features
    feature_source_evidence: MLP student is trained with node content features as
      input
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, Planetoid split (20-per-class train
      split)
    date: Aug 22, 2022
    date_display: Aug 2022
    date_iso: '2022-08-22'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8054
    at_pub_std: 0.0135
    at_pub_source_arxiv: '2110.08727'
    at_pub_source_title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks
      via Distillation'
    at_pub_source_date_iso: '2021-10-17'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-07-13'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0028000000000000247
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.836
    true_std: 0.0022
    value_gap_source_arxiv: '2307.06631'
    value_gap_source_title: Frameless Graph Knowledge Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.033399999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0022
    global_rank: 461
    paper_rank: 768
    rank_delta: 307
    rank_delta_abs: 307
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NOSMOG
    model_key: nosmog
    model_plain: NOSMOG
    value: 0.8304
    std: 0.0126
    paper_value: 0.8304
    paper_std: 0.0126
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: mixed
    feature_source_evidence: concatenate the node content feature and position feature
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, Planetoid split (20-per-class train
      split)
    date: Aug 22, 2022
    date_display: Aug 2022
    date_iso: '2022-08-22'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-04'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8304
    true_std: 0.0126
    value_gap_source_arxiv: '2308.02117'
    value_gap_source_title: 'VQGraph: Rethinking Graph Representation Space for Bridging
      GNNs and MLPs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8304
    sort_std: 0.0126
    global_rank: 538
    paper_rank: 538
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
single_proposed_model: NOSMOG
main_figure: /figures/2208.10010/main_figure.jpegoptim.jpg
---

