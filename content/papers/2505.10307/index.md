---
title: Negative Metric Learning for Graphs
arxiv_id: '2505.10307'
source_url: ''
authors:
- name: Yiyang Zhao
  orcid: null
  s2_author_id: '2366169339'
  s2_url: null
- name: Chengpei Wu
  orcid: null
  s2_author_id: '2350468873'
  s2_url: null
- name: Lili Zhang
  orcid: null
  s2_author_id: '2226224601'
  s2_url: null
- name: Ning Yang
  orcid: null
  s2_author_id: '2296194318'
  s2_url: null
published_date: May 15, 2025
published_date_iso: '2025-05-15'
published_venue: IJCAI 2025
published_conference: IJCAI 2025
published_conference_short: IJCAI
published_conference_slug: ijcai
abstract: Graph contrastive learning (GCL) often suffers from false negatives, which
  degrades the performance on downstream tasks. The existing methods addressing the
  false negative issue usually rely on human prior knowledge, still leading GCL to
  suboptimal results. In this paper, we propose a novel Negative Metric Learning (NML)
  enhanced GCL (NML-GCL). NML-GCL employs a learnable Negative Metric Network (NMN)
  to build a negative metric space, in which false negatives can be distinguished
  better from true negatives based on their distance to anchor node. To overcome the
  lack of explicit supervision signals for NML, we propose a joint training scheme
  with bi-level optimization objective, which implicitly utilizes the self-supervision
  signals to iteratively optimize the encoder and the negative metric network. The
  solid theoretical analysis and the extensive experiments conducted on widely used
  benchmarks verify the superiority of the proposed method.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NML-GCL
mrr: 0.0041
adjusted_mrr: 0.0041
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
    value: 0.9351
    std: 0.0006
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
    global_rank: 8
    sort_value: 0.9351
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8825
    std: 0.003
    paper_value: 0.8825
    paper_std: 0.003
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.9034
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02090000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9034
    true_std: 0.0019
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.02090000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9034
    sort_std: 0.0019
    global_rank: 110
    paper_rank: 239
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.879
    std: 0.0027
    paper_value: 0.879
    paper_std: 0.0027
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.8928
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.013800000000000034
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8955
    true_std: 0.0016
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.01649999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8955
    sort_std: 0.0016
    global_rank: 171
    paper_rank: 255
    rank_delta: 84
    rank_delta_abs: 84
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    comparison_source_arxiv: '2408.05087'
    is_best: false
    is_std_outlier: false
  - model: Local-GCL
    model_key: local-gcl
    model_plain: Local-GCL
    value: 0.8869
    std: 0.005
    paper_value: 0.8869
    paper_std: 0.005
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.8954
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2507.07141'
    at_pub_source_title: 'Str-GCL: Structural Commonsense Driven Graph Contrastive
      Learning'
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.008499999999999952
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8954
    true_std: 0.0032
    value_gap_source_arxiv: '2507.07141'
    value_gap_source_title: 'Str-GCL: Structural Commonsense Driven Graph Contrastive
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.008499999999999952
    has_value_note: false
    value_note: ''
    sort_value: 0.8954
    sort_std: 0.0032
    global_rank: 174
    paper_rank: 215
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Str-GCL: Structural Commonsense Driven Graph Contrastive
      Learning'
    comparison_source_arxiv: '2507.07141'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.8856
    std: 0.0031
    paper_value: 0.8856
    paper_std: 0.0031
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.8953
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.009699999999999931
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8953
    true_std: 0.0035
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.009699999999999931
    has_value_note: false
    value_note: ''
    sort_value: 0.8953
    sort_std: 0.0035
    global_rank: 176
    paper_rank: 223
    rank_delta: 47
    rank_delta_abs: 47
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
    is_best: false
    is_std_outlier: false
  - model: NML-GCL
    model_key: nml-gcl
    model_plain: NML-GCL
    value: 0.8943
    std: 0.0025
    paper_value: 0.8943
    paper_std: 0.0025
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8943
    true_std: 0.0025
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8943
    sort_std: 0.0025
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.8782
    std: 0.0048
    paper_value: 0.8782
    paper_std: 0.0048
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.89
    at_pub_std: 0.001
    at_pub_source_arxiv: '2409.08010'
    at_pub_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    at_pub_source_date_iso: '2024-09-12'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-09-12'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.011800000000000033
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.89
    true_std: 0.001
    value_gap_source_arxiv: '2409.08010'
    value_gap_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    value_gap_source_is_current_paper: false
    value_gap: 0.011800000000000033
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: 0.001
    global_rank: 196
    paper_rank: 258
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    comparison_source_arxiv: '2409.08010'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.8766
    std: 0.0025
    paper_value: 0.8766
    paper_std: 0.0025
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.8861
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2504.12011'
    at_pub_source_title: Balancing Graph Embedding Smoothness in Self-Supervised Learning
      via Information-Theoretic Decomposition
    at_pub_source_date_iso: '2025-04-16'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.009499999999999953
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8861
    true_std: 0.0064
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.009499999999999953
    has_value_note: false
    value_note: ''
    sort_value: 0.8861
    sort_std: 0.0064
    global_rank: 221
    paper_rank: 271
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    comparison_source_arxiv: '2504.12011'
    is_best: false
    is_std_outlier: false
  - model: GRAPE
    model_key: grape
    model_plain: GRAPE
    value: 0.8797
    std: 0.0033
    paper_value: 0.8797
    paper_std: 0.0033
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8797
    true_std: 0.0033
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: 0.0033
    global_rank: 253
    paper_rank: 253
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PHASES
    model_key: phases
    model_plain: PHASES
    value: 0.878
    std: 0.0044
    paper_value: 0.878
    paper_std: 0.0044
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.878
    true_std: 0.0044
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.878
    sort_std: 0.0044
    global_rank: 263
    paper_rank: 263
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8463
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11907'
    title: 'GraphFM: A generalist graph transformer that learns transferable representations
      across diverse domains'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/nerdslab/GraphFM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 365
    sort_value: 0.8463
    sort_std: null
    comparison_type: global_top
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
- &id003
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
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
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9669
    std: 0.0014
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
    sort_value: 0.9669
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
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
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.9271
    std: 0.0029
    paper_value: 0.9271
    paper_std: 0.0029
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.9381
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2311.02687'
    at_pub_source_title: 'Architecture Matters: Uncovering Implicit Mechanisms in
      Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-11-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-11-05'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9381
    true_std: 0.0048
    value_gap_source_arxiv: '2311.02687'
    value_gap_source_title: 'Architecture Matters: Uncovering Implicit Mechanisms
      in Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9381
    sort_std: 0.0048
    global_rank: 140
    paper_rank: 285
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Architecture Matters: Uncovering Implicit Mechanisms
      in Graph Contrastive Learning'
    comparison_source_arxiv: '2311.02687'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.9301
    std: 0.0027
    paper_value: 0.9301
    paper_std: 0.0027
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.9337
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2206.12933'
    at_pub_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9337
    true_std: 0.0021
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0035999999999999366
    has_value_note: false
    value_note: ''
    sort_value: 0.9337
    sort_std: 0.0021
    global_rank: 198
    paper_rank: 245
    rank_delta: 47
    rank_delta_abs: 47
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NML-GCL
    model_key: nml-gcl
    model_plain: NML-GCL
    value: 0.9336
    std: 0.0021
    paper_value: 0.9336
    paper_std: 0.0021
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9336
    true_std: 0.0021
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9336
    sort_std: 0.0021
    global_rank: 200
    paper_rank: 200
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Local-GCL
    model_key: local-gcl
    model_plain: Local-GCL
    value: 0.9283
    std: 0.0028
    paper_value: 0.9283
    paper_std: 0.0028
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.9325
    at_pub_std: 0.004
    at_pub_source_arxiv: '2212.04604'
    at_pub_source_title: Localized Graph Contrastive Learning
    at_pub_source_date_iso: '2022-12-08'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-08'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0041999999999999815
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9325
    true_std: 0.004
    value_gap_source_arxiv: '2212.04604'
    value_gap_source_title: Localized Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0041999999999999815
    has_value_note: false
    value_note: ''
    sort_value: 0.9325
    sort_std: 0.004
    global_rank: 214
    paper_rank: 262
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.9273
    std: 0.0035
    paper_value: 0.9273
    paper_std: 0.0035
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.928
    at_pub_std: 0.005
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-25'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0007000000000000339
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9313
    true_std: 0.0017
    value_gap_source_arxiv: '2505.19024'
    value_gap_source_title: Learn Beneficial Noise as Graph Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.9313
    sort_std: 0.0017
    global_rank: 229
    paper_rank: 284
    rank_delta: 55
    rank_delta_abs: 55
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.9259
    std: 0.0034
    paper_value: 0.9259
    paper_std: 0.0034
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.931
    at_pub_std: 0.004
    at_pub_source_arxiv: '2403.01400'
    at_pub_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    at_pub_source_date_iso: '2024-03-03'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0051000000000001044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.931
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.0051000000000001044
    has_value_note: false
    value_note: ''
    sort_value: 0.931
    sort_std: 0.004
    global_rank: 232
    paper_rank: 303
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.9231
    std: 0.0036
    paper_value: 0.9231
    paper_std: 0.0036
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.93
    at_pub_std: 0.002
    at_pub_source_arxiv: '2409.08010'
    at_pub_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    at_pub_source_date_iso: '2024-09-12'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-09-12'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.006900000000000017
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.93
    true_std: 0.002
    value_gap_source_arxiv: '2409.08010'
    value_gap_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    value_gap_source_is_current_paper: false
    value_gap: 0.006900000000000017
    has_value_note: false
    value_note: ''
    sort_value: 0.93
    sort_std: 0.002
    global_rank: 249
    paper_rank: 340
    rank_delta: 91
    rank_delta_abs: 91
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multiplex Graph Contrastive Learning with Soft Negatives
    comparison_source_arxiv: '2409.08010'
    is_best: false
    is_std_outlier: false
  - model: repl. cosine sim.
    model_key: repl. cosine sim.
    model_plain: repl. cosine sim.
    value: 0.928
    std: 0.0022
    paper_value: 0.928
    paper_std: 0.0022
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.928
    true_std: 0.0022
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.0022
    global_rank: 272
    paper_rank: 272
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAPE
    model_key: grape
    model_plain: GRAPE
    value: 0.9276
    std: 0.003
    paper_value: 0.9276
    paper_std: 0.003
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9276
    true_std: 0.003
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9276
    sort_std: 0.003
    global_rank: 279
    paper_rank: 279
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PHASES
    model_key: phases
    model_plain: PHASES
    value: 0.9274
    std: 0.0037
    paper_value: 0.9274
    paper_std: 0.0037
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
    protocol_note: 1:1:8 training/validation/testing split as per text
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9274
    true_std: 0.0037
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9274
    sort_std: 0.0037
    global_rank: 283
    paper_rank: 283
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9128
    std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 426
    sort_value: 0.9128
    sort_std: 0.0063
    comparison_type: global_top
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
- &id002
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7046
    std: 0.0023
    paper_value: 0.7046
    paper_std: 0.0023
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.7808
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07620000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7808
    true_std: 0.0006
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.07620000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0006
    global_rank: 108
    paper_rank: 657
    rank_delta: 549
    rank_delta_abs: 549
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7227
    std: 0.0026
    paper_value: 0.7227
    paper_std: 0.0026
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.76
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0373
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.0373
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.002
    global_rank: 171
    paper_rank: 491
    rank_delta: 320
    rank_delta_abs: 320
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7057
    std: 0.0053
    paper_value: 0.7057
    paper_std: 0.0053
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.745
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0393
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.0393
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 649
    rank_delta: 404
    rank_delta_abs: 404
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: NML-GCL
    model_key: nml-gcl
    model_plain: NML-GCL
    value: 0.7337
    std: 0.0013
    paper_value: 0.7337
    paper_std: 0.0013
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7337
    true_std: 0.0013
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7337
    sort_std: 0.0013
    global_rank: 339
    paper_rank: 339
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7289
    std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 401
    sort_value: 0.7289
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAPE
    model_key: grape
    model_plain: GRAPE
    value: 0.7234
    std: 0.0022
    paper_value: 0.7234
    paper_std: 0.0022
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7234
    true_std: 0.0022
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7234
    sort_std: 0.0022
    global_rank: 475
    paper_rank: 475
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.7011
    std: 0.0079
    paper_value: 0.7011
    paper_std: 0.0079
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.723
    at_pub_std: 0.007
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.02190000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.723
    true_std: 0.007
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.02190000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.007
    global_rank: 479
    paper_rank: 679
    rank_delta: 200
    rank_delta_abs: 200
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    comparison_source_arxiv: '2306.09614'
    is_best: false
    is_std_outlier: false
  - model: Local-GCL
    model_key: local-gcl
    model_plain: Local-GCL
    value: 0.7178
    std: 0.0048
    paper_value: 0.7178
    paper_std: 0.0048
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7178
    true_std: 0.0048
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7178
    sort_std: 0.0048
    global_rank: 536
    paper_rank: 536
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: repl. cosine sim.
    model_key: repl. cosine sim.
    model_plain: repl. cosine sim.
    value: 0.7118
    std: 0.0024
    paper_value: 0.7118
    paper_std: 0.0024
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7118
    true_std: 0.0024
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7118
    sort_std: 0.0024
    global_rank: 608
    paper_rank: 608
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.7063
    std: 0.0022
    paper_value: 0.7063
    paper_std: 0.0022
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.698
    at_pub_std: 0.005
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.008300000000000085
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7063
    true_std: 0.0022
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7063
    sort_std: 0.0022
    global_rank: 644
    paper_rank: 644
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    comparison_source_arxiv: '2306.09614'
    is_best: false
    is_std_outlier: false
  - model: PHASES
    model_key: phases
    model_plain: PHASES
    value: 0.7049
    std: 0.004
    paper_value: 0.7049
    paper_std: 0.004
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7049
    true_std: 0.004
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7049
    sort_std: 0.004
    global_rank: 654
    paper_rank: 654
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
- &id001
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
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7941
    std: 0.0023
    paper_value: 0.7941
    paper_std: 0.0023
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.883
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08889999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.883
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08889999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.883
    sort_std: 0.001
    global_rank: 167
    paper_rank: 577
    rank_delta: 410
    rank_delta_abs: 410
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.8113
    std: 0.0031
    paper_value: 0.8113
    paper_std: 0.0031
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.873
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06169999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.06169999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 224
    paper_rank: 412
    rank_delta: 188
    rank_delta_abs: 188
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7863
    std: 0.0027
    paper_value: 0.7863
    paper_std: 0.0027
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.8725
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08620000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8725
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.08620000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8725
    sort_std: 0.0012
    global_rank: 226
    paper_rank: 692
    rank_delta: 466
    rank_delta_abs: 466
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.869
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 243
    sort_value: 0.869
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NML-GCL
    model_key: nml-gcl
    model_plain: NML-GCL
    value: 0.821
    std: 0.003
    paper_value: 0.821
    paper_std: 0.003
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.821
    true_std: 0.003
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.821
    sort_std: 0.003
    global_rank: 373
    paper_rank: 373
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.8102
    std: 0.0068
    paper_value: 0.8102
    paper_std: 0.0068
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.811
    at_pub_std: 0.003
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.0008000000000000229
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.003
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.0008000000000000229
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.003
    global_rank: 414
    paper_rank: 419
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PHASES
    model_key: phases
    model_plain: PHASES
    value: 0.8108
    std: 0.0062
    paper_value: 0.8108
    paper_std: 0.0062
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8108
    true_std: 0.0062
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8108
    sort_std: 0.0062
    global_rank: 419
    paper_rank: 419
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Local-GCL
    model_key: local-gcl
    model_plain: Local-GCL
    value: 0.8095
    std: 0.0041
    paper_value: 0.8095
    paper_std: 0.0041
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-15'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8095
    true_std: 0.0041
    value_gap_source_arxiv: '2505.10307'
    value_gap_source_title: Negative Metric Learning for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8095
    sort_std: 0.0041
    global_rank: 425
    paper_rank: 425
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    value: 0.7814
    std: 0.0043
    paper_value: 0.7814
    paper_std: 0.0043
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
    protocol_note: Planetoid split as per Yang et al. 2016
    date: May 15, 2025
    date_display: May 2025
    date_iso: '2025-05-15'
    published_venue: IJCAI 2025
    published_conference: IJCAI 2025
    at_pub_value: 0.792
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-06-16'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.010600000000000054
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.792
    true_std: 0.002
    value_gap_source_arxiv: '2306.09614'
    value_gap_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.010600000000000054
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.002
    global_rank: 611
    paper_rank: 730
    rank_delta: 119
    rank_delta_abs: 119
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    comparison_source_arxiv: '2306.09614'
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
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
single_proposed_model: NML-GCL
main_figure: /figures/2505.10307/main_figure.jpegoptim.jpg
---

