---
title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks via Distillation'
arxiv_id: '2110.08727'
source_url: ''
authors:
- name: Shichang Zhang
  orcid: null
  s2_author_id: '2145408511'
  s2_url: null
- name: Yozen Liu
  orcid: null
  s2_author_id: '152891495'
  s2_url: null
- name: Yizhou Sun
  orcid: null
  s2_author_id: '2279734673'
  s2_url: null
- name: Neil Shah
  orcid: null
  s2_author_id: '145474474'
  s2_url: null
published_date: Oct 17, 2021
published_date_iso: '2021-10-17'
published_venue: ICLR 2021
published_conference: ICLR 2021
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Graph Neural Networks (GNNs) are popular for graph machine learning and
  have shown great results on wide node classification tasks. Yet, they are less popular
  for practical deployments in the industry owing to their scalability challenges
  incurred by data dependency. Namely, GNN inference depends on neighbor nodes multiple
  hops away from the target, and fetching them burdens latency-constrained applications.
  Existing inference acceleration methods like pruning and quantization can speed
  up GNNs by reducing Multiplication-and-ACcumulation (MAC) operations, but the improvements
  are limited given the data dependency is not resolved. Conversely, multi-layer perceptrons
  (MLPs) have no graph dependency and infer much faster than GNNs, even though they
  are less accurate than GNNs for node classification in general. Motivated by these
  complementary strengths and weaknesses, we bring GNNs and MLPs together via knowledge
  distillation (KD). Our work shows that the performance of MLPs can be improved by
  large margins with GNN KD. We call the distilled MLPs Graph-less Neural Networks
  (GLNN s) as they have no inference graph dependency. We show that GLNN s with competitive
  accuracy infer faster than GNNs by 146-273 and faster than other acceleration methods
  by 14-27. Under a production setting involving both transductive and inductive predictions
  across 7 datasets, GLNN accuracies improve over stand-alone MLPs by 12.36\
codebase_url: https://github.com/snap-research/graphless-neural-networks
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GLNN
mrr: 0.0029
adjusted_mrr: 0.0029
mrr_dataset_count: 4
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9412
    std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9412
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9398
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9398
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8297
    std: 0.0216
    paper_value: 0.8297
    paper_std: 0.0216
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting on A-computer
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.789
    at_pub_std: 0.021
    at_pub_source_arxiv: '2006.10222'
    at_pub_source_title: Class-Attentive Diffusion Network for Semi-Supervised Classification
    at_pub_source_date_iso: '2020-06-18'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.04069999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9351
    true_std: 0.0006
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.10540000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9351
    sort_std: 0.0006
    global_rank: 8
    paper_rank: 431
    rank_delta: 423
    rank_delta_abs: 423
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.912
    std: 0.0029
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.08798'
    title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
    date: Dec 9, 2025
    date_display: Dec 2025
    date_iso: '2025-12-09'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 64
    sort_value: 0.912
    sort_std: 0.0029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.8303
    std: 0.0187
    paper_value: 0.8303
    paper_std: 0.0187
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting on A-computer
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.875
    true_std: 0.006
    value_gap_source_arxiv: '2412.03864'
    value_gap_source_title: Training MLPs on Graphs without Supervision
    value_gap_source_is_current_paper: false
    value_gap: 0.04469999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.875
    sort_std: 0.006
    global_rank: 280
    paper_rank: 430
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.678
    std: 0.0106
    paper_value: 0.678
    paper_std: 0.0106
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting on A-computer
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.449
    at_pub_std: 0.058
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.22900000000000004
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8463
    true_std: null
    value_gap_source_arxiv: '2407.11907'
    value_gap_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    value_gap_source_is_current_paper: false
    value_gap: 0.1683
    has_value_note: false
    value_note: ''
    sort_value: 0.8463
    sort_std: null
    global_rank: 365
    paper_rank: 542
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Towards Deeper Graph Neural Networks
    comparison_source_arxiv: '2007.09296'
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
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
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
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
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
    input_feature_source: raw_features
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
  - model: EERM
    model_key: eerm
    model_plain: EERM
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
    input_feature_source: raw_features
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8774
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.7177
    std: 0.020099999999999996
    paper_value: 0.7177
    paper_std: 0.020099999999999996
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
    protocol_note: transductive setting on Planetoid split (Yang et al. 2016)
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-13'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
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
    value_gap: 0.022299999999999986
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.0002
    global_rank: 277
    paper_rank: 536
    rank_delta: 259
    rank_delta_abs: 259
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7033
    std: 0.0197
    paper_value: 0.7033
    paper_std: 0.0197
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
    protocol_note: transductive setting on Planetoid split (Yang et al. 2016)
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.7171
    at_pub_std: null
    at_pub_source_arxiv: '2103.02885'
    at_pub_source_title: 'Extract the Knowledge of Graph Neural Networks and Go Beyond
      it: An Effective Knowledge Distillation Framework'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.013799999999999923
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
    value_gap: 0.03279999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7361
    sort_std: 0.019
    global_rank: 305
    paper_rank: 663
    rank_delta: 358
    rank_delta_abs: 358
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5961
    std: 0.0288
    paper_value: 0.5961
    paper_std: 0.0288
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
    protocol_note: transductive setting on Planetoid split (Yang et al. 2016)
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.6398
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2010.12408'
    at_pub_source_title: On the Equivalence of Decoupled Graph Convolution Network
      and Label Propagation
    at_pub_source_date_iso: '2020-10-23'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.04370000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7289
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.13280000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 909
    rank_delta: 508
    rank_delta_abs: 508
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Decoupled Graph Convolution Network
      and Label Propagation
    comparison_source_arxiv: '2010.12408'
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
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9004
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
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 31
    sort_value: 0.9004
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.8054
    std: 0.0135
    paper_value: 0.8054
    paper_std: 0.0135
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
    protocol_note: transductive setting; Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split)
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-13'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
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
    value_gap: 0.03059999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0022
    global_rank: 419
    paper_rank: 714
    rank_delta: 295
    rank_delta_abs: 295
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5922
    std: 0.0131
    paper_value: 0.5922
    paper_std: 0.0131
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
    protocol_note: transductive setting; Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split)
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.616
    at_pub_std: 0.006
    at_pub_source_arxiv: '2103.07295'
    at_pub_source_title: Adversarial Graph Disentanglement with Component-specific
      Aggregation
    at_pub_source_date_iso: '2021-03-12'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.023800000000000043
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1846000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 963
    rank_delta: 157
    rank_delta_abs: 157
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Adversarial Graph Disentanglement with Component-specific
      Aggregation
    comparison_source_arxiv: '2103.07295'
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
- &id002
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
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
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
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
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
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
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9296
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 19
    sort_value: 0.9296
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7539
    std: 0.0209
    paper_value: 0.7539
    paper_std: 0.0209
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
    protocol_note: Transductive setting on Planetoid split (Yang et al. 2016).
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.7736
    at_pub_std: null
    at_pub_source_arxiv: '2103.02885'
    at_pub_source_title: 'Extract the Knowledge of Graph Neural Networks and Go Beyond
      it: An Effective Knowledge Distillation Framework'
    at_pub_source_date_iso: '2021-03-04'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.01969999999999994
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8881
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: false
    value_gap: 0.13419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8881
    sort_std: 0.0015
    global_rank: 134
    paper_rank: 869
    rank_delta: 735
    rank_delta_abs: 735
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6755
    std: 0.0231
    paper_value: 0.6755
    paper_std: 0.0231
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
    protocol_note: Transductive setting on Planetoid split (Yang et al. 2016).
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.742
    at_pub_std: 0.007
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.0665
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.1935
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 939
    rank_delta: 696
    rank_delta_abs: 696
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Deeper Graph Neural Networks
    comparison_source_arxiv: '2007.09296'
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.7542
    std: 0.0231
    paper_value: 0.7542
    paper_std: 0.0231
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
    protocol_note: Transductive setting on Planetoid split (Yang et al. 2016).
    date: Oct 17, 2021
    date_display: Oct 2021
    date_iso: '2021-10-17'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8027
    true_std: 0.0036
    value_gap_source_arxiv: '2405.03401'
    value_gap_source_title: 'E2GNN: Efficient Graph Neural Network Ensembles for Semi-Supervised
      Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04849999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8027
    sort_std: 0.0036
    global_rank: 479
    paper_rank: 867
    rank_delta: 388
    rank_delta_abs: 388
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
single_proposed_model: GLNN
main_figure: /figures/2110.08727/main_figure.jpegoptim.jpg
---

