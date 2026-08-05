---
title: Deep Temporal Graph Clustering
arxiv_id: '2305.10738'
source_url: ''
authors:
- name: Meng Liu
  orcid: null
  s2_author_id: '2152969291'
  s2_url: null
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: K. Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Siwei Wang
  orcid: null
  s2_author_id: '103307910'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
published_date: May 18, 2023
published_date_iso: '2023-05-18'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Deep graph clustering has recently received significant attention due to
  its ability to enhance the representation learning capabilities of models in unsupervised
  scenarios. Nevertheless, deep clustering for temporal graphs, which could capture
  crucial dynamic interaction information, has not been fully explored. It means that
  in many clustering-oriented real-world scenarios, temporal graphs can only be processed
  as static graphs. This not only causes the loss of dynamic information but also
  triggers huge computational consumption. To solve the problem, we propose a general
  framework for deep Temporal Graph Clustering called TGC, which introduces deep clustering
  techniques to suit the interaction sequence-based batch-processing pattern of temporal
  graphs. In addition, we discuss differences between temporal graph clustering and
  static graph clustering from several levels. To verify the superiority of the proposed
  framework TGC, we conduct extensive experiments. The experimental results show that
  temporal graph clustering enables more flexibility in finding a balance between
  time and space requirements, and our framework can effectively improve the performance
  of existing temporal graph learning methods. The code is released:.
codebase_url: https://github.com/MGitHubL/Deep-Temporal-Graph-Clustering
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TGC
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: DBLP
  rows:
  - model: AUG_bal
    model_key: aug_bal
    model_plain: AUG_bal
    value: 0.9454
    std: 0.0123
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    venue: International Conference on Information and Knowledge Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9454
    sort_std: 0.0123
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AUG_min
    model_key: aug_min
    model_plain: AUG_min
    value: 0.9375
    std: 0.0115
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    venue: International Conference on Information and Knowledge Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9375
    sort_std: 0.0115
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AUG_ran
    model_key: aug_ran
    model_plain: AUG_ran
    value: 0.9368
    std: 0.0108
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    venue: International Conference on Information and Knowledge Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9368
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.3504
    std: null
    paper_value: 0.3504
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.768
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-03-21'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.4176
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.768
    true_std: null
    value_gap_source_arxiv: '2203.10866'
    value_gap_source_title: Unsupervised Network Embedding Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.4176
    has_value_note: false
    value_note: ''
    sort_value: 0.768
    sort_std: null
    global_rank: 35
    paper_rank: 60
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    value: 0.3597
    std: null
    paper_value: 0.3597
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.757
    true_std: 0.008
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.3973
    has_value_note: false
    value_note: ''
    sort_value: 0.757
    sort_std: 0.008
    global_rank: 36
    paper_rank: 59
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AE
    model_key: ae
    model_plain: AE
    value: 0.3784
    std: null
    paper_value: 0.3784
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.746
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-03-21'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.3676
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.746
    true_std: null
    value_gap_source_arxiv: '2203.10866'
    value_gap_source_title: Unsupervised Network Embedding Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.3676
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: null
    global_rank: 37
    paper_rank: 59
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.732
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.10866'
    title: Unsupervised Network Embedding Beyond Homophily
    date: Mar 21, 2022
    date_display: Mar 2022
    date_iso: '2022-03-21'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/zhiqiangzhongddu/SELENE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 39
    sort_value: 0.732
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    value: 0.4031
    std: null
    paper_value: 0.4031
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.638
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2024-06-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2349
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6771
    true_std: 0.0151
    value_gap_source_arxiv: '2406.15797'
    value_gap_source_title: 'SynC: Synergistic Boosting of Structure and Representation
      for Deep Graph Clustering'
    value_gap_source_is_current_paper: false
    value_gap: 0.274
    has_value_note: false
    value_note: ''
    sort_value: 0.6771
    sort_std: 0.0151
    global_rank: 42
    paper_rank: 58
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.2479
    std: null
    paper_value: 0.2479
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.55
    true_std: 0.07
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.30210000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.55
    sort_std: 0.07
    global_rank: 50
    paper_rank: 63
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGC
    model_key: tgc
    model_plain: TGC
    value: 0.4503
    std: null
    paper_value: 0.4503
    paper_std: null
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4503
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4503
    sort_std: null
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TREND
    model_key: trend
    model_plain: TREND
    value: 0.4454
    std: null
    paper_value: 0.4454
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4454
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4454
    sort_std: null
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HTNE
    model_key: htne
    model_plain: HTNE
    value: 0.4398
    std: null
    paper_value: 0.4398
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4398
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4398
    sort_std: null
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4335
    std: null
    paper_value: 0.4335
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4335
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4335
    sort_std: null
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.3856
    std: null
    paper_value: 0.3856
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3856
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3856
    sort_std: null
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDCNQ
    model_key: sdcnq
    model_plain: SDCNQ
    value: 0.3518
    std: null
    paper_value: 0.3518
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3518
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3518
    sort_std: null
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.3422
    std: null
    paper_value: 0.3422
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3422
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3422
    sort_std: null
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.1323
    std: null
    paper_value: 0.1323
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1323
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1323
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.1066
    std: null
    paper_value: 0.1066
    paper_std: null
    metric: F1
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
    protocol_note: Node clustering task on DBLP
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1066
    true_std: null
    value_gap_source_arxiv: '2305.10738'
    value_gap_source_title: Deep Temporal Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1066
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
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
single_proposed_model: TGC
main_figure: /figures/2305.10738/main_figure.jpegoptim.jpg
---

