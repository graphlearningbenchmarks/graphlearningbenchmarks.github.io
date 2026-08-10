---
title: Accelerating Scalable Graph Neural Network Inference with Node-Adaptive Propagation
arxiv_id: '2310.10998'
source_url: ''
authors:
- name: Xin Gao
  orcid: null
  s2_author_id: '2192083394'
  s2_url: null
- name: Wentao Zhang
  orcid: null
  s2_author_id: '2108232566'
  s2_url: null
- name: Junliang Yu
  orcid: null
  s2_author_id: '28584977'
  s2_url: null
- name: Yingxiao Shao
  orcid: null
  s2_author_id: '2238939752'
  s2_url: null
- name: Q. Nguyen
  orcid: null
  s2_author_id: '144133815'
  s2_url: null
- name: Bin Cui
  orcid: null
  s2_author_id: '2257282067'
  s2_url: null
- name: Hongzhi Yin
  orcid: null
  s2_author_id: '2260297841'
  s2_url: null
published_date: Oct 17, 2023
published_date_iso: '2023-10-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) have exhibited exceptional efficacy in a diverse
  array of applications. However, the sheer size of large-scale graphs presents a
  significant challenge to real-time inference with GNNs. Although existing Scalable
  GNNs leverage linear propagation to preprocess the features and accelerate the training
  and inference procedure, these methods still suffer from scalability issues when
  making inferences on unseen nodes, as the feature preprocessing requires the graph
  to be known and fixed. To further accelerate Scalable GNNs inference in this inductive
  setting, we propose an online propagation framework and two novel node-adaptive
  propagation methods that can customize the optimal propagation depth for each node
  based on its topological information and thereby avoid redundant feature propagation.
  The trade-off between accuracy and latency can be flexibly managed through simple
  hyper-parameters to accommodate various latency constraints. Moreover, to compensate
  for the inference accuracy loss caused by the potential early termination of propagation,
  we further propose Inception Distillation to exploit the multi-scale receptive field
  information within graphs. The rigorous and comprehensive experimental study on
  public datasets with varying scales and characteristics demonstrates that the proposed
  inference acceleration framework outperforms existing state-of-the-art graph inference
  acceleration methods in terms of accuracy and efficiency. Particularly, the superiority
  of our approach is notable on datasets with larger scales, yielding a $75 $ inference
  speedup on the largest Ogbn-products dataset.
codebase_url: ''
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
  evaluated: 1
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7424
    std: null
    paper_value: 0.7424
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.822
    at_pub_std: 0.009
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.0796
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
    value_gap: 0.0796
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.009
    global_rank: 93
    paper_rank: 299
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.6312
    std: null
    paper_value: 0.6312
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7765
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2304.10668'
    at_pub_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation on
      Textual Graphs'
    at_pub_source_date_iso: '2023-04-20'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.14529999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7765
    true_std: 0.0048
    value_gap_source_arxiv: '2304.10668'
    value_gap_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation
      on Textual Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.14529999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.7765
    sort_std: 0.0048
    global_rank: 229
    paper_rank: 374
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation
      on Textual Graphs'
    comparison_source_arxiv: '2304.10668'
    is_best: false
    is_std_outlier: false
  - model: NAI_g
    model_key: nai_g
    model_plain: NAI_g
    value: 0.7389
    std: null
    paper_value: 0.7389
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7389
    true_std: null
    value_gap_source_arxiv: '2310.10998'
    value_gap_source_title: Accelerating Scalable Graph Neural Network Inference with
      Node-Adaptive Propagation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7389
    sort_std: null
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAI_d
    model_key: nai_d
    model_plain: NAI_d
    value: 0.737
    std: null
    paper_value: 0.737
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.737
    true_std: null
    value_gap_source_arxiv: '2310.10998'
    value_gap_source_title: Accelerating Scalable Graph Neural Network Inference with
      Node-Adaptive Propagation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: null
    global_rank: 315
    paper_rank: 315
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Quantization
    model_key: quantization
    model_plain: Quantization
    value: 0.7301
    std: null
    paper_value: 0.7301
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7301
    at_pub_std: null
    at_pub_source_arxiv: '2211.00495'
    at_pub_source_title: Efficient Graph Neural Network Inference at Large Scale
    at_pub_source_date_iso: '2022-11-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7301
    true_std: null
    value_gap_source_arxiv: '2310.10998'
    value_gap_source_title: Accelerating Scalable Graph Neural Network Inference with
      Node-Adaptive Propagation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7301
    sort_std: null
    global_rank: 320
    paper_rank: 320
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NOSMOG
    model_key: nosmog
    model_plain: NOSMOG
    value: 0.7248
    std: null
    paper_value: 0.7248
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7248
    true_std: null
    value_gap_source_arxiv: '2310.10998'
    value_gap_source_title: Accelerating Scalable Graph Neural Network Inference with
      Node-Adaptive Propagation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7248
    sort_std: null
    global_rank: 323
    paper_rank: 323
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TinyGNN
    model_key: tinygnn
    model_plain: TinyGNN
    value: 0.7133
    std: null
    paper_value: 0.7133
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification split for OGBN-Products
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7133
    at_pub_std: null
    at_pub_source_arxiv: '2211.00495'
    at_pub_source_title: Efficient Graph Neural Network Inference at Large Scale
    at_pub_source_date_iso: '2022-11-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7133
    true_std: null
    value_gap_source_arxiv: '2310.10998'
    value_gap_source_title: Accelerating Scalable Graph Neural Network Inference with
      Node-Adaptive Propagation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: null
    global_rank: 337
    paper_rank: 337
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
main_figure: /figures/2310.10998/main_figure.jpegoptim.jpg
---

