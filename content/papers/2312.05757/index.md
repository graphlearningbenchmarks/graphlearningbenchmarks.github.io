---
title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
  Graph'
arxiv_id: '2312.05757'
source_url: ''
authors:
- name: Tianqianjin Lin
  orcid: null
  s2_author_id: '1516806407'
  s2_url: null
- name: Kaisong Song
  orcid: null
  s2_author_id: '2270983508'
  s2_url: null
- name: Zhuoren Jiang
  orcid: null
  s2_author_id: '1695957219'
  s2_url: null
- name: Yangyang Kang
  orcid: null
  s2_author_id: '38753454'
  s2_url: null
- name: Weikang Yuan
  orcid: null
  s2_author_id: '2261186986'
  s2_url: null
- name: Xurui Li
  orcid: null
  s2_author_id: '2144393712'
  s2_url: null
- name: Changlong Sun
  orcid: null
  s2_author_id: '2060934'
  s2_url: null
- name: Cui Huang
  orcid: null
  s2_author_id: '2203170628'
  s2_url: null
- name: Xiaozhong Liu
  orcid: null
  s2_author_id: '1713802'
  s2_url: null
published_date: Dec 10, 2023
published_date_iso: '2023-12-10'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Heterogeneous graph neural networks have become popular in various domains.
  However, their generalizability and interpretability are limited due to the discrepancy
  between their inherent inference flows and human reasoning logic or underlying causal
  relationships for the learning problem. This study introduces a novel solution,
  HG-SCM (Heterogeneous Graph as Structural Causal Model). It can mimic the human
  perception and decision process through two key steps: constructing intelligible
  variables based on semantics derived from the graph schema and automatically learning
  task-level causal relationships among these variables by incorporating advanced
  causal discovery techniques. We compared HG-SCM to seven state-of-the-art baseline
  models on three real-world datasets, under three distinct and ubiquitous out-of-distribution
  settings. HG-SCM achieved the highest average performance rank with minimal standard
  deviation, substantiating its effectiveness and superiority in terms of both predictive
  power and generalizability. Additionally, the visualization and analysis of the
  auto-learned causal diagrams for the three tasks aligned well with domain knowledge
  and human cognition, demonstrating prominent interpretability. HG-SCM''s human-like
  nature and its enhanced generalizability and interpretability make it a promising
  solution for special scenarios where transparency and trustworthiness are paramount.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HG-SCM
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 3
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: ACM
  rows:
  - model: GCN+P+D
    model_key: signgt
    model_plain: GCN+P+D
    value: 0.9545
    std: 0.0049
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9545
    sort_std: 0.0049
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN+P+D
    model_key: nodeformer
    model_plain: GCN+P+D
    value: 0.9493
    std: 0.0035
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9493
    sort_std: 0.0035
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN+P+D
    model_key: fagcn
    model_plain: GCN+P+D
    value: 0.9487
    std: 0.0059
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9487
    sort_std: 0.0059
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    value: 0.9356
    std: 0.0032
    paper_value: 0.9356
    paper_std: 0.0032
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
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9356
    true_std: 0.0032
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9356
    sort_std: 0.0032
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9351
    std: 0.0045
    paper_value: 0.9351
    paper_std: 0.0045
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
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9351
    true_std: 0.0045
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9351
    sort_std: 0.0045
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
  - model: simpleHGN
    model_key: simplehgn
    model_plain: simpleHGN
    value: 0.9335
    std: 0.0045
    paper_value: 0.9335
    paper_std: 0.0045
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9335
    true_std: 0.0045
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9335
    sort_std: 0.0045
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
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9079
    std: 0.0043
    paper_value: 0.9079
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.922
    at_pub_std: 0.002
    at_pub_source_arxiv: '2011.09679'
    at_pub_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    at_pub_source_date_iso: '2020-11-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.014100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.002
    value_gap_source_arxiv: '2011.09679'
    value_gap_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.014100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.002
    global_rank: 42
    paper_rank: 48
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    comparison_source_arxiv: '2011.09679'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.91
    std: 0.0076
    paper_value: 0.91
    paper_std: 0.0076
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.919
    at_pub_std: 0.003
    at_pub_source_arxiv: '2011.09679'
    at_pub_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    at_pub_source_date_iso: '2020-11-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.919
    true_std: 0.003
    value_gap_source_arxiv: '2011.09679'
    value_gap_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.919
    sort_std: 0.003
    global_rank: 43
    paper_rank: 47
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9141
    std: 0.0075
    paper_value: 0.9141
    paper_std: 0.0075
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9175
    true_std: 0.0035
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.0033999999999999586
    has_value_note: false
    value_note: ''
    sort_value: 0.9175
    sort_std: 0.0035
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.912
    std: 0.0071
    paper_value: 0.912
    paper_std: 0.0071
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.0071
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.0071
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9077
    std: 0.0065
    paper_value: 0.9077
    paper_std: 0.0065
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9077
    true_std: 0.0065
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9077
    sort_std: 0.0065
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.9032
    std: 0.0154
    paper_value: 0.9032
    paper_std: 0.0154
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9032
    true_std: 0.0154
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9032
    sort_std: 0.0154
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.8991
    std: 0.0037
    paper_value: 0.8991
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8991
    true_std: 0.0037
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8991
    sort_std: 0.0037
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.8505
    std: 0.0025
    paper_value: 0.8505
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
    source_ref: simplehgn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: official i.i.d data split
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8505
    true_std: 0.0025
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8505
    sort_std: 0.0025
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: DBLP
  is_multi_metric: true
  rows:
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    metric_values:
    - null
    - 0.9449
    - 0.9489
    metric_stds:
    - null
    - 0.002
    - 0.0018
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9489
    sort_std: 0.0018
    true_value: null
    true_std: null
    paper_value: 0.9489
    paper_std: 0.0018
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: ''
    value_gap_source_title: ''
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    metric_values:
    - null
    - 0.9451
    - 0.949
    metric_stds:
    - null
    - 0.0015
    - 0.0015
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.9451
    sort_std: 0.0015
    true_value: 0.9451
    true_std: 0.0015
    paper_value: 0.9451
    paper_std: 0.0015
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1
  - model: simpleHGN
    model_key: simplehgn
    model_plain: simpleHGN
    metric_values:
    - null
    - 0.9401
    - 0.9446
    metric_stds:
    - null
    - 0.0024
    - 0.0022
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9401
    sort_std: 0.0024
    true_value: 0.9401
    true_std: 0.0024
    paper_value: 0.9401
    paper_std: 0.0024
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: GTN
    model_key: gtn
    model_plain: GTN
    metric_values:
    - null
    - 0.9352
    - 0.9397
    metric_stds:
    - null
    - 0.0055
    - 0.0054
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9352
    sort_std: 0.0055
    true_value: 0.9352
    true_std: 0.0055
    paper_value: 0.9352
    paper_std: 0.0055
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    metric_values:
    - null
    - 0.9334
    - 0.9381
    metric_stds:
    - null
    - 0.0058
    - 0.0055
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9334
    sort_std: 0.0058
    true_value: 0.9334
    true_std: 0.0058
    paper_value: 0.9334
    paper_std: 0.0058
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    metric_values:
    - null
    - 0.9328
    - 0.9376
    metric_stds:
    - null
    - 0.0051
    - 0.0045
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9328
    sort_std: 0.0051
    true_value: 0.9328
    true_std: 0.0051
    paper_value: 0.9328
    paper_std: 0.0051
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: HGT
    model_key: hgt
    model_plain: HGT
    metric_values:
    - null
    - 0.9301
    - 0.9349
    metric_stds:
    - null
    - 0.0023
    - 0.0025
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.9301
    sort_std: 0.0023
    true_value: 0.9301
    true_std: 0.0023
    paper_value: 0.9301
    paper_std: 0.0023
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    metric_values:
    - null
    - 0.9176
    - 0.9233
    metric_stds:
    - null
    - 0.0043
    - 0.0041
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9176
    sort_std: 0.0043
    true_value: 0.9176
    true_std: 0.0043
    paper_value: 0.9176
    paper_std: 0.0043
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: HAN
    model_key: han
    model_plain: HAN
    metric_values:
    - null
    - 0.9167
    - 0.9205
    metric_stds:
    - null
    - 0.0049
    - 0.0062
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9167
    sort_std: 0.0049
    true_value: 0.9167
    true_std: 0.0049
    paper_value: 0.9167
    paper_std: 0.0049
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    metric_values:
    - null
    - 0.9152
    - 0.9207
    metric_stds:
    - null
    - 0.005
    - 0.005
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9152
    sort_std: 0.005
    true_value: 0.9152
    true_std: 0.005
    paper_value: 0.9152
    paper_std: 0.005
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    metric_values:
    - null
    - 0.7855
    - 0.8056
    metric_stds:
    - null
    - 0.0242
    - 0.015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7855
    sort_std: 0.0242
    true_value: 0.7855
    true_std: 0.0242
    paper_value: 0.7855
    paper_std: 0.0242
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  metrics:
  - Micro-F1
  - Macro F1
  - Accuracy
  primary_metric: Micro-F1
  rank_metric: Macro F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Macro F1
  - Accuracy
  metric: Macro F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: IMDB
  is_multi_metric: true
  rows:
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    metric_values:
    - null
    - null
    - 0.6598
    metric_stds:
    - null
    - null
    - 0.0012
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6598
    sort_std: 0.0012
    true_value: 0.6598
    true_std: 0.0012
    paper_value: 0.6598
    paper_std: 0.0012
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    metric_values:
    - null
    - 0.6534
    - 0.669
    metric_stds:
    - null
    - 0.0033
    - 0.0061
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.6534
    sort_std: 0.0033
    true_value: 0.6534
    true_std: 0.0033
    paper_value: 0.6534
    paper_std: 0.0033
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 1
  - model: simpleHGN
    model_key: simplehgn
    model_plain: simpleHGN
    metric_values:
    - null
    - 0.6353
    - 0.6736
    metric_stds:
    - null
    - 0.0136
    - 0.0057
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6353
    sort_std: 0.0136
    true_value: 0.6353
    true_std: 0.0136
    paper_value: 0.6353
    paper_std: 0.0136
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: HGT
    model_key: hgt
    model_plain: HGT
    metric_values:
    - null
    - 0.63
    - 0.672
    metric_stds:
    - null
    - 0.0119
    - 0.0057
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.63
    sort_std: 0.0119
    true_value: 0.63
    true_std: 0.0119
    paper_value: 0.63
    paper_std: 0.0119
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: GTN
    model_key: gtn
    model_plain: GTN
    metric_values:
    - null
    - 0.6047
    - 0.6514
    metric_stds:
    - null
    - 0.0098
    - 0.0045
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6047
    sort_std: 0.0098
    true_value: 0.6047
    true_std: 0.0098
    paper_value: 0.6047
    paper_std: 0.0098
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    metric_values:
    - null
    - 0.5985
    - 0.6422
    metric_stds:
    - null
    - 0.0321
    - 0.0103
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5985
    sort_std: 0.0321
    true_value: 0.5985
    true_std: 0.0321
    paper_value: 0.5985
    paper_std: 0.0321
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    metric_values:
    - null
    - 0.5885
    - 0.6205
    metric_stds:
    - null
    - 0.0026
    - 0.0015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5885
    sort_std: 0.0026
    true_value: 0.5885
    true_std: 0.0026
    paper_value: 0.5885
    paper_std: 0.0026
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: HAN
    model_key: han
    model_plain: HAN
    metric_values:
    - null
    - 0.5774
    - 0.6463
    metric_stds:
    - null
    - 0.0096
    - 0.0058
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5774
    sort_std: 0.0096
    true_value: 0.5774
    true_std: 0.0096
    paper_value: 0.5774
    paper_std: 0.0096
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    metric_values:
    - null
    - 0.5649
    - 0.6467
    metric_stds:
    - null
    - 0.032
    - 0.0167
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5649
    sort_std: 0.032
    true_value: 0.5649
    true_std: 0.032
    paper_value: 0.5649
    paper_std: 0.032
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    metric_values:
    - null
    - 0.4947
    - 0.5768
    metric_stds:
    - null
    - 0.0121
    - 0.0044
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4947
    sort_std: 0.0121
    true_value: 0.4947
    true_std: 0.0121
    paper_value: 0.4947
    paper_std: 0.0121
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    metric_values:
    - null
    - 0.4825
    - 0.5116
    metric_stds:
    - null
    - 0.0067
    - 0.0065
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4825
    sort_std: 0.0067
    true_value: 0.4825
    true_std: 0.0067
    paper_value: 0.4825
    paper_std: 0.0067
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2312.05757'
    value_gap_source_title: 'Towards Human-like Perception: Learning Structural Causal
      Model in Heterogeneous Graph'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  metrics:
  - Micro-F1
  - Macro F1
  - Accuracy
  primary_metric: Micro-F1
  rank_metric: Macro F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Macro F1
  - Accuracy
  metric: Macro F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: IMDB
      dataset_slug: imdb
single_proposed_model: HG-SCM
main_figure: /figures/2312.05757/main_figure.jpegoptim.jpg
---

