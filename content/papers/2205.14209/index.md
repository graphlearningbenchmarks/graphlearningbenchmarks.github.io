---
title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop Subgraph'
arxiv_id: '2205.14209'
source_url: ''
authors:
- name: Hongzhu Li
  orcid: null
  s2_author_id: '2120465342'
  s2_url: null
- name: Xiang Gao
  orcid: null
  s2_author_id: '2149395798'
  s2_url: null
- name: Linhui Feng
  orcid: null
  s2_author_id: '47010066'
  s2_url: null
- name: Yafeng Deng
  orcid: null
  s2_author_id: '30639994'
  s2_url: null
- name: Yu Yin
  orcid: null
  s2_author_id: '2365399530'
  s2_url: null
published_date: May 27, 2022
published_date_iso: '2022-05-27'
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Conventional representation learning algorithms for knowledge graphs (KG)
  map each entity to a unique embedding vector, ignoring the rich information contained
  in the neighborhood. We propose a method named StarGraph, which gives a novel way
  to utilize the neighborhood information for large-scale knowledge graphs to obtain
  entity representations. An incomplete two-hop neighborhood subgraph for each target
  node is at first generated, then processed by a modified self-attention network
  to obtain the entity representation, which is used to replace the entity embedding
  in conventional methods. We achieved SOTA performance on ogbl-wikikg2 and got competitive
  results on fb15k-237. The experimental results proves that StarGraph is efficient
  in parameters, and the improvement made on ogbl-wikikg2 demonstrates its great effectiveness
  of representation learning on large-scale knowledge graphs. The code is now available
  at.
codebase_url: https://github.com/hzli-ucas/StarGraph
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- StarGraph + TripleRE'
mrr: 0.2581
adjusted_mrr: 0.172
mrr_dataset_count: 2
benchmark_categories:
- OGB
- Knowledge Graphs
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
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
  - model: CoKE
    model_key: coke
    model_plain: CoKE
    value: 0.364
    std: null
    paper_value: 0.364
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 10.19
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.361
    at_pub_std: null
    at_pub_source_arxiv: '2009.14332'
    at_pub_source_title: Multi-hop Attention Graph Neural Networks
    at_pub_source_date_iso: '2020-09-29'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.364
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.364
    sort_std: null
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multi-hop Attention Graph Neural Networks
    comparison_source_arxiv: '2009.14332'
    is_best: false
    is_std_outlier: false
  - model: GC-OTE
    model_key: gc-ote
    model_plain: GC-OTE
    value: 0.361
    std: null
    paper_value: 0.361
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
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.361
    at_pub_std: null
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
    true_value: 0.361
    true_std: null
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.361
    sort_std: null
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TripleRE'
    model_key: triplere'
    model_plain: TripleRE'
    value: 0.3514
    std: null
    paper_value: 0.3514
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.895296
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.3514
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3514
    sort_std: null
    global_rank: 52
    paper_rank: 52
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
    value: 0.351
    std: null
    paper_value: 0.351
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3348
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.351
    at_pub_std: 0.00066
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
    true_value: 0.351
    true_std: null
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.351
    sort_std: null
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: StarGraph + TripleRE'
    model_key: stargraph + triplere'
    model_plain: StarGraph + TripleRE'
    value: 0.3459
    std: null
    paper_value: 0.3459
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.3459
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3459
    sort_std: null
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RotatE
    model_key: rotate
    model_plain: RotatE
    value: 0.338
    std: null
    paper_value: 0.338
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.43575
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.338
    at_pub_std: null
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-25'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.338
    true_std: null
    value_gap_source_arxiv: '2302.13083'
    value_gap_source_title: Knowledge Graph Completion with Counterfactual Augmentation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.338
    sort_std: null
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.294
    std: null
    paper_value: 0.294
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.5695
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: Nguyen et al.
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.294
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
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
    true_value: 0.33
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03600000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.33
    sort_std: null
    global_rank: 78
    paper_rank: 90
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePiece + RotatE
    model_key: nodepiece + rotate
    model_plain: NodePiece + RotatE
    value: 0.258
    std: null
    paper_value: 0.258
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.2
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The plausibility of each triple is calculated on the
      embeddings of the entities and relations in it, and the embeddings are directly
      taken out from the embedding tables.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Toutanova & Chen 2015 split
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.258
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.258
    sort_std: null
    global_rank: 99
    paper_rank: 99
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
  - model: InterHT + DigPiece
    model_key: interht + digpiece
    model_plain: InterHT + DigPiece
    value: 0.7293
    std: 0.0018
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_display: Feb 2022
    date_iso: '2022-02-10'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7293
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: StarGraph + TripleRE'
    model_key: stargraph + triplere'
    model_plain: StarGraph + TripleRE'
    value: 0.729
    std: null
    paper_value: 0.729
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.729
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: null
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
  - model: TripleRE + StarGraph
    model_key: triplere + stargraph
    model_plain: TripleRE + StarGraph
    value: 0.7201
    std: 0.0011
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 86.7
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04897'
    title: 'InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail
      Entities'
    date: Feb 10, 2022
    date_display: Feb 2022
    date_iso: '2022-02-10'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7201
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TranS(large) + NodePiece
    model_key: trans(large) + nodepiece
    model_plain: TranS(large) + NodePiece
    value: 0.6939
    std: 0.0011
    paper_value: 0.6939
    paper_std: 0.0011
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 38.430804
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6939
    true_std: 0.0011
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6939
    sort_std: 0.0011
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
  - model: TranS + NodePiece
    model_key: trans + nodepiece
    model_plain: TranS + NodePiece
    value: 0.6882
    std: 0.0019
    paper_value: 0.6882
    paper_std: 0.0019
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.215402
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6882
    true_std: 0.0019
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6882
    sort_std: 0.0019
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
  - model: TripleREv3 + NodePiece
    model_key: triplerev3 + nodepiece
    model_plain: TripleREv3 + NodePiece
    value: 0.6866
    std: 0.0014
    paper_value: 0.6866
    paper_std: 0.0014
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 36.421802
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6866
    true_std: 0.0014
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6866
    sort_std: 0.0014
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
  - model: InterHT + NodePiece
    model_key: interht + nodepiece
    model_plain: InterHT + NodePiece
    value: 0.6779
    std: 0.0018
    paper_value: 0.6779
    paper_std: 0.0018
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 19.215402
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.6779
    at_pub_std: 0.0018
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
    true_value: 0.6779
    true_std: 0.0018
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6779
    sort_std: 0.0018
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
  - model: TripleREv2 + NodePiece
    model_key: triplerev2 + nodepiece
    model_plain: TripleREv2 + NodePiece
    value: 0.6582
    std: 0.002
    paper_value: 0.6582
    paper_std: 0.002
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7.289002
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6582
    true_std: 0.002
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6582
    sort_std: 0.002
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx-RP
    model_key: complex-rp
    model_plain: ComplEx-RP
    value: 0.6392
    std: 0.0045
    paper_value: 0.6392
    paper_std: 0.0045
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 250.1674
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6392
    true_std: 0.0045
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6392
    sort_std: 0.0045
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
  - model: TripleREv2
    model_key: triplerev2
    model_plain: TripleREv2
    value: 0.6045
    std: 0.0017
    paper_value: 0.6045
    paper_std: 0.0017
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.763337
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.6045
    true_std: 0.0017
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6045
    sort_std: 0.0017
    global_rank: 19
    paper_rank: 19
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
    value: 0.5208
    std: 0.0027
    paper_value: 0.5208
    paper_std: 0.0027
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.3348
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.5805
    at_pub_std: null
    at_pub_source_arxiv: '2204.13957'
    at_pub_source_title: 'PIE: a Parameter and Inference Efficient Solution for Large
      Scale Knowledge Graph Embedding Reasoning'
    at_pub_source_date_iso: '2022-04-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.059699999999999975
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5805
    true_std: null
    value_gap_source_arxiv: '2204.13957'
    value_gap_source_title: 'PIE: a Parameter and Inference Efficient Solution for
      Large Scale Knowledge Graph Embedding Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: 0.059699999999999975
    has_value_note: false
    value_note: ''
    sort_value: 0.5805
    sort_std: null
    global_rank: 24
    paper_rank: 29
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PIE: a Parameter and Inference Efficient Solution for
      Large Scale Knowledge Graph Embedding Reasoning'
    comparison_source_arxiv: '2204.13957'
    is_best: false
    is_std_outlier: false
  - model: TripleRE
    model_key: triplere
    model_plain: TripleRE
    value: 0.5794
    std: 0.002
    paper_value: 0.5794
    paper_std: 0.002
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.763337
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.5794
    at_pub_std: 0.002
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
    true_value: 0.5794
    true_std: 0.002
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5794
    sort_std: 0.002
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSF + NodePiece
    model_key: autosf + nodepiece
    model_plain: AutoSF + NodePiece
    value: 0.5703
    std: 0.0035
    paper_value: 0.5703
    paper_std: 0.0035
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.860602
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
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
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5703
    sort_std: 0.0035
    global_rank: 28
    paper_rank: 28
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
    std: 0.0052
    paper_value: 0.5458
    paper_std: 0.0052
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.2278
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
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
    global_rank: 29
    paper_rank: 29
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
    value: 0.5027
    std: 0.0027
    paper_value: 0.5027
    paper_std: 0.0027
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.5695
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.4028
    at_pub_std: 0.003
    at_pub_source_arxiv: '2011.03798'
    at_pub_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    at_pub_source_date_iso: '2020-11-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.09990000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5027
    true_std: 0.0027
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5027
    sort_std: 0.0027
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation
      Vectors'
    comparison_source_arxiv: '2011.03798'
    is_best: false
    is_std_outlier: false
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.4256
    std: 0.003
    paper_value: 0.4256
    paper_std: 0.003
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.5695
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.4536
    at_pub_std: 0.003
    at_pub_source_arxiv: '2011.03798'
    at_pub_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    at_pub_source_date_iso: '2020-11-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.028000000000000025
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4536
    true_std: 0.003
    value_gap_source_arxiv: '2011.03798'
    value_gap_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: 0.028000000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.4536
    sort_std: 0.003
    global_rank: 34
    paper_rank: 37
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PairRE: Knowledge Graph Embeddings via Paired Relation
      Vectors'
    comparison_source_arxiv: '2011.03798'
    is_best: false
    is_std_outlier: false
  - model: RotatE
    model_key: rotate
    model_plain: RotatE
    value: 0.4332
    std: 0.0025
    paper_value: 0.4332
    paper_std: 0.0025
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1250.43575
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard split for ogbl-wikikg2
    date: May 27, 2022
    date_display: May 2022
    date_iso: '2022-05-27'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.4332
    at_pub_std: 0.0025
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
    true_value: 0.4332
    true_std: 0.0025
    value_gap_source_arxiv: '2209.08271'
    value_gap_source_title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation
      Vectors'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4332
    sort_std: 0.0025
    global_rank: 35
    paper_rank: 35
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
- benchmark: OGB
  datasets:
  - *id001
- benchmark: Knowledge Graphs
  datasets:
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
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: FB15k-237
      dataset_slug: fb15k-237
single_proposed_model: StarGraph + TripleRE'
main_figure: /figures/2205.14209/main_figure.jpegoptim.jpg
---

