---
title: What Improves the Generalization of Graph Transformers? A Theoretical Dive
  into the Self-attention and Positional Encoding
arxiv_id: '2406.01977'
source_url: ''
authors:
- name: Hongkang Li
  orcid: null
  s2_author_id: '2162633775'
  s2_url: null
- name: Meng Wang
  orcid: null
  s2_author_id: '2261906420'
  s2_url: null
- name: Tengfei Ma
  orcid: null
  s2_author_id: '2329165433'
  s2_url: null
- name: Sijia Liu
  orcid: null
  s2_author_id: '2261649341'
  s2_url: null
- name: Zaixi Zhang
  orcid: null
  s2_author_id: '2350500728'
  s2_url: null
- name: Pin-Yu Chen
  orcid: null
  s2_author_id: '2257357506'
  s2_url: null
published_date: Jun 4, 2024
published_date_iso: '2024-06-04'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: Graph Transformers, which incorporate self-attention and positional encoding,
  have recently emerged as a powerful architecture for various graph learning tasks.
  Despite their impressive performance, the complex non-convex interactions across
  layers and the recursive graph structure have made it challenging to establish a
  theoretical foundation for learning and generalization. This study introduces the
  first theoretical investigation of a shallow Graph Transformer for semi-supervised
  node classification, comprising a self-attention layer with relative positional
  encoding and a two-layer perceptron. Focusing on a graph data model with discriminative
  nodes that determine node labels and non-discriminative nodes that are class-irrelevant,
  we characterize the sample complexity required to achieve a desirable generalization
  error by training with stochastic gradient descent (SGD). This paper provides the
  quantitative characterization of the sample complexity and number of iterations
  for convergence dependent on the fraction of discriminative nodes, the dominant
  patterns, and the initial model errors. Furthermore, we demonstrate that self-attention
  and positional encoding enhance generalization by making the attention map sparse
  and promoting the core neighborhood during training, which explains the superior
  feature representation of Graph Transformers. Our theoretical results are supported
  by empirical experiments on synthetic and real-world benchmarks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GT
mrr: 0.0101
adjusted_mrr: 0.0034
mrr_dataset_count: 1
benchmark_categories:
- Heterophilic Graphs
- LRGB
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Actor
  rows:
  - model: R-SoftGraphAIN
    model_key: nodeformer
    model_plain: R-SoftGraphAIN
    value: 0.7623
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7623
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: diggr
    model_plain: R-SoftGraphAIN
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.432
    std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 3
    sort_value: 0.432
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ZLHL
    model_key: zlhl
    model_plain: ZLHL
    value: 0.401
    std: null
    paper_value: 0.401
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
    table_ref: ''
    source_ref: ZLHL22
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 4, 2024
    date_display: Jun 2024
    date_iso: '2024-06-04'
    published_venue: ICML 2024
    published_conference: ICML 2024
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
    sort_value: 0.401
    sort_std: null
    global_rank: 51
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
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.401
    std: null
    paper_value: 0.401
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
    table_ref: ''
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 4, 2024
    date_display: Jun 2024
    date_iso: '2024-06-04'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.3794
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.021600000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3794
    true_std: 0.0026
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.021600000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.3794
    sort_std: 0.0026
    global_rank: 99
    paper_rank: 51
    rank_delta: -48
    rank_delta_abs: 48
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
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
- &id002
  dataset: PascalVOC-SP
  rows:
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.9854
    std: null
    paper_value: 0.9854
    paper_std: null
    metric: fraction of nodes satisfying $\Delta_n(z_m)>0$
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to pascalvoc-sp (score=89)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 4, 2024
    date_display: Jun 2024
    date_iso: '2024-06-04'
    published_venue: ICML 2024
    published_conference: ICML 2024
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
    sort_value: 0.9854
    sort_std: null
    global_rank: 1
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
    is_best: true
    is_std_outlier: false
  rank_metric: fraction of nodes satisfying $\Delta_n(z_m)>0$
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - fraction of nodes satisfying $\Delta_n(z_m)>0$
  metric: fraction of nodes satisfying $\Delta_n(z_m)>0$
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: LRGB
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PascalVOC-SP
      dataset_slug: pascalvoc-sp
single_proposed_model: GT
main_figure: /figures/2406.01977/main_figure.jpegoptim.jpg
---

