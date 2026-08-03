---
title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
arxiv_id: '2102.05034'
source_url: ''
authors:
- name: Bahare Fatemi
  orcid: null
  s2_author_id: '3422551'
  s2_url: null
- name: Layla El Asri
  orcid: null
  s2_author_id: '3349496'
  s2_url: null
- name: Seyed Mehran Kazemi
  orcid: null
  s2_author_id: '2470890'
  s2_url: null
published_date: Feb 9, 2021
published_date_iso: '2021-02-09'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph neural networks (GNNs) work well when the graph structure is provided.
  However, this structure may not always be available in real-world applications.
  One solution to this problem is to infer a task-specific latent structure and then
  apply a GNN to the inferred graph. Unfortunately, the space of possible graph structures
  grows super-exponentially with the number of nodes and so the task-specific supervision
  may be insufficient for learning both the structure and the GNN parameters. In this
  work, we propose the Simultaneous Learning of Adjacency and GNN Parameters with
  Self-supervision, or SLAPS, a method that provides more supervision for inferring
  a graph structure through self-supervision. A comprehensive experimental study demonstrates
  that SLAPS scales to large graphs with hundreds of thousands of nodes and outperforms
  several models that have been proposed to learn a task-specific graph structure
  on established benchmarks.
codebase_url: https://github.com/BorealisAI/SLAPS-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SLAPS (MLP-D)
- SLAPS (MLP) + AdaEdge
- SLAPS (MLP) + self-training
- SLAPS (MLP)
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: 20News
  rows:
  - model: LDS
    model_key: arma
    model_plain: LDS
    value: 0.7002
    std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_display: Jan 2019
    date_iso: '2019-01-05'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7002
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LDS
    model_key: cayleynet
    model_plain: LDS
    value: 0.6884
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_display: Jan 2019
    date_iso: '2019-01-05'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6884
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDS
    model_key: chebyshev
    model_plain: LDS
    value: 0.6824
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_display: Jan 2019
    date_iso: '2019-01-05'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6824
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SLAPS (MLP)
    model_key: slaps (mlp)
    model_plain: SLAPS (MLP)
    value: 0.504
    std: 0.007
    paper_value: 0.504
    paper_std: 0.007
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: scikit-learn classification task
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.504
    true_std: 0.007
    value_gap_source_arxiv: '2102.05034'
    value_gap_source_title: 'SLAPS: Self-Supervision Improves Structure Learning for
      Graph Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.504
    sort_std: 0.007
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IDGL
    model_key: idgl
    model_plain: IDGL
    value: 0.485
    std: 0.006
    paper_value: 0.485
    paper_std: 0.006
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
    protocol_note: scikit-learn classification task
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.485
    true_std: 0.006
    value_gap_source_arxiv: '2102.05034'
    value_gap_source_title: 'SLAPS: Self-Supervision Improves Structure Learning for
      Graph Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.485
    sort_std: 0.006
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LDS
    model_key: lds
    model_plain: LDS
    value: 0.464
    std: 0.016
    paper_value: 0.464
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: franceschi2019learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: scikit-learn classification task
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.464
    at_pub_std: 0.016
    at_pub_source_arxiv: '1903.11960'
    at_pub_source_title: Learning Discrete Structures for Graph Neural Networks
    at_pub_source_date_iso: '2019-03-28'
    at_pub_source_date_label: ICML 2019
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.464
    true_std: 0.016
    value_gap_source_arxiv: '2102.05034'
    value_gap_source_title: 'SLAPS: Self-Supervision Improves Structure Learning for
      Graph Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.464
    sort_std: 0.016
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: kNN-GCN
    model_key: knn-gcn
    model_plain: kNN-GCN
    value: 0.463
    std: 0.003
    paper_value: 0.463
    paper_std: 0.003
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
    protocol_note: scikit-learn classification task
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.413
    at_pub_std: 0.006
    at_pub_source_arxiv: '1903.11960'
    at_pub_source_title: Learning Discrete Structures for Graph Neural Networks
    at_pub_source_date_iso: '2019-03-28'
    at_pub_source_date_label: ICML 2019
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.463
    true_std: 0.003
    value_gap_source_arxiv: '2102.05034'
    value_gap_source_title: 'SLAPS: Self-Supervision Improves Structure Learning for
      Graph Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.463
    sort_std: 0.003
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Learning Discrete Structures for Graph Neural Networks
    comparison_source_arxiv: '1903.11960'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.304
    std: 0.001
    paper_value: 0.304
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: scikit-learn classification task
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.304
    true_std: 0.001
    value_gap_source_arxiv: '2102.05034'
    value_gap_source_title: 'SLAPS: Self-Supervision Improves Structure Learning for
      Graph Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.304
    sort_std: 0.001
    global_rank: 19
    paper_rank: 19
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: 20News
      dataset_slug: 20news
---

