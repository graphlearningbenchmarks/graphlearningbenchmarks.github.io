---
title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous Graphs
  via Domain-Specific Expert Encoding
arxiv_id: '2602.13075'
source_url: ''
authors:
- name: Chundong Liang
  orcid: null
  s2_author_id: '2106780589'
  s2_url: null
- name: Yongqi Huang
  orcid: null
  s2_author_id: '2293653375'
  s2_url: null
- name: Dongxiao He
  orcid: null
  s2_author_id: '2293422204'
  s2_url: null
- name: Peiyuan Li
  orcid: null
  s2_author_id: '48982166'
  s2_url: null
- name: Yawen Li
  orcid: null
  s2_author_id: '2222317038'
  s2_url: null
- name: Di Jin
  orcid: null
  s2_author_id: '2288101014'
  s2_url: null
- name: Weixiong Zhang
  orcid: null
  s2_author_id: '2288159687'
  s2_url: null
published_date: Feb 13, 2026
published_date_iso: '2026-02-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph pre-training has achieved remarkable success in recent years, delivering
  transferable representations for downstream adaptation. However, most existing methods
  are designed for either homogeneous or heterogeneous graphs, thereby hindering unified
  graph modeling across diverse graph types. This separation contradicts real-world
  applications, where mixed homogeneous and heterogeneous graphs are ubiquitous, and
  distribution shifts between upstream pre-training and downstream deployment are
  common. In this paper, we empirically demonstrate that a balanced mixture of homogeneous
  and heterogeneous graph pre-training benefits downstream tasks and propose a unified
  multi-domain Graph Pre-training method across Homogeneous and Heterogeneous graphs
  ($ GPH^2$). To address the lack of a unified encoder for homogeneous and heterogeneous
  graphs, we propose a Unified Multi-View Graph Construction that simultaneously encodes
  both without explicit graph-type-specific designs. To cope with the increased cross-domain
  distribution discrepancies arising from mixed graphs, we introduce domain-specific
  expert encoding. Each expert is independently pre-trained on a single graph to capture
  domain-specific knowledge, thereby shielding the pre-training encoder from the adverse
  effects of cross-domain discrepancies. For downstream tasks, we further design a
  Task-oriented Expert Fusion Strategy that adaptively integrates multiple experts
  based on their discriminative strengths. Extensive experiments on mixed graphs demonstrate
  that $ ^2$ enables stable transfer across graph types and domains, significantly
  outperforming existing graph pre-training methods.
codebase_url: https://github.com/hedongxiao-tju/GPH-2
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GPH^2
mrr: 0.037
adjusted_mrr: 0.0123
mrr_dataset_count: 1
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
  dataset: Freebase
  rows:
  - model: SlotGAT
    model_key: gc-hgnn
    model_plain: SlotGAT
    value: 0.6247
    std: 0.0042
    metric: Macro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 1
    sort_value: 0.6247
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HGMAE
    model_key: hgmae
    model_plain: HGMAE
    value: 0.3515
    std: 0.0362
    paper_value: 0.3515
    paper_std: 0.0362
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6082
    at_pub_std: 0.0051
    at_pub_source_arxiv: '2404.02810'
    at_pub_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2024-04-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2567
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6082
    true_std: 0.0051
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.2567
    has_value_note: false
    value_note: ''
    sort_value: 0.6082
    sort_std: 0.0051
    global_rank: 2
    paper_rank: 31
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    comparison_source_arxiv: '2404.02810'
    is_best: false
    is_std_outlier: false
  - model: HeCo
    model_key: heco
    model_plain: HeCo
    value: 0.3799
    std: 0.0312
    paper_value: 0.3799
    paper_std: 0.0312
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5987
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2404.02810'
    at_pub_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2024-04-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2188
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5987
    true_std: 0.0033
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.2188
    has_value_note: false
    value_note: ''
    sort_value: 0.5987
    sort_std: 0.0033
    global_rank: 3
    paper_rank: 31
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    comparison_source_arxiv: '2404.02810'
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.3337
    std: 0.0232
    paper_value: 0.3337
    paper_std: 0.0232
    metric: Macro-F1
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5599
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2404.02810'
    at_pub_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2024-04-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.22619999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5599
    true_std: 0.0059
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.22619999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.5599
    sort_std: 0.0059
    global_rank: 11
    paper_rank: 32
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    comparison_source_arxiv: '2404.02810'
    is_best: false
    is_std_outlier: false
  - model: GPH^2
    model_key: gph^2
    model_plain: GPH^2
    value: 0.4478
    std: 0.0547
    paper_value: 0.4478
    paper_std: 0.0547
    metric: Macro-F1
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4478
    true_std: 0.0547
    value_gap_source_arxiv: '2602.13075'
    value_gap_source_title: Unified Multi-Domain Graph Pre-training for Homogeneous
      and Heterogeneous Graphs via Domain-Specific Expert Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4478
    sort_std: 0.0547
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGPrompt
    model_key: hgprompt
    model_plain: HGPrompt
    value: 0.4078
    std: 0.0323
    paper_value: 0.4078
    paper_std: 0.0323
    metric: Macro-F1
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4078
    true_std: 0.0323
    value_gap_source_arxiv: '2602.13075'
    value_gap_source_title: Unified Multi-Domain Graph Pre-training for Homogeneous
      and Heterogeneous Graphs via Domain-Specific Expert Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4078
    sort_std: 0.0323
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HERO
    model_key: hero
    model_plain: HERO
    value: 0.3139
    std: 0.078
    paper_value: 0.3139
    paper_std: 0.078
    metric: Macro-F1
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
    protocol_note: 3-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3139
    true_std: 0.078
    value_gap_source_arxiv: '2602.13075'
    value_gap_source_title: Unified Multi-Domain Graph Pre-training for Homogeneous
      and Heterogeneous Graphs via Domain-Specific Expert Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3139
    sort_std: 0.078
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
  - model: HetGPT
    model_key: hetgpt
    model_plain: HetGPT
    value: 0.2903
    std: 0.0654
    paper_value: 0.2903
    paper_std: 0.0654
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
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
    protocol_note: 5-shot node classification on heterogeneous graphs
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2903
    true_std: 0.0654
    value_gap_source_arxiv: '2602.13075'
    value_gap_source_title: Unified Multi-Domain Graph Pre-training for Homogeneous
      and Heterogeneous Graphs via Domain-Specific Expert Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2903
    sort_std: 0.0654
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Macro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Macro-F1
  paper_metrics:
  - Macro-F1
  metric: Macro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
    - dataset: Freebase
      dataset_slug: freebase
single_proposed_model: GPH^2
main_figure: /figures/2602.13075/main_figure.jpegoptim.jpg
---

