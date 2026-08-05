---
title: Relation-Aware Graph Foundation Model
arxiv_id: '2505.12027'
source_url: ''
authors:
- name: Jianxiang Yu
  orcid: null
  s2_author_id: '2198507600'
  s2_url: null
- name: Jiapeng Zhu
  orcid: null
  s2_author_id: '2274978444'
  s2_url: null
- name: Hao Qian
  orcid: null
  s2_author_id: '2283849121'
  s2_url: null
- name: Ziqi Liu
  orcid: null
  s2_author_id: '2285057064'
  s2_url: null
- name: Zhiqiang Zhang
  orcid: null
  s2_author_id: '2266809812'
  s2_url: null
- name: Xiang Li
  orcid: null
  s2_author_id: '2258789569'
  s2_url: null
published_date: May 17, 2025
published_date_iso: '2025-05-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: In recent years, large language models (LLMs) have demonstrated remarkable
  generalization capabilities across various natural language processing (NLP) tasks.
  Similarly, graph foundation models (GFMs) have emerged as a promising direction
  in graph learning, aiming to generalize across diverse datasets through large-scale
  pre-training. However, unlike language models that rely on explicit token representations,
  graphs lack a well-defined unit for generalization, making it challenging to design
  effective pre-training strategies. In this work, we propose REEF, a novel framework
  that leverages relation tokens as the basic units for GFMs. Inspired by the token
  vocabulary in LLMs, we construct a relation vocabulary of relation tokens to store
  relational information within graphs. To accommodate diverse relations, we introduce
  two hypernetworks that adaptively generate the parameters of aggregators and classifiers
  in graph neural networks based on relation tokens. In addition, we design another
  hypernetwork to construct dataset-specific projectors and incorporate a dataset-level
  feature bias into the initial node representations, enhancing flexibility across
  different datasets with the same relation. Further, we adopt graph data augmentation
  and a mixed-dataset pre-training strategy, allowing REEF to capture relational diversity
  more effectively and exhibit strong generalization capabilities. Extensive experiments
  show that REEF significantly outperforms existing methods on both pre-training and
  transfer learning tasks, underscoring its potential as a powerful foundation model
  for graph-based applications.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- REEF
- REEF-LM
- REEF-FB
- REEF-FP
- REEF-AGU
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: WN18RR
  rows:
  - model: REEF-AGU
    model_key: ofa-llama2-13b
    model_plain: REEF-AGU
    value: 0.9814
    std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.00149'
    title: 'One for All: Towards Training One Graph Model for All Classification Tasks'
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/LechengKong/OneForAll
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9814
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: REEF-AGU
    model_key: ofa-llama2-7b
    model_plain: REEF-AGU
    value: 0.9808
    std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.00149'
    title: 'One for All: Towards Training One Graph Model for All Classification Tasks'
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/LechengKong/OneForAll
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9808
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: REEF-AGU
    model_key: ofa-e5
    model_plain: REEF-AGU
    value: 0.9784
    std: 0.0035
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.00149'
    title: 'One for All: Towards Training One Graph Model for All Classification Tasks'
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/LechengKong/OneForAll
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9784
    sort_std: 0.0035
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: REEF
    model_key: reef
    model_plain: REEF
    value: 0.947
    std: null
    paper_value: 0.947
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.947
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.947
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
  - model: REEF-FP
    model_key: reef-fp
    model_plain: REEF-FP
    value: 0.9429
    std: null
    paper_value: 0.9429
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Ablation study on pre-training task for W18RR.
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9429
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9429
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
  - model: REEF-LM
    model_key: reef-lm
    model_plain: REEF-LM
    value: 0.9406
    std: null
    paper_value: 0.9406
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Ablation study on pre-training task for WN18RR.
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9406
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9406
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.7899
    std: null
    paper_value: 0.7899
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9387
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2412.16441'
    at_pub_source_title: 'Towards Graph Foundation Models: Learning Generalities Across
      Graphs via Task-Trees'
    at_pub_source_date_iso: '2024-12-21'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.14879999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9387
    true_std: 0.0035
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.14879999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9387
    sort_std: 0.0035
    global_rank: 11
    paper_rank: 21
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    comparison_source_arxiv: '2412.16441'
    is_best: false
    is_std_outlier: false
  - model: REEF-AGU
    model_key: reef-agu
    model_plain: REEF-AGU
    value: 0.9378
    std: null
    paper_value: 0.9378
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Ablation study on pre-training task for WN18RR.
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9378
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9378
    sort_std: null
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: REEF-FB
    model_key: reef-fb
    model_plain: REEF-FB
    value: 0.9218
    std: null
    paper_value: 0.9218
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Ablation study on pre-training task for WN18RR.
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9218
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9218
    sort_std: null
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
  - model: GFT
    model_key: gft
    model_plain: GFT
    value: 0.9191
    std: null
    paper_value: 0.9191
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9191
    true_std: null
    value_gap_source_arxiv: '2505.12027'
    value_gap_source_title: Relation-Aware Graph Foundation Model
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9191
    sort_std: null
    global_rank: 16
    paper_rank: 16
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
    value: 0.7379
    std: null
    paper_value: 0.7379
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8677
    at_pub_std: 0.003
    at_pub_source_arxiv: '2412.16441'
    at_pub_source_title: 'Towards Graph Foundation Models: Learning Generalities Across
      Graphs via Task-Trees'
    at_pub_source_date_iso: '2024-12-21'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.12980000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8677
    true_std: 0.003
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.12980000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8677
    sort_std: 0.003
    global_rank: 18
    paper_rank: 25
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    comparison_source_arxiv: '2412.16441'
    is_best: false
    is_std_outlier: false
  - model: GIANT
    model_key: giant
    model_plain: GIANT
    value: 0.8436
    std: null
    paper_value: 0.8436
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8436
    true_std: 0.003
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8436
    sort_std: 0.003
    global_rank: 20
    paper_rank: 20
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
    value: 0.8016
    std: null
    paper_value: 0.8016
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8016
    true_std: 0.0027
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8016
    sort_std: 0.0027
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
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.785
    std: null
    paper_value: 0.785
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.785
    true_std: 0.0059
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.785
    sort_std: 0.0059
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7575
    std: null
    paper_value: 0.7575
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7575
    true_std: 0.009
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7575
    sort_std: 0.009
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7544
    std: null
    paper_value: 0.7544
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7544
    true_std: 0.003
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7544
    sort_std: 0.003
    global_rank: 24
    paper_rank: 24
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
    value: 0.7402
    std: null
    paper_value: 0.7402
    paper_std: null
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR split as described in experimental
      settings (142, 47, 48).
    date: May 17, 2025
    date_display: May 2025
    date_iso: '2025-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.573
    at_pub_std: 0.034
    at_pub_source_arxiv: '2310.00149'
    at_pub_source_title: 'One for All: Towards Training One Graph Model for All Classification
      Tasks'
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: 0.16720000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7402
    true_std: 0.0055
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7402
    sort_std: 0.0055
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    comparison_source_arxiv: '2310.00149'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
main_figure: /figures/2505.12027/main_figure.jpegoptim.jpg
---

