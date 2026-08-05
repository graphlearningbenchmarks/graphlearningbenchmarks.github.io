---
title: 'GraphCLIP: Enhancing Transferability in Graph Foundation Models for Text-Attributed
  Graphs'
arxiv_id: '2410.10329'
source_url: ''
authors:
- name: Yun Zhu
  orcid: null
  s2_author_id: '2257195454'
  s2_url: null
- name: Haizhou Shi
  orcid: null
  s2_author_id: '2313685962'
  s2_url: null
- name: Xiaotang Wang
  orcid: null
  s2_author_id: '2313745417'
  s2_url: null
- name: Yongchao Liu
  orcid: null
  s2_author_id: '2313693489'
  s2_url: null
- name: Yaoke Wang
  orcid: null
  s2_author_id: '2257134292'
  s2_url: null
- name: Boci Peng
  orcid: null
  s2_author_id: '2314827534'
  s2_url: null
- name: Chuntao Hong
  orcid: null
  s2_author_id: '2313754922'
  s2_url: null
- name: Siliang Tang
  orcid: null
  s2_author_id: '2257997261'
  s2_url: null
published_date: Oct 14, 2024
published_date_iso: '2024-10-14'
published_venue: WWW 2024
published_conference: WWW 2024
published_conference_short: WWW
published_conference_slug: www
abstract: 'Recently, research on Text-Attributed Graphs (TAGs) has gained significant
  attention due to the prevalence of free-text node features in real-world applications
  and the advancements in Large Language Models (LLMs) that bolster TAG methodologies.
  However, current TAG approaches face two primary challenges: (i) Heavy reliance
  on label information and (ii) Limited cross-domain zero/few-shot transferability.
  These issues constrain the scaling of both data and model size, owing to high labor
  costs and scaling laws, complicating the development of graph foundation models
  with strong transferability. In this work, we propose the GraphCLIP framework to
  address these challenges by learning foundation models with strong ross-domain zero/few-shot
  transferabi ty through a self-supervised contrastive graph-summary retraining method.
  Specifically, we generate and curate large-scale graph-summary pair data with the
  assistance of LLMs, and introduce a novel graph-summary pretraining method, combined
  with invariant learning, to enhance graph foundation models with strong cross-domain
  zero-shot transferability. For few-shot learning, we propose a novel graph prompt
  tuning technique aligned with our pretraining objective to mitigate catastrophic
  forgetting and minimize learning costs. Extensive experiments show the superiority
  of GraphCLIP in both zero-shot and few-shot settings, while evaluations across various
  downstream tasks confirm the versatility of GraphCLIP. Our code is available at:
  https://github.com/ZhuYun97/GraphCLIP.'
codebase_url: https://github.com/ZhuYun97/GraphCLIP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphCLIP
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: WikiCS
  rows:
  - model: GPM
    model_key: gcn
    model_plain: GPM
    value: 0.9302
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9302
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rse + rgcn (70b)
    model_plain: GPM
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPM
    model_key: rse + sehgnn (70b)
    model_plain: GPM
    value: 0.8796
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 3
    sort_value: 0.8796
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.0265
    std: 0.0072
    paper_value: 0.0265
    paper_std: 0.0072
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7000.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: llaga
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.7388
    at_pub_std: null
    at_pub_source_arxiv: '2407.07457'
    at_pub_source_title: 'GLBench: A Comprehensive Benchmark for Graph with Large
      Language Models'
    at_pub_source_date_iso: '2024-07-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-03-05'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.7123
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8074
    true_std: null
    value_gap_source_arxiv: '2503.03313'
    value_gap_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.7809
    has_value_note: false
    value_note: ''
    sort_value: 0.8074
    sort_std: null
    global_rank: 44
    paper_rank: 280
    rank_delta: 236
    rank_delta_abs: 236
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GLBench: A Comprehensive Benchmark for Graph with Large
      Language Models'
    comparison_source_arxiv: '2407.07457'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.1835
    std: 0.0022
    paper_value: 0.1835
    paper_std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 128.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bgrl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.8
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.6165
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: 0.001
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.6165
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.001
    global_rank: 61
    paper_rank: 280
    rank_delta: 219
    rank_delta_abs: 219
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: BERT
    model_key: bert
    model_plain: BERT
    value: 0.2937
    std: 0.0
    paper_value: 0.2937
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bert
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.7833
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.4896
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7833
    true_std: 0.0043
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.4896
    has_value_note: false
    value_note: ''
    sort_value: 0.7833
    sort_std: 0.0043
    global_rank: 117
    paper_rank: 279
    rank_delta: 162
    rank_delta_abs: 162
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.1886
    std: 0.0025
    paper_value: 0.1886
    paper_std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 128.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dgi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.7825
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.5939
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7825
    true_std: 0.0056
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.5939
    has_value_note: false
    value_note: ''
    sort_value: 0.7825
    sort_std: 0.0056
    global_rank: 120
    paper_rank: 280
    rank_delta: 160
    rank_delta_abs: 160
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    comparison_source_arxiv: '2408.05087'
    is_best: false
    is_std_outlier: false
  - model: DeBERTa
    model_key: deberta
    model_plain: DeBERTa
    value: 0.1529
    std: 0.0
    paper_value: 0.1529
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 184.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: he2020deberta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.7511
    at_pub_std: 0.0197
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.5982
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7511
    true_std: 0.0197
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.5982
    has_value_note: false
    value_note: ''
    sort_value: 0.7511
    sort_std: 0.0197
    global_rank: 179
    paper_rank: 280
    rank_delta: 101
    rank_delta_abs: 101
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: true
  - model: Base
    model_key: base
    model_plain: Base
    value: 0.7019
    std: null
    paper_value: 0.7019
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Scale analysis on target data
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7019
    true_std: null
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7019
    sort_std: null
    global_rank: 212
    paper_rank: 212
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Large
    model_key: large
    model_plain: Large
    value: 0.7014
    std: null
    paper_value: 0.7014
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Scale analysis on target data
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7014
    true_std: null
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7014
    sort_std: null
    global_rank: 213
    paper_rank: 213
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Medium
    model_key: medium
    model_plain: Medium
    value: 0.6942
    std: null
    paper_value: 0.6942
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Scale analysis on target data
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6942
    true_std: null
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6942
    sort_std: null
    global_rank: 218
    paper_rank: 218
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Small
    model_key: small
    model_plain: Small
    value: 0.6785
    std: null
    paper_value: 0.6785
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Scale analysis on target data
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6785
    true_std: null
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6785
    sort_std: null
    global_rank: 228
    paper_rank: 228
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaMA3.1
    model_key: llama3.1
    model_plain: LLaMA3.1
    value: 0.6282
    std: 0.0004
    paper_value: 0.6282
    paper_std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 8000.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: vavekanand2024llama
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6282
    true_std: 0.0004
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6282
    sort_std: 0.0004
    global_rank: 258
    paper_rank: 258
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Qwen2
    model_key: qwen2
    model_plain: Qwen2
    value: 0.6091
    std: 0.0008
    paper_value: 0.6091
    paper_std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7000.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: qwen2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6091
    true_std: 0.0008
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6091
    sort_std: 0.0008
    global_rank: 264
    paper_rank: 264
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPT
    model_key: graphgpt
    model_plain: GraphGPT
    value: 0.063
    std: 0.0026
    paper_value: 0.063
    paper_std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 7000.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: graphgpt
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3359
    true_std: null
    value_gap_source_arxiv: '2505.17599'
    value_gap_source_title: Dynamic Bundling with Large Language Models for Zero-Shot
      Inference on Text-Attributed Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.2729
    has_value_note: false
    value_note: ''
    sort_value: 0.3359
    sort_std: null
    global_rank: 278
    paper_rank: 280
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G2P2
    model_key: g2p2
    model_plain: G2P2
    value: 0.3192
    std: 0.0015
    paper_value: 0.3192
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 63.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: g2p2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Zero-shot inference on public WikiCS split
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3192
    true_std: 0.0015
    value_gap_source_arxiv: '2410.10329'
    value_gap_source_title: 'GraphCLIP: Enhancing Transferability in Graph Foundation
      Models for Text-Attributed Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3192
    sort_std: 0.0015
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: WikiCS
      dataset_slug: wikics
single_proposed_model: GraphCLIP
main_figure: /figures/2410.10329/main_figure.jpegoptim.jpg
---

