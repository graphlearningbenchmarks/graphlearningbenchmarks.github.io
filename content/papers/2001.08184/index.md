---
title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
arxiv_id: '2001.08184'
source_url: ''
authors:
- name: Nikhil Goyal
  orcid: null
  s2_author_id: '2066989298'
  s2_url: null
- name: Harsh Vardhan Jain
  orcid: null
  s2_author_id: '2059143233'
  s2_url: null
- name: Sayan Ranu
  orcid: null
  s2_author_id: '1699732'
  s2_url: null
published_date: Jan 22, 2020
published_date_iso: '2020-01-22'
published_venue: WWW 2020
published_conference: WWW 2020
published_conference_short: WWW
published_conference_slug: www
abstract: Graph generative models have been extensively studied in the data mining
  literature. While traditional techniques are based on generating structures that
  adhere to a pre-decided distribution, recent techniques have shifted towards learning
  this distribution directly from the data. While learning-based approaches have imparted
  significant improvement in quality, some limitations remain to be addressed. First,
  learning graph distributions introduces additional computational overhead, which
  limits their scalability to large graph databases. Second, many techniques only
  learn the structure and do not address the need to also learn node and edge labels,
  which encode important semantic information and influence the structure itself.
  Third, existing techniques often incorporate domain-specific rules and lack generalizability.
  Fourth, the experimentation of existing techniques is not comprehensive enough due
  to either using weak evaluation metrics or focusing primarily on synthetic or small
  datasets. In this work, we develop a domain-agnostic technique called GraphGen to
  overcome all of these limitations. GraphGen converts graphs to sequences using minimum
  DFS codes. Minimum DFS codes are canonical labels and capture the graph structure
  precisely along with the label information. The complex joint distributions between
  structure and semantic labels are learned through a novel LSTM architecture. Extensive
  experiments on million-sized, real graph datasets show GraphGen to be $4$ times
  faster on average than state-of-the-art techniques while being significantly better
  in quality across a comprehensive set of $11$ different metrics. Our code is released
  at:.
codebase_url: https://github.com/idea-iitd/graphgen
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphGen
mrr: 0.0
adjusted_mrr: 0.0
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
  dataset: ENZYMES
  is_multi_metric: true
  rows:
  - model: CatFlow
    model_key: catflow
    model_plain: CatFlow
    metric_values:
    - 0.008
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.04843'
    title: Variational Flow Matching for Graph Generation
    published_venue: ''
    date: Jun 7, 2024
    date_display: Jun 2024
    date_iso: '2024-06-07'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.008
    sort_std: 0.007
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphGen
    model_key: graphgen
    model_plain: GraphGen
    metric_values:
    - null
    - 0.016
    - 0.051
    - 0.249
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.016
    sort_std: null
    true_value: 0.016
    true_std: null
    paper_value: 0.016
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2001.08184'
    value_gap_source_title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled
      Graph Generation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-01-22'
    value_gap_source_date_label: WWW 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: WWW 2020
    date: Jan 22, 2020
    date_display: Jan 2020
    date_iso: '2020-01-22'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: GraphRNN
    model_key: graphrnn
    model_plain: GraphRNN
    metric_values:
    - null
    - 0.038
    - 0.067
    - 0.312
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.038
    sort_std: null
    true_value: 0.038
    true_std: null
    paper_value: 0.038
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2001.08184'
    value_gap_source_title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled
      Graph Generation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-01-22'
    value_gap_source_date_label: WWW 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: WWW 2020
    date: Jan 22, 2020
    date_display: Jan 2020
    date_iso: '2020-01-22'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  metrics:
  - Accuracy
  - Orbit
  - NSPDK
  - Joint Node Label & Degree
  - Uniqueness
  primary_metric: Accuracy
  rank_metric: Orbit
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Orbit
  - NSPDK
  - Joint Node Label & Degree
  - Uniqueness
  metric: Orbit
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: GraphGen
main_figure: /figures/2001.08184/main_figure.jpegoptim.jpg
---

