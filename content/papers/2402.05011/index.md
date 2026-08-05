---
title: 'Navigating Complexity: Toward Lossless Graph Condensation via Expanding Window
  Matching'
arxiv_id: '2402.05011'
source_url: ''
authors:
- name: Yuchen Zhang
  orcid: null
  s2_author_id: '2254849450'
  s2_url: null
- name: Tianle Zhang
  orcid: null
  s2_author_id: '2256233019'
  s2_url: null
- name: Kai Wang
  orcid: null
  s2_author_id: '2283053585'
  s2_url: null
- name: Ziyao Guo
  orcid: null
  s2_author_id: '2257137154'
  s2_url: null
- name: Yuxuan Liang
  orcid: null
  s2_author_id: '2268400993'
  s2_url: null
- name: Xavier Bresson
  orcid: null
  s2_author_id: '2279831845'
  s2_url: null
- name: Wei Jin
  orcid: null
  s2_author_id: '2283256874'
  s2_url: null
- name: Yang You
  orcid: null
  s2_author_id: '2283134324'
  s2_url: null
published_date: Feb 7, 2024
published_date_iso: '2024-02-07'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: Graph condensation aims to reduce the size of a large-scale graph dataset
  by synthesizing a compact counterpart without sacrificing the performance of Graph
  Neural Networks (GNNs) trained on it, which has shed light on reducing the computational
  cost for training GNNs. Nevertheless, existing methods often fall short of accurately
  replicating the original graph for certain datasets, thereby failing to achieve
  the objective of lossless condensation. To understand this phenomenon, we investigate
  the potential reasons and reveal that the previous state-of-the-art trajectory matching
  method provides biased and restricted supervision signals from the original graph
  when optimizing the condensed one. This significantly limits both the scale and
  efficacy of the condensed graph. In this paper, we make the first attempt toward
  lossless graph condensation by bridging the previously neglected supervision signals.
  Specifically, we employ a curriculum learning strategy to train expert trajectories
  with more diverse supervision signals from the original graph, and then effectively
  transfer the information into the condensed graph with expanding window matching.
  Moreover, we design a loss function to further extract knowledge from the expert
  trajectories. Theoretical analysis justifies the design of our method and extensive
  experiments verify its superiority across different datasets. Code is released at
  https://github.com/NUS-HPC-AI-Lab/GEOM.
codebase_url: https://github.com/NUS-HPC-AI-Lab/GEOM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GEOM
mrr: 0.0033
adjusted_mrr: 0.0011
mrr_dataset_count: 1
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
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GEOM
    model_key: geom
    model_plain: GEOM
    value: 0.829
    std: 0.01
    paper_value: 0.829
    paper_std: 0.01
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      used for evaluation on condensed graphs.
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.8527
    at_pub_std: null
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.023700000000000054
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8527
    true_std: null
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.023700000000000054
    has_value_note: false
    value_note: ''
    sort_value: 0.8527
    sort_std: null
    global_rank: 304
    paper_rank: 546
    rank_delta: 242
    rank_delta_abs: 242
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    comparison_source_arxiv: '2211.11761'
    is_best: false
    is_std_outlier: false
  - model: SFGC
    model_key: sfgc
    model_plain: SFGC
    value: 0.643
    std: 0.016
    paper_value: 0.643
    paper_std: 0.016
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      used for evaluation on condensed graphs.
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.817
    at_pub_std: 0.005
    at_pub_source_arxiv: '2402.04924'
    at_pub_source_title: 'Two Trades are not Baffled: Condensing Graph via Crafting
      Rational Gradient Matching'
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.17399999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.817
    true_std: 0.005
    value_gap_source_arxiv: '2402.04924'
    value_gap_source_title: 'Two Trades are not Baffled: Condensing Graph via Crafting
      Rational Gradient Matching'
    value_gap_source_is_current_paper: false
    value_gap: 0.17399999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: 0.005
    global_rank: 682
    paper_rank: 980
    rank_delta: 298
    rank_delta_abs: 298
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Two Trades are not Baffled: Condensing Graph via Crafting
      Rational Gradient Matching'
    comparison_source_arxiv: '2402.04924'
    is_best: false
    is_std_outlier: false
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.614
    std: 0.029
    paper_value: 0.614
    paper_std: 0.029
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      used for evaluation on condensed graphs.
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.801
    at_pub_std: 0.006
    at_pub_source_arxiv: '2402.04924'
    at_pub_source_title: 'Two Trades are not Baffled: Condensing Graph via Crafting
      Rational Gradient Matching'
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.18700000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.809
    true_std: 0.032
    value_gap_source_arxiv: '2407.08064'
    value_gap_source_title: 'TinyGraph: Joint Feature and Node Condensation for Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.19500000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.809
    sort_std: 0.032
    global_rank: 744
    paper_rank: 985
    rank_delta: 241
    rank_delta_abs: 241
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Two Trades are not Baffled: Condensing Graph via Crafting
      Rational Gradient Matching'
    comparison_source_arxiv: '2402.04924'
    is_best: false
    is_std_outlier: false
  - model: DC-Graph
    model_key: dc-graph
    model_plain: DC-Graph
    value: 0.593
    std: 0.016
    paper_value: 0.593
    paper_std: 0.016
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      used for evaluation on condensed graphs.
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.593
    true_std: 0.016
    value_gap_source_arxiv: '2402.05011'
    value_gap_source_title: 'Navigating Complexity: Toward Lossless Graph Condensation
      via Expanding Window Matching'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.593
    sort_std: 0.016
    global_rank: 994
    paper_rank: 994
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
    - dataset: Cora
      dataset_slug: cora
single_proposed_model: GEOM
main_figure: /figures/2402.05011/main_figure.jpegoptim.jpg
---

