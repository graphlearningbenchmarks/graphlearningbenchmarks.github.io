---
title: GraphBench
arxiv_id: '2512.04475'
source_url: ''
authors:
- name: Timo Stoll
  orcid: null
  s2_author_id: '2373023981'
  s2_url: null
- name: Chendi Qian
  orcid: null
  s2_author_id: '2253440539'
  s2_url: null
- name: Ben Finkelshtein
  orcid: null
  s2_author_id: '2253392547'
  s2_url: null
- name: Alipanah Parviz
  orcid: null
  s2_author_id: '84094194'
  s2_url: null
- name: Darius Weber
  orcid: null
  s2_author_id: '2396374048'
  s2_url: null
- name: Fabrizio Frasca
  orcid: null
  s2_author_id: '51484149'
  s2_url: null
- name: Hadar Shavit
  orcid: null
  s2_author_id: '2310896181'
  s2_url: null
- name: Antoine Siraudin
  orcid: null
  s2_author_id: '2186404013'
  s2_url: null
- name: Arman Mielke
  orcid: null
  s2_author_id: '2347345328'
  s2_url: null
- name: Marie Anastacio
  orcid: null
  s2_author_id: '2355348522'
  s2_url: null
- name: Erik Muller
  orcid: null
  s2_author_id: '2061778304'
  s2_url: null
- name: Maya Bechler-Speicher
  orcid: null
  s2_author_id: '2412075764'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2303841731'
  s2_url: null
- name: Mikhail Galkin
  orcid: null
  s2_author_id: '2373458958'
  s2_url: null
- name: Holger H. Hoos
  orcid: null
  s2_author_id: '2355183412'
  s2_url: null
- name: Mathias Niepert
  orcid: null
  s2_author_id: '2253455028'
  s2_url: null
- name: Bryan Perozzi
  orcid: null
  s2_author_id: '2271808'
  s2_url: null
- name: Jan Tonshoff
  orcid: null
  s2_author_id: '2182291897'
  s2_url: null
- name: Christopher Morris
  orcid: null
  s2_author_id: '2305618073'
  s2_url: null
published_date: Dec 4, 2025
published_date_iso: '2025-12-04'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Machine learning on graphs has made substantial progress across domains
  such as molecular property prediction and chip design. Yet benchmarking practices
  remain fragmented, often relying on narrow, task-specific datasets and inconsistent
  evaluation protocols, hindering reproducibility and broader progress. With the recent
  popularity of graph foundation models, these weaknesses have become apparent, as
  existing benchmarks are insufficient for thorough evaluation. To address these challenges,
  we introduce GraphBench, a comprehensive benchmark suite spanning diverse real-world
  domains and task settings, including node-level, edge-level, graph-level, and generative
  tasks. GraphBench provides standardized evaluation protocols, including consistent
  dataset splits and metrics for assessing out-of-distribution generalization across
  selected tasks, as well as a unified hyperparameter-tuning framework. We further
  evaluate GraphBench with recent message-passing neural networks and graph transformer
  models, establishing principled baselines for future research. See www.graphbench.io
  for further details.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: SAT Solving
  rows:
  - model: PR
    model_key: pr
    model_plain: PR
    value: 0.51
    std: 0.01
    paper_value: 0.51
    paper_std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 1
    input_feature_source: other_external_features
    feature_source_evidence: SATzilla feature-based baselines
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Large instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.51
    true_std: 0.01
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.51
    sort_std: 0.01
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.45
    std: 0.0
    paper_value: 0.45
    paper_std: 0.0
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
    feature_source_evidence: forcing them to learn solely from the graph structure
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Small instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.45
    true_std: 0.0
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.45
    sort_std: 0.0
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Gated GCN+
    model_key: gated gcn+
    model_plain: Gated GCN+
    value: 0.4
    std: 0.04
    paper_value: 0.4
    paper_std: 0.04
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
    feature_source_evidence: forcing them to learn solely from the graph structure
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Small instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4
    true_std: 0.04
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4
    sort_std: 0.04
    global_rank: 3
    paper_rank: 3
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
    value: 0.31
    std: 0.0
    paper_value: 0.31
    paper_std: 0.0
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
    feature_source_evidence: forcing them to learn solely from the graph structure
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Small instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.31
    true_std: 0.0
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.31
    sort_std: 0.0
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PC
    model_key: pc
    model_plain: PC
    value: 0.21
    std: 0.01
    paper_value: 0.21
    paper_std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 1
    input_feature_source: other_external_features
    feature_source_evidence: SATzilla feature-based baselines
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Large instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.21
    true_std: 0.01
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.21
    sort_std: 0.01
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
  - model: MC
    model_key: mc
    model_plain: MC
    value: -0.05
    std: 0.01
    paper_value: -0.05
    paper_std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 1
    input_feature_source: other_external_features
    feature_source_evidence: SATzilla feature-based baselines
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Large instances, fixed train-validation-test split as described
      in text
    date: Dec 4, 2025
    date_display: Dec 2025
    date_iso: '2025-12-04'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -0.05
    true_std: 0.01
    value_gap_source_arxiv: '2512.04475'
    value_gap_source_title: GraphBench
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -0.05
    sort_std: 0.01
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
- benchmark: GraphBench
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: SAT Solving
      dataset_slug: sat-solving
main_figure: /figures/2512.04475/main_figure.jpegoptim.jpg
---

