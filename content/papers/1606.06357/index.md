---
title: Complex Embeddings for Simple Link Prediction
arxiv_id: '1606.06357'
source_url: ''
authors:
- name: Théo Trouillon
  orcid: null
  s2_author_id: '2057146'
  s2_url: null
- name: Johannes Welbl
  orcid: null
  s2_author_id: '1851564'
  s2_url: null
- name: Sebastian Riedel
  orcid: null
  s2_author_id: '48662861'
  s2_url: null
- name: Éric Gaussier
  orcid: null
  s2_author_id: '1732180'
  s2_url: null
- name: Guillaume Bouchard
  orcid: null
  s2_author_id: '1684865'
  s2_url: null
published_date: Jun 19, 2016
published_date_iso: '2016-06-19'
published_venue: ICML 2016
published_conference: ICML 2016
published_conference_short: ICML
published_conference_slug: icml
abstract: In statistical relational learning, the link prediction problem is key to
  automatically understand the structure of large knowledge bases. As in previous
  studies, we propose to solve this problem through latent factorization. However,
  here we make use of complex valued embeddings. The composition of complex embeddings
  can handle a large variety of binary relations, among them symmetric and antisymmetric
  relations. Compared to state-of-the-art models such as Neural Tensor Network and
  Holographic Embeddings, our approach based on complex embeddings is arguably simpler,
  as it only uses the Hermitian dot product, the complex counterpart of the standard
  dot product between real vectors. Our approach is scalable to large datasets as
  it remains linear in both space and time, while consistently outperforming alternative
  approaches on standard link prediction benchmarks.
codebase_url: https://github.com/ttrouill/complex
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
  dataset: WN18
  rows:
  - model: TripleRE
    model_key: rotate
    model_plain: TripleRE
    value: 0.949
    std: 0.0
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: Sep 27, 2018
    date_display: Sep 2018
    date_iso: '2018-09-27'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraphEmbedding
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.949
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TripleRE
    model_key: complex
    model_plain: TripleRE
    value: 0.941
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.06103'
    title: Modeling Relational Data with Graph Convolutional Networks
    date: Mar 17, 2017
    date_display: Mar 2017
    date_iso: '2017-03-17'
    venue: Extended Semantic Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.941
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HolE
    model_key: hole
    model_plain: HolE
    value: 0.938
    std: null
    paper_value: 0.938
    paper_std: null
    metric: MRR
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
    table_ref: "Table \ref{tab:fb15k_wn18_res}"
    source_ref: nickel_2016_holographic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 test split
    date: Jun 19, 2016
    date_display: Jun 2016
    date_iso: '2016-06-19'
    published_venue: ICML 2016
    published_conference: ICML 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.938
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.938
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
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.822
    std: null
    paper_value: 0.822
    paper_std: null
    metric: MRR
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
    table_ref: "Table \ref{tab:fb15k_wn18_res}"
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 test split
    date: Jun 19, 2016
    date_display: Jun 2016
    date_iso: '2016-06-19'
    published_venue: ICML 2016
    published_conference: ICML 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.822
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: null
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
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.454
    std: null
    paper_value: 0.454
    paper_std: null
    metric: MRR
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
    table_ref: "Table \ref{tab:fb15k_wn18_res}"
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 test split
    date: Jun 19, 2016
    date_display: Jun 2016
    date_iso: '2016-06-19'
    published_venue: ICML 2016
    published_conference: ICML 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.454
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.454
    sort_std: null
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
  - model: CP
    model_key: cp
    model_plain: CP
    value: 0.075
    std: null
    paper_value: 0.075
    paper_std: null
    metric: MRR
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
    table_ref: "Table \ref{tab:fb15k_wn18_res}"
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Filtered MRR on WN18 test split
    date: Jun 19, 2016
    date_display: Jun 2016
    date_iso: '2016-06-19'
    published_venue: ICML 2016
    published_conference: ICML 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-06-19'
    value_gap_source_date_label: ICML 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.075
    true_std: null
    value_gap_source_arxiv: '1606.06357'
    value_gap_source_title: Complex Embeddings for Simple Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.075
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
    - dataset: WN18
      dataset_slug: wn18
---

