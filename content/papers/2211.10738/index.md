---
title: Knowledge Graph Contrastive Learning based on Relation-Symmetrical Structure
arxiv_id: '2211.10738'
source_url: ''
authors:
- name: K. Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Wenxuan Tu
  orcid: null
  s2_author_id: '1381761887'
  s2_url: null
- name: Yi Wen
  orcid: null
  s2_author_id: '2187327966'
  s2_url: null
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Xiang Dong
  orcid: null
  s2_author_id: '2118187046'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
published_date: Nov 19, 2022
published_date_iso: '2022-11-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Knowledge graph embedding (KGE) aims at learning powerful representations
  to benefit various artificial intelligence applications. Meanwhile, contrastive
  learning has been widely leveraged in graph learning as an effective mechanism to
  enhance the discriminative capacity of the learned representations. However, the
  complex structures of KG make it hard to construct appropriate contrastive pairs.
  Only a few attempts have integrated contrastive learning strategies with KGE. But,
  most of them rely on language models (e.g., Bert) for contrastive pair construction
  instead of fully mining information underlying the graph structure, hindering expressive
  ability. Surprisingly, we find that the entities within a relational symmetrical
  structure are usually similar and correlated. To this end, we propose a knowledge
  graph contrastive learning framework based on relation-symmetrical structure, KGE-SymCL,
  which mines symmetrical structure information in KGs to enhance the discriminative
  ability of KGE models. Concretely, a plug-and-play approach is proposed by taking
  entities in the relation-symmetrical positions as positive pairs. Besides, a self-supervised
  alignment loss is designed to pull together positive pairs. Experimental results
  on link prediction and entity classification datasets demonstrate that our KGE-SymCL
  can be easily adopted to various KGE models for performance improvements. Moreover,
  extensive experiments show that our model could outperform other state-of-the-art
  baselines.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TransE-SymCL
- HAKE-SymCL
- DisMult-SymCL
- ComplEX-DURA-SymCL
- RGCN-SymCL
- COMPGCN-SymCL
- SimKGC-SymCL
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 2
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: FB15k-237
  rows:
  - model: CompGCN
    model_key: llms
    model_plain: CompGCN
    value: 0.815
    std: 0.023
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
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
    global_rank: 1
    sort_value: 0.815
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: gcope
    model_plain: CompGCN
    value: 0.793
    std: 0.022
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
    global_rank: 2
    sort_value: 0.793
    sort_std: 0.022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    value: 0.791
    std: 0.016
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
    global_rank: 3
    sort_value: 0.791
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ComplEX-DURA-SymCL
    model_key: complex-dura-symcl
    model_plain: ComplEX-DURA-SymCL
    value: 0.371
    std: null
    paper_value: 0.371
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.371
    sort_std: null
    global_rank: 18
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
  - model: ComplEX-DURA
    model_key: complex-dura
    model_plain: ComplEX-DURA
    value: 0.37
    std: null
    paper_value: 0.37
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.37
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.37
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
  - model: CompGCN
    model_key: compgcn
    model_plain: CompGCN
    value: 0.352
    std: null
    paper_value: 0.352
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.355
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.355
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.355
    sort_std: null
    global_rank: 30
    paper_rank: 32
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    comparison_source_arxiv: '1911.03082'
    is_best: false
    is_std_outlier: false
  - model: COMPGCN-SymCL
    model_key: compgcn-symcl
    model_plain: COMPGCN-SymCL
    value: 0.354
    std: null
    paper_value: 0.354
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.354
    sort_std: null
    global_rank: 32
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
  - model: HAKE-SymCL
    model_key: hake-symcl
    model_plain: HAKE-SymCL
    value: 0.346
    std: null
    paper_value: 0.346
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.346
    sort_std: null
    global_rank: 43
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
  - model: HAKE
    model_key: hake
    model_plain: HAKE
    value: 0.335
    std: null
    paper_value: 0.335
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
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.346
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-02-25'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.010999999999999954
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.346
    true_std: null
    value_gap_source_arxiv: '2302.13083'
    value_gap_source_title: Knowledge Graph Completion with Counterfactual Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.010999999999999954
    has_value_note: false
    value_note: ''
    sort_value: 0.346
    sort_std: null
    global_rank: 41
    paper_rank: 49
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural
      Network Framework for Link Prediction'
    comparison_source_arxiv: '2106.06935'
    is_best: false
    is_std_outlier: false
  - model: SimKGC-SymCL
    model_key: simkgc-symcl
    model_plain: SimKGC-SymCL
    value: 0.324
    std: null
    paper_value: 0.324
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.324
    sort_std: null
    global_rank: 64
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
  - model: SimKGC
    model_key: simkgc
    model_plain: SimKGC
    value: 0.322
    std: null
    paper_value: 0.322
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: SimKGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.322
    sort_std: null
    global_rank: 64
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
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.289
    std: null
    paper_value: 0.289
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.294
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.294
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.294
    sort_std: null
    global_rank: 66
    paper_rank: 67
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    comparison_source_arxiv: '1911.03082'
    is_best: false
    is_std_outlier: false
  - model: TransE-SymCL
    model_key: transe-symcl
    model_plain: TransE-SymCL
    value: 0.29
    std: null
    paper_value: 0.29
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.29
    sort_std: null
    global_rank: 68
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
  - model: DisMult-SymCL
    model_key: dismult-symcl
    model_plain: DisMult-SymCL
    value: 0.26
    std: null
    paper_value: 0.26
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.26
    sort_std: null
    global_rank: 71
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
  - model: RGCN-SymCL
    model_key: rgcn-symcl
    model_plain: RGCN-SymCL
    value: 0.249
    std: null
    paper_value: 0.249
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.249
    sort_std: null
    global_rank: 73
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.273
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.025000000000000022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.248
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.248
    sort_std: null
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural
      Network Framework for Link Prediction'
    comparison_source_arxiv: '2106.06935'
    is_best: false
    is_std_outlier: false
  - model: DisMult
    model_key: dismult
    model_plain: DisMult
    value: 0.243
    std: null
    paper_value: 0.243
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
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.241
    at_pub_std: null
    at_pub_source_arxiv: '2112.01064'
    at_pub_source_title: 'AutoGEL: An Automated Graph Neural Network with Explicit
      Link Information'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.243
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.243
    sort_std: null
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'AutoGEL: An Automated Graph Neural Network with Explicit
      Link Information'
    comparison_source_arxiv: '2112.01064'
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
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    value: 0.9191
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_display: Nov 2024
    date_iso: '2024-11-09'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Zehong-Wang/GFT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9191
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: unigraph2
    model_plain: CompGCN
    value: 0.8786
    std: 0.0006
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.00806'
    title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
    date: Feb 2, 2025
    date_display: Feb 2025
    date_iso: '2025-02-02'
    venue: The Web Conference
    codebase_url: https://github.com/yf-he/UniGraph2
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8786
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CompGCN
    model_key: gat
    model_plain: CompGCN
    value: 0.8552
    std: 0.0012
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
    global_rank: 3
    sort_value: 0.8552
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimKGC-SymCL
    model_key: simkgc-symcl
    model_plain: SimKGC-SymCL
    value: 0.657
    std: null
    paper_value: 0.657
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.657
    sort_std: null
    global_rank: 23
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
  - model: SimKGC
    model_key: simkgc
    model_plain: SimKGC
    value: 0.652
    std: null
    paper_value: 0.652
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.652
    sort_std: null
    global_rank: 23
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
  - model: HAKE-SymCL
    model_key: hake-symcl
    model_plain: HAKE-SymCL
    value: 0.497
    std: null
    paper_value: 0.497
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.497
    sort_std: null
    global_rank: 32
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
  - model: HAKE
    model_key: hake
    model_plain: HAKE
    value: 0.497
    std: null
    paper_value: 0.497
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
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.497
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
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
    true_value: 0.497
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.497
    sort_std: null
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEX-DURA-SymCL
    model_key: complex-dura-symcl
    model_plain: ComplEX-DURA-SymCL
    value: 0.491
    std: null
    paper_value: 0.491
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.491
    sort_std: null
    global_rank: 34
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
  - model: ComplEX-DURA
    model_key: complex-dura
    model_plain: ComplEX-DURA
    value: 0.489
    std: null
    paper_value: 0.489
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.489
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.489
    sort_std: null
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
  - model: CompGCN
    model_key: compgcn
    model_plain: CompGCN
    value: 0.469
    std: null
    paper_value: 0.469
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.479
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.479
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.479
    sort_std: null
    global_rank: 46
    paper_rank: 52
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    comparison_source_arxiv: '1911.03082'
    is_best: false
    is_std_outlier: false
  - model: COMPGCN-SymCL
    model_key: compgcn-symcl
    model_plain: COMPGCN-SymCL
    value: 0.471
    std: null
    paper_value: 0.471
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.471
    sort_std: null
    global_rank: 51
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
  - model: RGCN-SymCL
    model_key: rgcn-symcl
    model_plain: RGCN-SymCL
    value: 0.432
    std: null
    paper_value: 0.432
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.432
    sort_std: null
    global_rank: 70
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.427
    std: null
    paper_value: 0.427
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.402
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.024999999999999967
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.427
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.427
    sort_std: null
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural
      Network Framework for Link Prediction'
    comparison_source_arxiv: '2106.06935'
    is_best: false
    is_std_outlier: false
  - model: DisMult-SymCL
    model_key: dismult-symcl
    model_plain: DisMult-SymCL
    value: 0.421
    std: null
    paper_value: 0.421
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.421
    sort_std: null
    global_rank: 74
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
  - model: DisMult
    model_key: dismult
    model_plain: DisMult
    value: 0.42
    std: null
    paper_value: 0.42
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
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.43
    at_pub_std: null
    at_pub_source_arxiv: '2112.01064'
    at_pub_source_title: 'AutoGEL: An Automated Graph Neural Network with Explicit
      Link Information'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.42
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.42
    sort_std: null
    global_rank: 74
    paper_rank: 74
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AutoGEL: An Automated Graph Neural Network with Explicit
      Link Information'
    comparison_source_arxiv: '2112.01064'
    is_best: false
    is_std_outlier: false
  - model: TransE-SymCL
    model_key: transe-symcl
    model_plain: TransE-SymCL
    value: 0.233
    std: null
    paper_value: 0.233
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
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
    sort_value: 0.233
    sort_std: null
    global_rank: 78
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
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.231
    std: null
    paper_value: 0.231
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 19, 2022
    date_display: Nov 2022
    date_iso: '2022-11-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.226
    at_pub_std: null
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.231
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.231
    sort_std: null
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    comparison_source_arxiv: '1902.10197'
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
main_figure: /figures/2211.10738/main_figure.jpegoptim.jpg
---

