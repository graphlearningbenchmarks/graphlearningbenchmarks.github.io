---
title: Knowledge Graphs
arxiv_id: '1707.01476'
source_url: ''
authors:
- name: Tim Dettmers
  orcid: null
  s2_author_id: '3239480'
  s2_url: null
- name: Pasquale Minervini
  orcid: null
  s2_author_id: '3051815'
  s2_url: null
- name: Pontus Stenetorp
  orcid: null
  s2_author_id: '1918552'
  s2_url: null
- name: Sebastian Riedel
  orcid: null
  s2_author_id: '48662861'
  s2_url: null
published_date: Jul 5, 2017
published_date_iso: '2017-07-05'
published_venue: AAAI 2017
published_conference: AAAI 2017
published_conference_short: AAAI
published_conference_slug: aaai
abstract: 'Link prediction for knowledge graphs is the task of predicting missing
  relationships between entities. Previous work on link prediction has focused on
  shallow, fast models which can scale to large knowledge graphs. However, these models
  learn less expressive features than deep, multi-layer models -- which potentially
  limits performance. In this work we introduce ConvE, a multi-layer convolutional
  network model for link prediction, and report state-of-the-art results for several
  established datasets. We also show that the model is highly parameter efficient,
  yielding the same performance as DistMult and R-GCN with 8x and 17x fewer parameters.
  Analysis of our model suggests that it is particularly effective at modelling nodes
  with high indegree -- which are common in highly-connected, complex knowledge graphs
  such as Freebase and YAGO3. In addition, it has been noted that the WN18 and FB15k
  datasets suffer from test set leakage, due to inverse relations from the training
  set being present in the test set -- however, the extent of this issue has so far
  not been quantified. We find this problem to be severe: a simple rule-based model
  can achieve state-of-the-art results on both WN18 and FB15k. To ensure that models
  are evaluated on datasets where simply exploiting inverse relations cannot yield
  competitive results, we investigate and validate several commonly used datasets
  -- deriving robust variants where necessary. We then perform experiments on these
  robust datasets for our own and several previously proposed models, and find that
  ConvE achieves state-of-the-art Mean Reciprocal Rank across most datasets.'
codebase_url: https://github.com/TimDettmers/ConvE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ConvE
mrr: 0.1178
adjusted_mrr: 0.1178
mrr_dataset_count: 3
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 3
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: FB15k-237
  rows:
  - model: sum, Msg_r^3, f(t)=0
    model_key: sum, msg_r^3, f(t)=0
    model_plain: sum, Msg_r^3, f(t)=0
    value: 0.85
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.85
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: sum, Msg_r^3, f(t)=t
    model_key: sum, msg_r^3, f(t)=t
    model_plain: sum, Msg_r^3, f(t)=t
    value: 0.844
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.844
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: relation-specific
    model_key: relation-specific
    model_plain: relation-specific
    value: 0.835
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.835
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.637
    std: 0.017
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted by ICLR'26, 41 pages
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 28
    sort_value: 0.637
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.241
    std: null
    paper_value: 0.241
    paper_std: null
    metric: MRR
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
    source_ref: yang15:embedding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.358
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: 0.11699999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.358
    sort_std: null
    global_rank: 58
    paper_rank: 116
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.247
    std: null
    paper_value: 0.247
    paper_std: null
    metric: MRR
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
    source_ref: DBLP:conf/icml/TrouillonWRGB16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.346
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: 0.09899999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.346
    sort_std: null
    global_rank: 73
    paper_rank: 115
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConvE
    model_key: conve
    model_plain: ConvE
    value: 0.325
    std: null
    paper_value: 0.325
    paper_std: null
    metric: MRR
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.325
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.325
    sort_std: null
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.248
    std: null
    paper_value: 0.248
    paper_std: null
    metric: MRR
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
    source_ref: schlichtkrull2017modeling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.249
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.249
    sort_std: null
    global_rank: 113
    paper_rank: 114
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Inverse Model
    model_key: inverse model
    model_plain: Inverse Model
    value: 0.01
    std: null
    paper_value: 0.01
    paper_std: null
    metric: MRR
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.01
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.01
    sort_std: null
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: WN18
  rows:
  - model: Inverse Model
    model_key: inverse model
    model_plain: Inverse Model
    value: 0.963
    std: null
    paper_value: 0.963
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
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
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.963
    sort_std: null
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
  - model: RotatE
    model_key: rotate
    model_plain: RotatE
    value: 0.949
    std: 0.0
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraphEmbedding
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.949
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConvE
    model_key: conve
    model_plain: ConvE
    value: 0.943
    std: null
    paper_value: 0.943
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.943
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.943
    sort_std: null
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
  - model: ANALOGY
    model_key: analogy
    model_plain: ANALOGY
    value: 0.942
    std: null
    paper_value: 0.942
    paper_std: null
    metric: MRR
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
    source_ref: 2017arXiv170502426L
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.942
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.942
    sort_std: null
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.941
    std: null
    paper_value: 0.941
    paper_std: null
    metric: MRR
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
    source_ref: DBLP:conf/icml/TrouillonWRGB16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: 0.941
    at_pub_std: null
    at_pub_source_arxiv: '1703.06103'
    at_pub_source_title: Modeling Relational Data with Graph Convolutional Networks
    at_pub_source_date_iso: '2017-03-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.941
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.941
    sort_std: null
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
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.822
    std: null
    paper_value: 0.822
    paper_std: null
    metric: MRR
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
    source_ref: yang15:embedding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: 0.822
    at_pub_std: null
    at_pub_source_arxiv: '1606.06357'
    at_pub_source_title: Complex Embeddings for Simple Link Prediction
    at_pub_source_date_iso: '2016-06-19'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.822
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: null
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
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.814
    std: null
    paper_value: 0.814
    paper_std: null
    metric: MRR
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
    source_ref: schlichtkrull2017modeling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: 0.819
    at_pub_std: null
    at_pub_source_arxiv: '1703.06103'
    at_pub_source_title: Modeling Relational Data with Graph Convolutional Networks
    at_pub_source_date_iso: '2017-03-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2017-03-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: null
    value_gap_source_arxiv: '1703.06103'
    value_gap_source_title: Modeling Relational Data with Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: null
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Modeling Relational Data with Graph Convolutional Networks
    comparison_source_arxiv: '1703.06103'
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: WN18RR
  rows:
  - model: PNA, Msg_r^2, f(t)=t
    model_key: pna, msg_r^2, f(t)=t
    model_plain: PNA, Msg_r^2, f(t)=t
    value: 0.947
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA, Msg_r^3, f(t)=0
    model_key: pna, msg_r^3, f(t)=0
    model_plain: PNA, Msg_r^3, f(t)=0
    value: 0.947
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PNA, Msg_r^2, f(t)=0
    model_key: pna, msg_r^2, f(t)=0
    model_plain: PNA, Msg_r^2, f(t)=0
    value: 0.946
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_display: Feb 2023
    date_iso: '2023-02-04'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.946
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8298
    std: 0.0022
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: Accepted by NeurIPS 2025
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 27
    sort_value: 0.8298
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConvE
    model_key: conve
    model_plain: ConvE
    value: 0.43
    std: null
    paper_value: 0.43
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-25'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.462
    true_std: null
    value_gap_source_arxiv: '2302.13083'
    value_gap_source_title: Knowledge Graph Completion with Counterfactual Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.03200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.462
    sort_std: null
    global_rank: 105
    paper_rank: 117
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.43
    std: null
    paper_value: 0.43
    paper_std: null
    metric: MRR
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
    source_ref: yang15:embedding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.455
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: 0.025000000000000022
    has_value_note: false
    value_note: ''
    sort_value: 0.455
    sort_std: null
    global_rank: 109
    paper_rank: 117
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.44
    std: null
    paper_value: 0.44
    paper_std: null
    metric: MRR
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
    source_ref: DBLP:conf/icml/TrouillonWRGB16
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.44
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.44
    sort_std: null
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Inverse Model
    model_key: inverse model
    model_plain: Inverse Model
    value: 0.35
    std: null
    paper_value: 0.35
    paper_std: null
    metric: MRR
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jul 5, 2017
    date_display: Jul 2017
    date_iso: '2017-07-05'
    published_venue: AAAI 2017
    published_conference: AAAI 2017
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-05'
    value_gap_source_date_label: AAAI 2017
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.35
    true_std: null
    value_gap_source_arxiv: '1707.01476'
    value_gap_source_title: Knowledge Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.35
    sort_std: null
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
    - dataset: FB15k-237
      dataset_slug: fb15k-237
    - dataset: WN18
      dataset_slug: wn18
single_proposed_model: ConvE
main_figure: /figures/1707.01476/main_figure.jpegoptim.jpg
---

