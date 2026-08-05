---
title: Inductive Relation Prediction by Subgraph Reasoning
arxiv_id: '1911.06962'
source_url: ''
authors:
- name: Komal K. Teru
  orcid: null
  s2_author_id: '1419929288'
  s2_url: null
- name: E. Denis
  orcid: null
  s2_author_id: '114240083'
  s2_url: null
- name: William L. Hamilton
  orcid: null
  s2_author_id: '49437682'
  s2_url: null
published_date: Nov 16, 2019
published_date_iso: '2019-11-16'
published_venue: ICML 2019
published_conference: ICML 2019
published_conference_short: ICML
published_conference_slug: icml
abstract: The dominant paradigm for relation prediction in knowledge graphs involves
  learning and operating on latent representations (i.e., embeddings) of entities
  and relations. However, these embedding-based methods do not explicitly capture
  the compositional logical rules underlying the knowledge graph, and they are limited
  to the transductive setting, where the full set of entities must be known during
  training. Here, we propose a graph neural network based relation prediction framework,
  GraIL, that reasons over local subgraph structures and has a strong inductive bias
  to learn entity-independent relational semantics. Unlike embedding-based models,
  GraIL is naturally inductive and can generalize to unseen entities and graphs after
  training. We provide theoretical proof and strong empirical evidence that GraIL
  can represent a useful subset of first-order logic and show that GraIL outperforms
  existing rule-induction baselines in the inductive setting. We also demonstrate
  significant gains obtained by ensembling GraIL with various knowledge graph embedding
  methods in the transductive setting, highlighting the complementary inductive bias
  of our method.
codebase_url: https://github.com/kkteru/grail
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: FB15k-237
  rows:
  - model: GraIL
    model_key: grail
    model_plain: GraIL
    value: 0.9057
    std: null
    paper_value: 0.9057
    paper_std: null
    metric: AUC-PR
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 16, 2019
    date_display: Nov 2019
    date_iso: '2019-11-16'
    published_venue: ICML 2019
    published_conference: ICML 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-11-16'
    value_gap_source_date_label: ICML 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9057
    true_std: null
    value_gap_source_arxiv: '1911.06962'
    value_gap_source_title: Inductive Relation Prediction by Subgraph Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9057
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
  - model: RuleN
    model_key: rulen
    model_plain: RuleN
    value: 0.887
    std: null
    paper_value: 0.887
    paper_std: null
    metric: AUC-PR
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 16, 2019
    date_display: Nov 2019
    date_iso: '2019-11-16'
    published_venue: ICML 2019
    published_conference: ICML 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-11-16'
    value_gap_source_date_label: ICML 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.887
    true_std: null
    value_gap_source_arxiv: '1911.06962'
    value_gap_source_title: Inductive Relation Prediction by Subgraph Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: null
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
  - model: Neural-LP
    model_key: neural-lp
    model_plain: Neural-LP
    value: 0.7655
    std: null
    paper_value: 0.7655
    paper_std: null
    metric: AUC-PR
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 16, 2019
    date_display: Nov 2019
    date_iso: '2019-11-16'
    published_venue: ICML 2019
    published_conference: ICML 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-11-16'
    value_gap_source_date_label: ICML 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7655
    true_std: null
    value_gap_source_arxiv: '1911.06962'
    value_gap_source_title: Inductive Relation Prediction by Subgraph Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7655
    sort_std: null
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
  - model: DRUM
    model_key: drum
    model_plain: DRUM
    value: 0.7644
    std: null
    paper_value: 0.7644
    paper_std: null
    metric: AUC-PR
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 16, 2019
    date_display: Nov 2019
    date_iso: '2019-11-16'
    published_venue: ICML 2019
    published_conference: ICML 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-11-16'
    value_gap_source_date_label: ICML 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7644
    true_std: null
    value_gap_source_arxiv: '1911.06962'
    value_gap_source_title: Inductive Relation Prediction by Subgraph Reasoning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7644
    sort_std: null
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
  rank_metric: AUC-PR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - AUC-PR
  metric: AUC-PR
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: FB15k-237
      dataset_slug: fb15k-237
main_figure: /figures/1911.06962/main_figure.jpegoptim.jpg
---

