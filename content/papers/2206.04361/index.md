---
title: Model Degradation Hinders Deep Graph Neural Networks
arxiv_id: '2206.04361'
source_url: ''
authors:
- name: Wentao Zhang
  orcid: null
  s2_author_id: '2108232566'
  s2_url: null
- name: Zeang Sheng
  orcid: null
  s2_author_id: '2120972284'
  s2_url: null
- name: Ziqi Yin
  orcid: null
  s2_author_id: '27036277'
  s2_url: null
- name: Yuezihan Jiang
  orcid: null
  s2_author_id: '2121246509'
  s2_url: null
- name: Yikuan Xia
  orcid: null
  s2_author_id: '1570458824'
  s2_url: null
- name: Jun Gao
  orcid: null
  s2_author_id: '2125047801'
  s2_url: null
- name: Zhi Yang
  orcid: null
  s2_author_id: '2109540175'
  s2_url: null
- name: Bin Cui
  orcid: null
  s2_author_id: '2068228300'
  s2_url: null
published_date: Jun 9, 2022
published_date_iso: '2022-06-09'
published_venue: KDD 2022
published_conference: KDD 2022
published_conference_short: KDD
published_conference_slug: kdd
abstract: 'Graph Neural Networks (GNNs) have achieved great success in various graph
  mining tasks. However, drastic performance degradation is always observed when a
  GNN is stacked with many layers. As a result, most GNNs only have shallow architectures,
  which limits their expressive power and exploitation of deep neighborhoods. Most
  recent studies attribute the performance degradation of deep GNNs to the over-smoothing
  issue. In this paper, we disentangle the conventional graph convolution operation
  into two independent operations: Propagation (P) and Transformation (T). Following
  this, the depth of a GNN can be split into the propagation depth ($D_p$) and the
  transformation depth ($D_t$). Through extensive experiments, we find that the major
  cause for the performance degradation of deep GNNs is the model degradation issue
  caused by large $D_t$ rather than the over-smoothing issue mainly caused by large
  $D_p$. Further, we present Adaptive Initial Residual (AIR), a plug-and-play module
  compatible with all kinds of GNN architectures, to alleviate the model degradation
  issue and the over-smoothing issue simultaneously. Experimental results on six real-world
  datasets demonstrate that GNNs equipped with AIR outperform most GNNs with shallow
  architectures owing to the benefits of both large $D_p$ and $D_t$, while the time
  costs associated with AIR can be ignored.'
codebase_url: https://github.com/PKU-DAIR/AIR
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
- GCN+AIR
mrr: 0.0431
adjusted_mrr: 0.0431
mrr_dataset_count: 4
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
    value: 0.6329
    std: 0.0019
    paper_value: 0.6329
    paper_std: 0.0019
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.661
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2111.00064'
    at_pub_source_title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood
      Prediction
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.028100000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.791
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.15810000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: null
    global_rank: 1
    paper_rank: 81
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
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
  - model: SGC+AIR
    model_key: sgc+air
    model_plain: SGC+AIR
    value: 0.6723
    std: 0.002
    paper_value: 0.6723
    paper_std: 0.002
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
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6723
    true_std: 0.002
    value_gap_source_arxiv: '2206.04361'
    value_gap_source_title: Model Degradation Hinders Deep Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6723
    sort_std: 0.002
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
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.6428
    std: 0.0014
    paper_value: 0.6428
    paper_std: 0.0014
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
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.6568
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.014000000000000012
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6636
    true_std: 0.0005
    value_gap_source_arxiv: '2504.13266'
    value_gap_source_title: 'Graph Learning at Scale: Characterizing and Optimizing
      Pre-Propagation GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.02079999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.6636
    sort_std: 0.0005
    global_rank: 42
    paper_rank: 73
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    comparison_source_arxiv: '2104.09376'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6483
    std: 0.0015
    paper_value: 0.6483
    paper_std: 0.0015
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.658
    at_pub_std: null
    at_pub_source_arxiv: '2111.06483'
    at_pub_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    at_pub_source_date_iso: '2021-11-11'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-11-11'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.009700000000000042
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.658
    true_std: null
    value_gap_source_arxiv: '2111.06483'
    value_gap_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.009700000000000042
    has_value_note: false
    value_note: ''
    sort_value: 0.658
    sort_std: null
    global_rank: 56
    paper_rank: 68
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    comparison_source_arxiv: '2111.06483'
    is_best: false
    is_std_outlier: false
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.6524
    std: 0.0013
    paper_value: 0.6524
    paper_std: 0.0013
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
    source_ref: ChenWDL00W20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.6523
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6524
    true_std: 0.0013
    value_gap_source_arxiv: '2206.04361'
    value_gap_source_title: Model Degradation Hinders Deep Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6524
    sort_std: 0.0013
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S^2GC
    model_key: s^2gc
    model_plain: S^2GC
    value: 0.6473
    std: 0.0021
    paper_value: 0.6473
    paper_std: 0.0021
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
    source_ref: zhu2021simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.647
    at_pub_std: 0.003
    at_pub_source_arxiv: '2108.00955'
    at_pub_source_title: Evaluating Deep Graph Neural Networks
    at_pub_source_date_iso: '2021-08-02'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6473
    true_std: 0.0021
    value_gap_source_arxiv: '2206.04361'
    value_gap_source_title: Model Degradation Hinders Deep Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6473
    sort_std: 0.0021
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.7768
    std: 0.0025
    paper_value: 0.7768
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
    source_ref: ChenWDL00W20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.835
    at_pub_std: 0.008
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.05819999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.835
    true_std: 0.008
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.05819999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.008
    global_rank: 72
    paper_rank: 228
    rank_delta: 156
    rank_delta_abs: 156
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.7683
    std: 0.0039
    paper_value: 0.7683
    paper_std: 0.0039
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
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.831
    at_pub_std: 0.008
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.06269999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.008
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.06269999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.008
    global_rank: 77
    paper_rank: 239
    rank_delta: 162
    rank_delta_abs: 162
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: S^2GC
    model_key: s^2gc
    model_plain: S^2GC
    value: 0.7713
    std: 0.0024
    paper_value: 0.7713
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
    source_ref: zhu2021simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.831
    at_pub_std: 0.007
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.059699999999999975
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.007
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.059699999999999975
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.007
    global_rank: 78
    paper_rank: 236
    rank_delta: 158
    rank_delta_abs: 158
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7829
    std: 0.0016
    paper_value: 0.7829
    paper_std: 0.0016
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.801
    at_pub_std: null
    at_pub_source_arxiv: '2111.06483'
    at_pub_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    at_pub_source_date_iso: '2021-11-11'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.018100000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8287
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04579999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8287
    sort_std: null
    global_rank: 82
    paper_rank: 220
    rank_delta: 138
    rank_delta_abs: 138
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sequential Aggregation and Rematerialization: Distributed
      Full-batch Training of Graph Neural Networks on Large Graphs'
    comparison_source_arxiv: '2111.06483'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7594
    std: 0.0022
    paper_value: 0.7594
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: 0.822
    at_pub_std: 0.009
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.06259999999999999
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
    value_gap: 0.06259999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.009
    global_rank: 93
    paper_rank: 251
    rank_delta: 158
    rank_delta_abs: 158
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: SGC+AIR
    model_key: sgc+air
    model_plain: SGC+AIR
    value: 0.8144
    std: 0.0016
    paper_value: 0.8144
    paper_std: 0.0016
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
    protocol_note: Test accuracy on node classification task
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: KDD 2022
    published_conference: KDD 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8144
    true_std: 0.0016
    value_gap_source_arxiv: '2206.04361'
    value_gap_source_title: Model Degradation Hinders Deep Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8144
    sort_std: 0.0016
    global_rank: 110
    paper_rank: 110
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
main_figure: /figures/2206.04361/main_figure.jpegoptim.jpg
---

