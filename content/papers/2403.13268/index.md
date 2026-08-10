---
title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
arxiv_id: '2403.13268'
source_url: ''
authors:
- name: Ningyi Liao
  orcid: null
  s2_author_id: '1940000983'
  s2_url: null
- name: Zihao Yu
  orcid: null
  s2_author_id: '2112220938'
  s2_url: null
- name: Siqiang Luo
  orcid: null
  s2_author_id: '2261689385'
  s2_url: null
published_date: Mar 19, 2024
published_date_iso: '2024-03-19'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: Graph Neural Networks (GNNs) have shown promising performance, but at the
  cost of resource-intensive operations on graph-scale matrices. To reduce computational
  overhead, previous studies attempt to sparsify the graph or network parameters,
  but with limited flexibility and precision boundaries. In this work, we propose
  Unifews, a joint sparsification technique to unify graph and weight matrix operations
  and enhance GNN learning efficiency. The Unifews design enables adaptive compression
  across GNN layers with progressively increased sparsity, and is applicable to a
  variety of architectures with on-the-fly simplification. Theoretically, we establish
  a novel framework to characterize sparsified GNN learning in view of the graph optimization
  process, showing that Unifews effectively approximates the learning objective with
  bounded error and reduced computational overhead. Extensive experiments demonstrate
  that Unifews achieves efficiency improvements with comparable or better accuracy,
  including 10-20x matrix operation reduction and up to 100x acceleration on graphs
  up to billion-edge scale.
codebase_url: https://github.com/gdmnl/Unifews
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Unifews
- SGC + Unifews
- APPNP + Unifews
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: ogbn-papers100M
  rows:
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.791
    std: null
    paper_value: 0.791
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-papers100m as per dataset
      statistics.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.661
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2111.00064'
    at_pub_source_title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood
      Prediction
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.13
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.791
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    comparison_source_arxiv: '2111.00064'
    is_best: true
    is_std_outlier: false
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.7036
    std: 0.0002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/AndyJZhao/GLEM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7036
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLEM-GNN
    model_key: glem-gnn
    model_plain: GLEM-GNN
    value: 0.7036
    std: 0.0002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/AndyJZhao/GLEM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7036
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.6644
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: Conference on Machine Learning and Systems
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 39
    sort_value: 0.6644
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC + Unifews
    model_key: sgc + unifews
    model_plain: SGC + Unifews
    value: 0.631
    std: null
    paper_value: 0.631
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-papers100m as per dataset
      statistics.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.631
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.631
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.609
    std: null
    paper_value: 0.609
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-papers100m as per dataset
      statistics.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6288
    true_std: 0.001
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: false
    value_gap: 0.01980000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.6288
    sort_std: 0.001
    global_rank: 85
    paper_rank: 91
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP + Unifews
    model_key: appnp + unifews
    model_plain: APPNP + Unifews
    value: 0.628
    std: null
    paper_value: 0.628
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-papers100m as per dataset
      statistics.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.628
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.628
    sort_std: null
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC + NIGCN
    model_key: sgc + nigcn
    model_plain: SGC + NIGCN
    value: 0.537
    std: null
    paper_value: 0.537
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-papers100m as per dataset
      statistics.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.537
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.537
    sort_std: null
    global_rank: 94
    paper_rank: 94
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
    value: 0.496
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.01535'
    title: 'Rethinking and Scaling Up Graph Contrastive Learning: An Extremely Efficient
      Approach with Group Discrimination'
    date: Jun 3, 2022
    date_display: Jun 2022
    date_iso: '2022-06-03'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/zyzisastudyreallyhardguy/Graph-Group-Discrimination
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 102
    sort_value: 0.496
    sort_std: 0.003
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
- &id001
  dataset: ogbn-products
  rows:
  - model: Jacobi
    model_key: jacobi
    model_plain: Jacobi
    value: 0.8968
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8968
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPR
    model_key: gpr
    model_plain: GPR
    value: 0.8953
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8953
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP4HG
    model_key: lemp4hg
    model_plain: LEMP4HG
    value: 0.8939
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8939
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8933
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 4
    sort_value: 0.8933
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.648
    std: null
    paper_value: 0.648
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-products with 8/2/90
      split.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.817
    at_pub_std: 0.003
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.16899999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8634
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.21539999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8634
    sort_std: null
    global_rank: 29
    paper_rank: 368
    rank_delta: 339
    rank_delta_abs: 339
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.688
    std: null
    paper_value: 0.688
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-products with 8/2/90
      split.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.822
    at_pub_std: 0.009
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.134
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.822
    true_std: 0.009
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.134
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.009
    global_rank: 93
    paper_rank: 351
    rank_delta: 258
    rank_delta_abs: 258
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: SGC + Unifews
    model_key: sgc + unifews
    model_plain: SGC + Unifews
    value: 0.694
    std: null
    paper_value: 0.694
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-products with 8/2/90
      split.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.694
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.694
    sort_std: null
    global_rank: 350
    paper_rank: 350
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
    value: 0.6605
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2211.16199'
    title: Latent Graph Inference using Product Manifolds
    date: Nov 26, 2022
    date_display: Nov 2022
    date_iso: '2022-11-26'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 361
    sort_value: 0.6605
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP + Unifews
    model_key: appnp + unifews
    model_plain: APPNP + Unifews
    value: 0.65
    std: null
    paper_value: 0.65
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-products with 8/2/90
      split.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.65
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.65
    sort_std: null
    global_rank: 367
    paper_rank: 367
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC + NIGCN
    model_key: sgc + nigcn
    model_plain: SGC + NIGCN
    value: 0.637
    std: null
    paper_value: 0.637
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ogbn-products with 8/2/90
      split.
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.637
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.637
    sort_std: null
    global_rank: 374
    paper_rank: 374
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
- benchmark: OGB
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
    - dataset: ogbn-papers100M
      dataset_slug: ogbn-papers100m
main_figure: /figures/2403.13268/main_figure.jpegoptim.jpg
---

