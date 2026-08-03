---
title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
  Graph Embedding Reasoning'
arxiv_id: '2204.13957'
source_url: ''
authors:
- name: Linlin Chao
  orcid: null
  s2_author_id: '1850313'
  s2_url: null
- name: Taifeng Wang
  orcid: null
  s2_author_id: '1799672'
  s2_url: null
- name: Wei Chu
  orcid: null
  s2_author_id: '2057047939'
  s2_url: null
published_date: Apr 29, 2022
published_date_iso: '2022-04-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Knowledge graph (KG) embedding methods which map entities and relations
  to unique embeddings in the KG have shown promising results on many reasoning tasks.
  However, the same embedding dimension for both dense entities and sparse entities
  will cause either over parameterization (sparse entities) or under fitting (dense
  entities). Normally, a large dimension is set to get better performance. Meanwhile,
  the inference time grows log-linearly with the number of entities for all entities
  are traversed and compared. Both the parameter and inference become challenges when
  working with huge amounts of entities. Thus, we propose PIE, a parameter and inference
  efficient solution. Inspired from tensor decomposition methods, we find that decompose
  entity embedding matrix into low rank matrices can reduce more than half of the
  parameters while maintaining comparable performance. To accelerate model inference,
  we propose a self-supervised auxiliary task, which can be seen as fine-grained entity
  typing. By randomly masking and recovering entities' connected relations, the task
  learns the co-occurrence of entity and relations. Utilizing the fine grained typing,
  we can filter unrelated entities during inference and get targets with possibly
  sub-linear time requirement. Experiments on link prediction benchmarks demonstrate
  the proposed key capabilities. Moreover, we prove effectiveness of the proposed
  solution on the Open Graph Benchmark large scale challenge dataset WikiKG90Mv2 and
  achieve the state of the art performance.
codebase_url: https://github.com/migalkin/NodePiece
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: ogbl-biokg
  rows:
  - model: PairRE+LRE
    model_key: pairre+lre
    model_plain: PairRE+LRE
    value: 0.836
    std: null
    paper_value: 0.836
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 501.0
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chao-etal-2021-pairre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.836
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AutoSF
    model_key: autosf
    model_plain: AutoSF
    value: 0.8309
    std: null
    paper_value: 0.8309
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.2
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhang2020autosf
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8309
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-09-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8309
    true_std: 0.0008
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8309
    sort_std: 0.0008
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TripleREv2
    model_key: triplerev2
    model_plain: TripleREv2
    value: 0.8272
    std: 0.0007
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 500.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.08271'
    title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
    date: Sep 17, 2022
    date_display: Sep 2022
    date_iso: '2022-09-17'
    venue: null
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraph-
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8272
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TripleREv2
    model_key: triplere
    model_plain: TripleREv2
    value: 0.8191
    std: 0.0014
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.08271'
    title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
    date: Sep 17, 2022
    date_display: Sep 2022
    date_iso: '2022-09-17'
    venue: null
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraph-
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8191
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PairRE
    model_key: pairre
    model_plain: PairRE
    value: 0.8164
    std: null
    paper_value: 0.8164
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chao-etal-2021-pairre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8164
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2011.03798'
    at_pub_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    at_pub_source_date_iso: '2020-11-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-09-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8164
    true_std: 0.0005
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8164
    sort_std: 0.0005
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
  dataset: ogbl-wikikg2
  rows:
  - model: Information-Flow (IF) framework
    model_key: stargraph + triplere'
    model_plain: Information-Flow (IF) framework
    value: 0.729
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.729
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Information-Flow (IF) framework
    model_key: trans(large) + nodepiece
    model_plain: Information-Flow (IF) framework
    value: 0.6939
    std: 0.0011
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 38.430804
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6939
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Information-Flow (IF) framework
    model_key: trans + nodepiece
    model_plain: Information-Flow (IF) framework
    value: 0.6882
    std: 0.0019
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.215402
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.14209'
    title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
      Subgraph'
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    venue: Under review in ICLR 2023 (https://openreview.net/forum?id=mTOB_VK_BWk)
    codebase_url: https://github.com/hzli-ucas/StarGraph
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6882
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PairRE+LRE
    model_key: pairre+lre
    model_plain: PairRE+LRE
    value: 0.597
    std: null
    paper_value: 0.597
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 501.0
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chao-etal-2021-pairre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.597
    sort_std: null
    global_rank: 11
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSF + NodePiece
    model_key: autosf + nodepiece
    model_plain: AutoSF + NodePiece
    value: 0.5703
    std: null
    paper_value: 0.5703
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.9
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: galkin2021nodepiece
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5703
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2202.04897'
    at_pub_source_title: 'InterHT: Knowledge Graph Embeddings by Interaction between
      Head and Tail Entities'
    at_pub_source_date_iso: '2022-02-10'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5703
    true_std: 0.0035
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5703
    sort_std: 0.0035
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
  - model: AutoSF
    model_key: autosf
    model_plain: AutoSF
    value: 0.5458
    std: null
    paper_value: 0.5458
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.2
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhang2020autosf
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5458
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2202.04897'
    at_pub_source_title: 'InterHT: Knowledge Graph Embeddings by Interaction between
      Head and Tail Entities'
    at_pub_source_date_iso: '2022-02-10'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5458
    true_std: 0.0052
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5458
    sort_std: 0.0052
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PairRE
    model_key: pairre
    model_plain: PairRE
    value: 0.5805
    std: null
    paper_value: 0.5805
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chao-etal-2021-pairre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 29, 2022
    date_display: Apr 2022
    date_iso: '2022-04-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5289
    at_pub_std: 0.003
    at_pub_source_arxiv: '2011.03798'
    at_pub_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    at_pub_source_date_iso: '2020-11-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-09-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05159999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5208
    true_std: 0.0027
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: 0.059699999999999975
    has_value_note: false
    value_note: ''
    sort_value: 0.5208
    sort_std: 0.0027
    global_rank: 16
    paper_rank: 11
    rank_delta: -5
    rank_delta_abs: 5
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation
      Vectors'
    comparison_source_arxiv: '2011.03798'
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
- benchmark: OGB
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-wikikg2
      dataset_slug: ogbl-wikikg2
    - dataset: ogbl-biokg
      dataset_slug: ogbl-biokg
---

