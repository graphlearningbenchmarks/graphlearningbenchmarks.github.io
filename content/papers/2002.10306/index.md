---
title: Adaptive Propagation Graph Convolutional Network
arxiv_id: '2002.10306'
source_url: ''
authors:
- name: Indro Spinelli
  orcid: null
  s2_author_id: '115566972'
  s2_url: null
- name: Simone Scardapane
  orcid: null
  s2_author_id: '1752983'
  s2_url: null
- name: A. Uncini
  orcid: null
  s2_author_id: '1737292'
  s2_url: null
published_date: Feb 24, 2020
published_date_iso: '2020-02-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph convolutional networks (GCNs) are a family of neural network models
  that perform inference on graph data by interleaving vertex-wise operations and
  message-passing exchanges across nodes. Concerning the latter, two key questions
  arise: (i) how to design a differentiable exchange protocol (e.g., a $1$-hop Laplacian
  smoothing in the original GCN), and (ii) how to characterize the trade-off in complexity
  with respect to the local updates. In this paper, we show that state-of-the-art
  results can be achieved by adapting the number of communication steps independently
  at every node. In particular, we endow each node with a halting unit (inspired by
  Graves'' adaptive computation time) that after every exchange decides whether to
  continue communicating or not. We show that the proposed adaptive propagation GCN
  (AP-GCN) achieves superior or similar results to the best proposed models so far
  on a number of benchmarks, while requiring a small overhead in terms of additional
  parameters. We also investigate a regularization term to enforce an explicit trade-off
  between communication and accuracy. The code for the AP-GCN experiments is released
  as an open-source library.'
codebase_url: https://github.com/spindro/AP-GCN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
- AP-GCN
mrr: 0.1984
adjusted_mrr: 0.1984
mrr_dataset_count: 3
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
  dataset: Amazon-Computers
  rows:
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7862
    std: 0.003
    paper_value: 0.7862
    paper_std: 0.003
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy with 20 nodes per class in training set
    date: Feb 24, 2020
    date_display: Feb 2020
    date_iso: '2020-02-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.819
    at_pub_std: 0.017
    at_pub_source_arxiv: '1911.07123'
    at_pub_source_title: Graph-Revised Convolutional Network
    at_pub_source_date_iso: '2019-11-17'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03279999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.15500000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 474
    rank_delta: 472
    rank_delta_abs: 472
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Revised Convolutional Network
    comparison_source_arxiv: '1911.07123'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7608
    std: 0.0047
    paper_value: 0.7608
    paper_std: 0.0047
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy with 20 nodes per class in training set
    date: Feb 24, 2020
    date_display: Feb 2020
    date_iso: '2020-02-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.818
    at_pub_std: 0.02
    at_pub_source_arxiv: '1911.07123'
    at_pub_source_title: Graph-Revised Convolutional Network
    at_pub_source_date_iso: '2019-11-17'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05719999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.17899999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 482
    rank_delta: 479
    rank_delta_abs: 479
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Revised Convolutional Network
    comparison_source_arxiv: '1911.07123'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8017
    std: 0.0031
    paper_value: 0.8017
    paper_std: 0.0031
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy with 20 nodes per class in training set
    date: Feb 24, 2020
    date_display: Feb 2020
    date_iso: '2020-02-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9093
    true_std: 0.0018
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.10760000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9093
    sort_std: 0.0018
    global_rank: 84
    paper_rank: 464
    rank_delta: 380
    rank_delta_abs: 380
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AP-GCN
    model_key: ap-gcn
    model_plain: AP-GCN
    value: 0.8518
    std: 0.0023
    paper_value: 0.8518
    paper_std: 0.0023
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy with 20 nodes per class in training set
    date: Feb 24, 2020
    date_display: Feb 2020
    date_iso: '2020-02-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-02-24'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8518
    true_std: 0.0023
    value_gap_source_arxiv: '2002.10306'
    value_gap_source_title: Adaptive Propagation Graph Convolutional Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8518
    sort_std: 0.0023
    global_rank: 349
    paper_rank: 349
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ARMA
    model_key: arma
    model_plain: ARMA
    value: 0.8075
    std: 0.0037
    paper_value: 0.8075
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=77)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average accuracy with 20 nodes per class in training set
    date: Feb 24, 2020
    date_display: Feb 2020
    date_iso: '2020-02-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.638
    at_pub_std: 0.189
    at_pub_source_arxiv: '1909.03211'
    at_pub_source_title: Measuring and Relieving the Over-smoothing Problem for Graph
      Neural Networks from the Topological View
    at_pub_source_date_iso: '2019-09-07'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.16949999999999998
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8383
    true_std: 0.0058
    value_gap_source_arxiv: '2407.11361'
    value_gap_source_title: 'Graph Structure Prompt Learning: A Novel Methodology
      to Improve Performance of Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.03080000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8383
    sort_std: 0.0058
    global_rank: 393
    paper_rank: 461
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
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
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
main_figure: /figures/2002.10306/main_figure.jpegoptim.jpg
---

