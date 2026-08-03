---
title: 'Beyond Weisfeiler-Lehman: A Quantitative Framework for GNN Expressiveness'
arxiv_id: '2401.08514'
source_url: ''
authors:
- name: Bohang Zhang
  orcid: null
  s2_author_id: '1988294358'
  s2_url: null
- name: Jingchu Gai
  orcid: null
  s2_author_id: '2279749992'
  s2_url: null
- name: Yiheng Du
  orcid: null
  s2_author_id: '2279758346'
  s2_url: null
- name: Qiwei Ye
  orcid: null
  s2_author_id: '2279751598'
  s2_url: null
- name: Di He
  orcid: null
  s2_author_id: '2266469594'
  s2_url: null
- name: Liwei Wang
  orcid: null
  s2_author_id: '2257314569'
  s2_url: null
published_date: Jan 16, 2024
published_date_iso: '2024-01-16'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: '=-1 Designing expressive Graph Neural Networks (GNNs) is a fundamental
  topic in the graph learning community. So far, GNN expressiveness has been primarily
  assessed via the Weisfeiler-Lehman (WL) hierarchy. However, such an expressivity
  measure has notable limitations: it is inherently coarse, qualitative, and may not
  well reflect practical requirements (e.g., the ability to encode substructures).
  In this paper, we introduce a unified framework for quantitatively studying the
  expressiveness of GNN architectures, addressing all the above limitations. Specifically,
  we identify a fundamental expressivity measure termed homomorphism expressivity,
  which quantifies the ability of GNN models to count graphs under homomorphism. Homomorphism
  expressivity offers a complete and practical assessment tool: the completeness enables
  direct expressivity comparisons between GNN models, while the practicality allows
  for understanding concrete GNN abilities such as subgraph counting. By examining
  four classes of prominent GNNs as case studies, we derive simple, unified, and elegant
  descriptions of their homomorphism expressivity for both invariant and equivariant
  settings. Our results provide novel insights into a series of previous work, unify
  the landscape of different subareas in the community, and settle several open questions.
  Empirically, extensive experiments on both synthetic and real-world tasks verify
  our theory, showing that the practical performance of GNN models aligns well with
  the proposed metric.'
codebase_url: https://github.com/subgraph23/homomorphism-expressivity
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ZINC
  rows:
  - model: Subgraphormer
    model_key: ppgn++
    model_plain: Subgraphormer
    value: 0.02
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_display: Feb 2023
    date_iso: '2023-02-22'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.02
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Subgraphormer
    model_key: subgraphormer
    model_plain: Subgraphormer
    value: 0.02
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.02
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Subgraphormer
    model_key: cin
    model_plain: Subgraphormer
    value: 0.021
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.03561'
    title: 'CIN++: Enhancing Topological Message Passing'
    date: Jun 6, 2023
    date_display: Jun 2023
    date_iso: '2023-06-06'
    venue: arXiv.org
    codebase_url: https://github.com/twitter-research/cwn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Without any use of feature augmentation such as positional
      encoding, our model exhibits particularly strong performance
    is_global_top: true
    global_rank: 3
    sort_value: 0.021
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: N2-GNN
    model_key: n2-gnn
    model_plain: N2-GNN
    value: 0.059
    std: 0.002
    paper_value: 0.059
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    source_ref: feng2023towards
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2024
    date_display: Jan 2024
    date_iso: '2024-01-16'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
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
    sort_value: 0.059
    sort_std: 0.002
    global_rank: 23
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
---

