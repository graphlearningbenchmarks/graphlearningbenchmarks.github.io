---
title: 'GOAt: Explaining Graph Neural Networks via Graph Output Attribution'
arxiv_id: '2401.14578'
source_url: ''
authors:
- name: Shengyao Lu
  orcid: null
  s2_author_id: '2165373965'
  s2_url: null
- name: Keith G. Mills
  orcid: null
  s2_author_id: '2066263931'
  s2_url: null
- name: Jiao He
  orcid: null
  s2_author_id: '2281739381'
  s2_url: null
- name: Bang Liu
  orcid: null
  s2_author_id: '2261686248'
  s2_url: null
- name: Di Niu
  orcid: null
  s2_author_id: '2264969180'
  s2_url: null
published_date: Jan 26, 2024
published_date_iso: '2024-01-26'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Understanding the decision-making process of Graph Neural Networks (GNNs)
  is crucial to their interpretability. Most existing methods for explaining GNNs
  typically rely on training auxiliary models, resulting in the explanations remain
  black-boxed. This paper introduces Graph Output Attribution (GOAt), a novel method
  to attribute graph outputs to input graph features, creating GNN explanations that
  are faithful, discriminative, as well as stable across similar samples. By expanding
  the GNN as a sum of scalar products involving node features, edge features and activation
  patterns, we propose an efficient analytical method to compute contribution of each
  node or edge feature to each scalar product and aggregate the contributions from
  all scalar products in the expansion form to derive the importance of each node
  and edge. Through extensive experiments on synthetic and real-world data, we show
  that our method not only outperforms various state-of-the-art GNN explainers in
  terms of the commonly used fidelity metric, but also exhibits stronger discriminability,
  and stability by a remarkable margin. Code can be found at:.
codebase_url: https://github.com/sluxsr/GOAt
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: NCI1
  rows:
  - model: ECC
    model_key: wl-mlp
    model_plain: ECC
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.83
    std: null
    paper_value: 0.83
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy of trained GNN on NCI1
    date: Jan 26, 2024
    date_display: Jan 2024
    date_iso: '2024-01-26'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.9934
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1634
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9934
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.1634
    has_value_note: false
    value_note: ''
    sort_value: 0.9934
    sort_std: null
    global_rank: 2
    paper_rank: 76
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.81
    std: null
    paper_value: 0.81
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy of trained GNN on NCI1
    date: Jan 26, 2024
    date_display: Jan 2024
    date_iso: '2024-01-26'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.9727
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.16269999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9727
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.16269999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9727
    sort_std: null
    global_rank: 3
    paper_rank: 172
    rank_delta: 169
    rank_delta_abs: 169
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8
    std: null
    paper_value: 0.8
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy of trained GNN on NCI1
    date: Jan 26, 2024
    date_display: Jan 2024
    date_iso: '2024-01-26'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: 0.8303
    at_pub_std: 0.0137
    at_pub_source_arxiv: '2310.01794'
    at_pub_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    at_pub_source_date_iso: '2023-10-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.030299999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8303
    true_std: 0.0137
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_gap_source_is_current_paper: false
    value_gap: 0.030299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8303
    sort_std: 0.0137
    global_rank: 76
    paper_rank: 226
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    comparison_source_arxiv: '2310.01794'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: NCI1
      dataset_slug: nci1
main_figure: /figures/2401.14578/main_figure.jpegoptim.jpg
---

