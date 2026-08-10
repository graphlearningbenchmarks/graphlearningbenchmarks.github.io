---
title: Learning on Large-scale Text-attributed Graphs via Variational Inference
arxiv_id: '2210.14709'
source_url: ''
authors:
- name: Jianan Zhao
  orcid: null
  s2_author_id: '48018967'
  s2_url: null
- name: Meng Qu
  orcid: null
  s2_author_id: '145252498'
  s2_url: null
- name: Chaozhuo Li
  orcid: null
  s2_author_id: '2869810'
  s2_url: null
- name: Hao Yan
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Qian Liu
  orcid: null
  s2_author_id: '1409707585'
  s2_url: null
- name: Rui Li
  orcid: null
  s2_author_id: '1500522974'
  s2_url: null
- name: Xing Xie
  orcid: null
  s2_author_id: '2110972816'
  s2_url: null
- name: Jian Tang
  orcid: null
  s2_author_id: '152226504'
  s2_url: null
published_date: Oct 2022
published_date_iso: 2022-10
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: This paper studies learning on text-attributed graphs (TAGs), where each
  node is associated with a text description. An ideal solution for such a problem
  would be integrating both the text and graph structure information with large language
  models and graph neural networks (GNNs). However, the problem becomes very challenging
  when graphs are large due to the high computational complexity brought by training
  large language models and GNNs together. In this paper, we propose an efficient
  and effective solution to learning on large text-attributed graphs by fusing graph
  structure and language learning with a variational Expectation-Maximization (EM)
  framework, called GLEM. Instead of simultaneously training large language models
  and GNNs on big graphs, GLEM proposes to alternatively update the two modules in
  the E-step and M-step. Such a procedure allows training the two modules separately
  while simultaneously allowing the two modules to interact and mutually enhance each
  other. Extensive experiments on multiple data sets demonstrate the efficiency and
  effectiveness of the proposed approach..
codebase_url: https://github.com/AndyJZhao/GLEM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GLEM-GNN
- GLEM-LM
mrr: 0.1979
adjusted_mrr: 0.1319
mrr_dataset_count: 2
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
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.13268'
    title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
    date: Mar 19, 2024
    date_display: Mar 2024
    date_iso: '2024-03-19'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/gdmnl/Unifews
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.791
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GLEM-GNN
    model_key: glem-gnn
    model_plain: GLEM-GNN
    value: 0.7036
    std: 0.0002
    paper_value: 0.7036
    paper_std: 0.0002
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: OGB official split (78/8/14)
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7036
    true_std: 0.0002
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7036
    sort_std: 0.0002
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
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.7036
    std: 0.0002
    paper_value: 0.7036
    paper_std: 0.0002
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
    protocol_note: OGB official split (78/8/14)
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.6771
    at_pub_std: 0.002
    at_pub_source_arxiv: '2108.10097'
    at_pub_source_title: Graph Attention MLP with Reliable Label Utilization
    at_pub_source_date_iso: '2021-08-23'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.026499999999999968
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7036
    true_std: 0.0002
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7036
    sort_std: 0.0002
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Attention MLP with Reliable Label Utilization
    comparison_source_arxiv: '2108.10097'
    is_best: false
    is_std_outlier: false
  - model: GLEM-LM
    model_key: glem-lm
    model_plain: GLEM-LM
    value: 0.6671
    std: 0.0025
    paper_value: 0.6671
    paper_std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: OGB official split (78/8/14)
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6671
    true_std: 0.0025
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6671
    sort_std: 0.0025
    global_rank: 34
    paper_rank: 34
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
    value: 0.8233
    std: 0.0037
    paper_value: 0.8233
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
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8933
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06999999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8933
    sort_std: null
    global_rank: 4
    paper_rank: 90
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8868
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
    global_rank: 6
    sort_value: 0.8868
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLEM-GNN
    model_key: glem-gnn
    model_plain: GLEM-GNN
    value: 0.8736
    std: 0.0007
    paper_value: 0.8736
    paper_std: 0.0007
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
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
  - model: SAGN
    model_key: sagn
    model_plain: SAGN
    value: 0.8736
    std: 0.0007
    paper_value: 0.8736
    paper_std: 0.0007
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
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.812
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.06159999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    comparison_source_arxiv: '2104.09376'
    is_best: false
    is_std_outlier: false
  - model: GLEM-LM
    model_key: glem-lm
    model_plain: GLEM-LM
    value: 0.8483
    std: 0.0004
    paper_value: 0.8483
    paper_std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8483
    true_std: 0.0004
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8483
    sort_std: 0.0004
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.8354
    std: 0.0009
    paper_value: 0.8354
    paper_std: 0.0009
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
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.8354
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2108.10097'
    at_pub_source_title: Graph Attention MLP with Reliable Label Utilization
    at_pub_source_date_iso: '2021-08-23'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8376
    true_std: 0.0019
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.8376
    sort_std: 0.0019
    global_rank: 65
    paper_rank: 71
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LM-Ft
    model_key: lm-ft
    model_plain: LM-Ft
    value: 0.7963
    std: 0.0012
    paper_value: 0.7963
    paper_std: 0.0012
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard test split for ogbn-products
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7963
    true_std: 0.0012
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7963
    sort_std: 0.0012
    global_rank: 157
    paper_rank: 157
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
main_figure: /figures/2210.14709/main_figure.jpegoptim.jpg
---

