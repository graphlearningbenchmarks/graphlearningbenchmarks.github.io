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
mrr: 0.0175
adjusted_mrr: 0.0058
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
  - model: DiGGR
    model_key: diggr
    model_plain: DiGGR
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TRIGON
    model_key: trigon
    model_plain: TRIGON
    value: 0.4402
    std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.19071'
    title: Dynamic Triangulation-Based Graph Rewiring for Graph Neural Networks
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Hugo-Attali/TRIGON-CIKM-2025
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
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
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4026
    std: 0.0108
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 54
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
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
    value_gap_source_date_iso: '2024-06-04'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.021600000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.401
    true_std: null
    value_gap_source_arxiv: '2406.01977'
    value_gap_source_title: What Improves the Generalization of Graph Transformers?
      A Theoretical Dive into the Self-attention and Positional Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.401
    sort_std: null
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
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
    value_gap_source_date_iso: '2024-06-04'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.401
    true_std: null
    value_gap_source_arxiv: '2406.01977'
    value_gap_source_title: What Improves the Generalization of Graph Transformers?
      A Theoretical Dive into the Self-attention and Positional Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.401
    sort_std: null
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3899
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 86
    sort_value: 0.3899
    sort_std: 0.0085
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
    value_gap_source_date_iso: '2024-06-04'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9854
    true_std: null
    value_gap_source_arxiv: '2406.01977'
    value_gap_source_title: What Improves the Generalization of Graph Transformers?
      A Theoretical Dive into the Self-attention and Positional Encoding
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9854
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

