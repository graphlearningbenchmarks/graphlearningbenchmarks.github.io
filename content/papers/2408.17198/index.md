---
title: Towards Symbolic XAI -- Explanation Through Human Understandable Logical Relationships
  Between Features
arxiv_id: '2408.17198'
source_url: ''
authors:
- name: T. Schnake
  orcid: null
  s2_author_id: '90387439'
  s2_url: null
- name: F. Jafari
  orcid: null
  s2_author_id: '67218340'
  s2_url: null
- name: Jonas Lederer
  orcid: null
  s2_author_id: '95930534'
  s2_url: null
- name: Pin Xiong
  orcid: null
  s2_author_id: '2062775158'
  s2_url: null
- name: Shinichi Nakajima
  orcid: null
  s2_author_id: '2251769478'
  s2_url: null
- name: Stefan Gugler
  orcid: null
  s2_author_id: '2296992109'
  s2_url: null
- name: G. Montavon
  orcid: null
  s2_author_id: '144535526'
  s2_url: null
- name: Klaus-Robert Müller
  orcid: null
  s2_author_id: '2287775247'
  s2_url: null
published_date: Aug 30, 2024
published_date_iso: '2024-08-30'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Explainable Artificial Intelligence (XAI) plays a crucial role in fostering
  transparency and trust in AI systems, where traditional XAI approaches typically
  offer one level of abstraction for explanations, often in the form of heatmaps highlighting
  single or multiple input features. However, we ask whether abstract reasoning or
  problem-solving strategies of a model may also be relevant, as these align more
  closely with how humans approach solutions to problems. We propose a framework,
  called Symbolic XAI, that attributes relevance to symbolic queries expressing logical
  relationships between input features, thereby capturing the abstract reasoning behind
  a model’s predictions. The methodology is built upon a simple yet general multi-order
  decomposition of model predictions. This decomposition can be specified using higher-order
  propagation-based relevance methods, such as GNN-LRP, or perturbation-based explanation
  methods commonly used in XAI. The effectiveness of our framework is demonstrated
  in the domains of natural language processing (NLP), vision, and quantum chemistry
  (QC), where abstract symbolic domain knowledge is abundant and of significant interest
  to users. The Symbolic XAI framework provides an understanding of the model’s decision-making
  process that is both flexible for customization by the user and human-readable through
  logical formulas.
codebase_url: https://huggingface.co/dima806/facial_emotions_image_detection
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  dataset: IMDB
  rows:
  - model: BERT-Base, Uncased
    model_key: bert-base, uncased
    model_plain: BERT-Base, Uncased
    value: 0.919
    std: null
    paper_value: 0.919
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: 'Section: On the sentiment analysis task'
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Classification accuracy reported for the IMDB dataset in the NLP
      experiments section.
    date: Aug 30, 2024
    date_display: Aug 2024
    date_iso: '2024-08-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.919
    true_std: null
    value_gap_source_arxiv: '2408.17198'
    value_gap_source_title: Towards Symbolic XAI -- Explanation Through Human Understandable
      Logical Relationships Between Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.919
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HG-SCM
    model_key: shgn
    model_plain: HG-SCM
    value: 0.6736
    std: 0.0057
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    venue: KDD 2026 research track. Code available at https://github.com/EdisonLeeeee/lrGAE
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6736
    sort_std: 0.0057
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HG-SCM
    model_key: simplehgn
    model_plain: HG-SCM
    value: 0.6736
    std: 0.0057
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6736
    sort_std: 0.0057
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
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
    - dataset: IMDB
      dataset_slug: imdb
---

