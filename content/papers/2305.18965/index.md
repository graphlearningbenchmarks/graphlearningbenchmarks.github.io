---
title: Node Embedding from Neural Hamiltonian Orbits in Graph Neural Networks
arxiv_id: '2305.18965'
source_url: ''
authors:
- name: Qiyu Kang
  orcid: null
  s2_author_id: '22758176'
  s2_url: null
- name: Kai Zhao
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Yang Song
  orcid: null
  s2_author_id: '2006209232'
  s2_url: null
- name: Sijie Wang
  orcid: null
  s2_author_id: '2116422074'
  s2_url: null
- name: Wee Peng Tay
  orcid: null
  s2_author_id: '3118058'
  s2_url: null
published_date: May 30, 2023
published_date_iso: '2023-05-30'
published_venue: ICML 2023
published_conference: ICML 2023
published_conference_short: ICML
published_conference_slug: icml
abstract: 'In the graph node embedding problem, embedding spaces can vary significantly
  for different data types, leading to the need for different GNN model types. In
  this paper, we model the embedding update of a node feature as a Hamiltonian orbit
  over time. Since the Hamiltonian orbits generalize the exponential maps, this approach
  allows us to learn the underlying manifold of the graph in training, in contrast
  to most of the existing literature that assumes a fixed graph embedding manifold
  with a closed exponential map solution. Our proposed node embedding strategy can
  automatically learn, without extensive tuning, the underlying geometry of any given
  graph dataset even if it has diverse geometries. We test Hamiltonian functions of
  different forms and verify the performance of our approach on two graph node embedding
  downstream tasks: node classification and link prediction. Numerical experiments
  demonstrate that our approach adapts better to different types of graph datasets
  than popular state-of-the-art graph node embedding GNNs. The code is available at.'
codebase_url: https://github.com/zknus/Hamiltonian-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 1
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Cora-CA
  rows:
  - model: HAN (full batch)
    model_key: han (full batch)
    model_plain: HAN (full batch)
    value: 0.8404
    std: 0.0102
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8404
    sort_std: 0.0102
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AllSetTransformer
    model_key: allsettransformer
    model_plain: AllSetTransformer
    value: 0.8363
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8363
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UniGCNII
    model_key: unigcnii
    model_plain: UniGCNII
    value: 0.836
    std: 0.0114
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.836
    sort_std: 0.0114
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.8204
    std: 0.0127
    paper_value: 0.8204
    paper_std: 0.0127
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
    variant_inference_reason: 'dataset: fuzzy match to cora-ca (score=80)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 30, 2023
    date_display: May 2023
    date_iso: '2023-05-30'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-30'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8204
    true_std: 0.0127
    value_gap_source_arxiv: '2305.18965'
    value_gap_source_title: Node Embedding from Neural Hamiltonian Orbits in Graph
      Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8204
    sort_std: 0.0127
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HGCN
    model_key: hgcn
    model_plain: HGCN
    value: 0.7872
    std: 0.0042
    paper_value: 0.7872
    paper_std: 0.0042
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
    variant_inference_reason: 'dataset: fuzzy match to cora-ca (score=80)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 30, 2023
    date_display: May 2023
    date_iso: '2023-05-30'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-30'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7872
    true_std: 0.0042
    value_gap_source_arxiv: '2305.18965'
    value_gap_source_title: Node Embedding from Neural Hamiltonian Orbits in Graph
      Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7872
    sort_std: 0.0042
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7516
    std: 0.0065
    paper_value: 0.7516
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to cora-ca (score=80)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 30, 2023
    date_display: May 2023
    date_iso: '2023-05-30'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.7366
    at_pub_std: 0.013
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2023-05-30'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.015000000000000013
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7516
    true_std: 0.0065
    value_gap_source_arxiv: '2305.18965'
    value_gap_source_title: Node Embedding from Neural Hamiltonian Orbits in Graph
      Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7516
    sort_std: 0.0065
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7431
    std: 0.0189
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_display: Jun 2021
    date_iso: '2021-06-24'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jianhao2016/AllSet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 30
    sort_value: 0.7431
    sort_std: 0.0189
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
  - model: HamGNN
    model_key: hamgnn
    model_plain: HamGNN
    value: 0.7987
    std: null
    paper_value: 0.7987
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
    table_ref: Table 10 (last row snippet)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 30, 2023
    date_display: May 2023
    date_iso: '2023-05-30'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-30'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7987
    true_std: null
    value_gap_source_arxiv: '2305.18965'
    value_gap_source_title: Node Embedding from Neural Hamiltonian Orbits in Graph
      Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7987
    sort_std: null
    global_rank: 172
    paper_rank: 172
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
    global_rank: 394
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
- benchmark: Hypergraph Benchmarks
  datasets:
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
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: Cora-CA
      dataset_slug: cora-ca
main_figure: /figures/2305.18965/main_figure.jpegoptim.jpg
---

