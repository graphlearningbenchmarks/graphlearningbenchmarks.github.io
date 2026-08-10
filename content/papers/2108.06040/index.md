---
title: Knowledge Graph Reasoning with Relational Digraph
arxiv_id: '2108.06040'
source_url: ''
authors:
- name: Yongqi Zhang
  orcid: null
  s2_author_id: '48379419'
  s2_url: null
- name: Quanming Yao
  orcid: null
  s2_author_id: '3259992'
  s2_url: null
published_date: Aug 13, 2021
published_date_iso: '2021-08-13'
published_venue: WWW 2021
published_conference: WWW 2021
published_conference_short: WWW
published_conference_slug: www
abstract: Reasoning on the knowledge graph (KG) aims to infer new facts from existing
  ones. Methods based on the relational path have shown strong, interpretable, and
  transferable reasoning ability. However, paths are naturally limited in capturing
  local evidence in graphs. In this paper, we introduce a novel relational structure,
  i.e., relational directed graph (r-digraph), which is composed of overlapped relational
  paths, to capture the KG's local evidence. Since the r-digraphs are more complex
  than paths, how to efficiently construct and effectively learn from them are challenging.
  Directly encoding the r-digraphs cannot scale well and capturing query-dependent
  information is hard in r-digraphs. We propose a variant of graph neural network,
  i.e., RED-GNN, to address the above challenges. Specifically, RED-GNN makes use
  of dynamic programming to recursively encodes multiple r-digraphs with shared edges,
  and utilizes query-dependent attention mechanism to select the strongly correlated
  edges. We demonstrate that RED-GNN is not only efficient but also can achieve significant
  performance gains in both inductive and transductive reasoning tasks over existing
  methods. Besides, the learned attention weights in RED-GNN can exhibit interpretable
  evidence for KG reasoning.. Correspondence is to Q. Yao.
codebase_url: https://github.com/LARS-research/RED-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- RED-GNN
mrr: 0.0311
adjusted_mrr: 0.0208
mrr_dataset_count: 2
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
  - model: GraIL
    model_key: grail
    model_plain: GraIL
    value: 0.279
    std: null
    paper_value: 0.279
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.642
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.363
    has_value_note: false
    value_note: ''
    sort_value: 0.642
    sort_std: null
    global_rank: 17
    paper_rank: 94
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRUM
    model_key: drum
    model_plain: DRUM
    value: 0.343
    std: null
    paper_value: 0.343
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.343
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.529
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.186
    has_value_note: false
    value_note: ''
    sort_value: 0.529
    sort_std: null
    global_rank: 19
    paper_rank: 65
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RuleN
    model_key: rulen
    model_plain: RuleN
    value: 0.363
    std: null
    paper_value: 0.363
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.498
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.135
    has_value_note: false
    value_note: ''
    sort_value: 0.498
    sort_std: null
    global_rank: 21
    paper_rank: 38
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RED-GNN
    model_key: red-gnn
    model_plain: RED-GNN
    value: 0.374
    std: null
    paper_value: 0.374
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.374
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.374
    sort_std: null
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
  - model: DPMPN
    model_key: dpmpn
    model_plain: DPMPN
    value: 0.369
    std: null
    paper_value: 0.369
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    true_value: 0.369
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: QuatE
    model_key: quate
    model_plain: QuatE
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.366
    at_pub_std: null
    at_pub_source_arxiv: '2009.14332'
    at_pub_source_title: Multi-hop Attention Graph Neural Networks
    at_pub_source_date_iso: '2020-09-29'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.366
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.016000000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.366
    sort_std: null
    global_rank: 36
    paper_rank: 55
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-hop Attention Graph Neural Networks
    comparison_source_arxiv: '2009.14332'
    is_best: false
    is_std_outlier: false
  - model: CompGCN
    model_key: compgcn
    model_plain: CompGCN
    value: 0.355
    std: null
    paper_value: 0.355
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.355
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-09-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.355
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.355
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RNNLogic
    model_key: rnnlogic
    model_plain: RNNLogic
    value: 0.344
    std: null
    paper_value: 0.344
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.344
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.344
    sort_std: null
    global_rank: 65
    paper_rank: 65
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
    value: 0.337
    std: null
    paper_value: 0.337
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.338
    at_pub_std: null
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-25'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.338
    true_std: null
    value_gap_source_arxiv: '2302.13083'
    value_gap_source_title: Knowledge Graph Completion with Counterfactual Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.338
    sort_std: null
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    comparison_source_arxiv: '1902.10197'
    is_best: false
    is_std_outlier: false
  - model: pLogicNet
    model_key: plogicnet
    model_plain: pLogicNet
    value: 0.332
    std: null
    paper_value: 0.332
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    true_value: 0.332
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.332
    sort_std: null
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Neural LP
    model_key: neural lp
    model_plain: Neural LP
    value: 0.325
    std: null
    paper_value: 0.325
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-13'
    value_gap_source_date_label: WWW 2021
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
    value_gap_source_arxiv: '2108.06040'
    value_gap_source_title: Knowledge Graph Reasoning with Relational Digraph
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.325
    sort_std: null
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
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
    source_ref: original papers
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.325
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
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
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MINERVA
    model_key: minerva
    model_plain: MINERVA
    value: 0.293
    std: null
    paper_value: 0.293
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.293
    true_std: null
    value_gap_source_arxiv: '2206.04798'
    value_gap_source_title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.293
    sort_std: null
    global_rank: 91
    paper_rank: 91
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
    global_rank: 25
    sort_value: 0.8298
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraIL
    model_key: grail
    model_plain: GraIL
    value: 0.627
    std: null
    paper_value: 0.627
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.825
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.19799999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.825
    sort_std: null
    global_rank: 26
    paper_rank: 40
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RuleN
    model_key: rulen
    model_plain: RuleN
    value: 0.668
    std: null
    paper_value: 0.668
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.809
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.14100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.809
    sort_std: null
    global_rank: 29
    paper_rank: 36
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRUM
    model_key: drum
    model_plain: DRUM
    value: 0.666
    std: null
    paper_value: 0.666
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.486
    at_pub_std: null
    at_pub_source_arxiv: '2106.06935'
    at_pub_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural Network
      Framework for Link Prediction'
    at_pub_source_date_iso: '2021-06-13'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-02-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.18000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.744
    true_std: null
    value_gap_source_arxiv: '2302.02209'
    value_gap_source_title: A Theory of Link Prediction via Relational Weisfeiler-Leman
      on Knowledge Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.07799999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.744
    sort_std: null
    global_rank: 35
    paper_rank: 36
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Neural Bellman-Ford Networks: A General Graph Neural
      Network Framework for Link Prediction'
    comparison_source_arxiv: '2106.06935'
    is_best: false
    is_std_outlier: false
  - model: RED-GNN
    model_key: red-gnn
    model_plain: RED-GNN
    value: 0.701
    std: null
    paper_value: 0.701
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-13'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.701
    true_std: null
    value_gap_source_arxiv: '2108.06040'
    value_gap_source_title: Knowledge Graph Reasoning with Relational Digraph
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.701
    sort_std: null
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Neural LP
    model_key: neural lp
    model_plain: Neural LP
    value: 0.649
    std: null
    paper_value: 0.649
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-13'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.649
    true_std: null
    value_gap_source_arxiv: '2108.06040'
    value_gap_source_title: Knowledge Graph Reasoning with Relational Digraph
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.649
    sort_std: null
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: QuatE
    model_key: quate
    model_plain: QuatE
    value: 0.48
    std: null
    paper_value: 0.48
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.488
    at_pub_std: null
    at_pub_source_arxiv: '2009.14332'
    at_pub_source_title: Multi-hop Attention Graph Neural Networks
    at_pub_source_date_iso: '2020-09-29'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.488
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.008000000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: null
    global_rank: 69
    paper_rank: 76
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-hop Attention Graph Neural Networks
    comparison_source_arxiv: '2009.14332'
    is_best: false
    is_std_outlier: false
  - model: RNNLogic
    model_key: rnnlogic
    model_plain: RNNLogic
    value: 0.483
    std: null
    paper_value: 0.483
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.483
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.483
    sort_std: null
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DPMPN
    model_key: dpmpn
    model_plain: DPMPN
    value: 0.482
    std: null
    paper_value: 0.482
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    true_value: 0.482
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.482
    sort_std: null
    global_rank: 74
    paper_rank: 74
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
    value: 0.479
    std: null
    paper_value: 0.479
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.479
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-09-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.479
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.479
    sort_std: null
    global_rank: 81
    paper_rank: 81
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
    value: 0.477
    std: null
    paper_value: 0.477
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.477
    at_pub_std: 0.001
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2024-09-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.477
    true_std: null
    value_gap_source_arxiv: '2409.12865'
    value_gap_source_title: 'KnowFormer: Revisiting Transformers for Knowledge Graph
      Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.477
    sort_std: null
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.43
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
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
    global_rank: 97
    paper_rank: 109
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MINERVA
    model_key: minerva
    model_plain: MINERVA
    value: 0.448
    std: null
    paper_value: 0.448
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    true_value: 0.448
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.448
    sort_std: null
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: pLogicNet
    model_key: plogicnet
    model_plain: pLogicNet
    value: 0.441
    std: null
    paper_value: 0.441
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
    date: Aug 13, 2021
    date_display: Aug 2021
    date_iso: '2021-08-13'
    published_venue: WWW 2021
    published_conference: WWW 2021
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
    true_value: 0.441
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.441
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
single_proposed_model: RED-GNN
main_figure: /figures/2108.06040/main_figure.jpegoptim.jpg
---

