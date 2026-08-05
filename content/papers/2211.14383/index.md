---
title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
arxiv_id: '2211.14383'
source_url: ''
authors:
- name: Yushun Dong
  orcid: null
  s2_author_id: '123918726'
  s2_url: null
- name: Song Wang
  orcid: null
  s2_author_id: '2117075272'
  s2_url: null
- name: Jing Ma
  orcid: null
  s2_author_id: '2157405959'
  s2_url: null
- name: Ninghao Liu
  orcid: null
  s2_author_id: '47717322'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '1737121128'
  s2_url: null
published_date: Nov 25, 2022
published_date_iso: '2022-11-25'
published_venue: AAAI 2022
published_conference: AAAI 2022
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Graph Neural Networks (GNNs) have emerged as the leading paradigm for solving
  graph analytical problems in various real-world applications. Nevertheless, GNNs
  could potentially render biased predictions towards certain demographic subgroups.
  Understanding how the bias in predictions arises is critical, as it guides the design
  of GNN debiasing mechanisms. However, most existing works overwhelmingly focus on
  GNN debiasing, but fall short on explaining how such bias is induced. In this paper,
  we study a novel problem of interpreting GNN unfairness through attributing it to
  the influence of training nodes. Specifically, we propose a novel strategy named
  Probabilistic Distribution Disparity (PDD) to measure the bias exhibited in GNNs,
  and develop an algorithm to efficiently estimate the influence of each training
  node on such bias. We verify the validity of PDD and the effectiveness of influence
  estimation through experiments on real-world datasets. Finally, we also demonstrate
  how the proposed framework could be used for debiasing GNNs. Open-source code can
  be found at https://github.com/yushundong/BIND.
codebase_url: https://github.com/yushundong/BIND
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BIND 1%
- BIND 10%
mrr: 0.0238
adjusted_mrr: 0.0079
mrr_dataset_count: 1
benchmark_categories:
- LINKX Benchmarks
benchmark_coverage:
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Pokec
  rows:
  - model: FMP
    model_key: polynormer-r
    model_plain: FMP
    value: 0.861
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.861
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FMP
    model_key: polynormer
    model_plain: FMP
    value: 0.8595
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8595
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FMP
    model_key: moe-h2gcn
    model_plain: FMP
    value: 0.8302
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_display: Nov 2023
    date_iso: '2023-11-09'
    venue: Accepted for publication in ICLR 2024
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8302
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NIFTY
    model_key: nifty
    model_plain: NIFTY
    value: 0.653
    std: 0.002
    paper_value: 0.653
    paper_std: 0.002
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
    source_ref: agarwal2021towards
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.653
    true_std: 0.002
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.653
    sort_std: 0.002
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FairGNN
    model_key: fairgnn
    model_plain: FairGNN
    value: 0.64
    std: 0.007
    paper_value: 0.64
    paper_std: 0.007
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
    source_ref: dai2021say
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64
    true_std: 0.007
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: 0.007
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BIND 1%
    model_key: bind 1%
    model_plain: BIND 1%
    value: 0.635
    std: 0.004
    paper_value: 0.635
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.635
    true_std: 0.004
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.635
    sort_std: 0.004
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Van. GCN
    model_key: van. gcn
    model_plain: Van. GCN
    value: 0.632
    std: 0.007
    paper_value: 0.632
    paper_std: 0.007
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
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.632
    true_std: 0.007
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.632
    sort_std: 0.007
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BIND 10%
    model_key: bind 10%
    model_plain: BIND 10%
    value: 0.629
    std: 0.004
    paper_value: 0.629
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.629
    true_std: 0.004
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.629
    sort_std: 0.004
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EDITS
    model_key: edits
    model_plain: EDITS
    value: 0.616
    std: 0.009
    paper_value: 0.616
    paper_std: 0.009
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
    source_ref: dong2021edits
    variant_inference_reason: 'dataset: fuzzy match to pokec (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Pokec-z dataset
    date: Nov 25, 2022
    date_display: Nov 2022
    date_iso: '2022-11-25'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.616
    true_std: 0.009
    value_gap_source_arxiv: '2211.14383'
    value_gap_source_title: Interpreting Unfairness in Graph Neural Networks via Training
      Node Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.616
    sort_std: 0.009
    global_rank: 46
    paper_rank: 46
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
- benchmark: LINKX Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: Pokec
      dataset_slug: pokec
main_figure: /figures/2211.14383/main_figure.jpegoptim.jpg
---

