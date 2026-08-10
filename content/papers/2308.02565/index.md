---
title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph Learning'
arxiv_id: '2308.02565'
source_url: ''
authors:
- name: Keyu Duan
  orcid: null
  s2_author_id: '108237152'
  s2_url: null
- name: Qian Liu
  orcid: null
  s2_author_id: '1409707585'
  s2_url: null
- name: Tat-seng Chua
  orcid: null
  s2_author_id: '143779329'
  s2_url: null
- name: Shuicheng Yan
  orcid: null
  s2_author_id: '2186749683'
  s2_url: null
- name: Wei Tsang Ooi
  orcid: null
  s2_author_id: '1678873'
  s2_url: null
- name: Qizhe Xie
  orcid: null
  s2_author_id: '1912046'
  s2_url: null
- name: Junxian He
  orcid: null
  s2_author_id: '2109932032'
  s2_url: null
published_date: Aug 3, 2023
published_date_iso: '2023-08-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Textual graphs (TGs) are graphs whose nodes correspond to text (sentences
  or documents), which are widely prevalent. The representation learning of TGs involves
  two stages: \((i)\) unsupervised feature extraction and \((ii)\) supervised graph
  representation learning. In recent years, extensive efforts have been devoted to
  the latter stage, where Graph Neural Networks (GNNs) have dominated. However, the
  former stage for most existing graph benchmarks still relies on traditional feature
  engineering techniques. More recently, with the rapid development of language models
  (LMs), researchers have focused on leveraging LMs to facilitate the learning of
  TGs, either by jointly training them in a computationally intensive framework (merging
  the two stages), or designing complex self-supervised training tasks for feature
  extraction (enhancing the first stage). In this work, we present SimTeG, a frustratingly
  ple approach for xtual raph learning that does not innovate in frameworks, models,
  and tasks. Instead, we first perform supervised parameter-efficient fine-tuning
  (PEFT) on a pre-trained LM on the downstream task, such as node classification.
  We then generate node embeddings using the last hidden states of finetuned LM. These
  derived features can be further utilized by any GNN for training on the same task.
  We evaluate our approach on two fundamental graph representation learning tasks:
  node classification and link prediction. Through extensive experiments, we show
  that our approach significantly improves the performance of various GNNs on multiple
  graph benchmarks. Remarkably, when additional supporting text provided by large
  language models (LLMs) is included, a simple two-layer GraphSAGE trained on an ensemble
  of SimTeG \ achieves an accuracy of 77.48\ comparable to state-of-the-art (SOTA)
  performance obtained from far more complicated GNN architectures. Furthermore, when
  combined with a SOTA GNN, we achieve a new SOTA of \(78.04 \ Our code is publicly
  available at \ and the generated node features for all graph benchmarks can be accessed
  at.'
codebase_url: https://github.com/vermouthdky/SimTeG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SimTEG
mrr: 0.0256
adjusted_mrr: 0.0085
mrr_dataset_count: 1
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
  - model: GLEM
    model_key: glem
    model_plain: GLEM
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
    source_ref: zhao2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Official OGB split for node classification
    date: Aug 3, 2023
    date_display: Aug 2023
    date_iso: '2023-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8125
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2304.10668'
    at_pub_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation on
      Textual Graphs'
    at_pub_source_date_iso: '2023-04-20'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.06110000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Train Your Own GNN Teacher: Graph-Aware Distillation
      on Textual Graphs'
    comparison_source_arxiv: '2304.10668'
    is_best: false
    is_std_outlier: false
  - model: X-GIANT
    model_key: x-giant
    model_plain: X-GIANT
    value: 0.8612
    std: 0.0034
    paper_value: 0.8612
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
    protocol_note: Official OGB split for node classification
    date: Aug 3, 2023
    date_display: Aug 2023
    date_iso: '2023-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8612
    true_std: 0.0034
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8612
    sort_std: 0.0034
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
  - model: SimTEG
    model_key: simteg
    model_plain: SimTEG
    value: 0.854
    std: 0.0028
    paper_value: 0.854
    paper_std: 0.0028
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
    protocol_note: Official OGB split for node classification
    date: Aug 3, 2023
    date_display: Aug 2023
    date_iso: '2023-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.0028
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.0028
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
  - model: X-OGB
    model_key: x-ogb
    model_plain: X-OGB
    value: 0.8182
    std: 0.0044
    paper_value: 0.8182
    paper_std: 0.0044
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
    protocol_note: Official OGB split for node classification
    date: Aug 3, 2023
    date_display: Aug 2023
    date_iso: '2023-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8182
    true_std: 0.0044
    value_gap_source_arxiv: '2308.02565'
    value_gap_source_title: 'SimTeG: A Frustratingly ple Approach Improves xtual raph
      Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8182
    sort_std: 0.0044
    global_rank: 103
    paper_rank: 103
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
single_proposed_model: SimTEG
main_figure: /figures/2308.02565/main_figure.jpegoptim.jpg
---

