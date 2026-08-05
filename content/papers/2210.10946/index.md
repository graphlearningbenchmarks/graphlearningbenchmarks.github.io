---
title: Causally-guided Regularization of Graph Attention Improves Generalizability
arxiv_id: '2210.10946'
source_url: ''
authors:
- name: Alexander P. Wu
  orcid: null
  s2_author_id: '2075409981'
  s2_url: null
- name: Thomas Markovich
  orcid: null
  s2_author_id: '47966426'
  s2_url: null
- name: Bonnie Berger
  orcid: null
  s2_author_id: '2055375593'
  s2_url: null
- name: Nils Y. Hammerla
  orcid: null
  s2_author_id: '3128867'
  s2_url: null
- name: Rohit Singh
  orcid: null
  s2_author_id: '2115508790'
  s2_url: null
published_date: Oct 20, 2022
published_date_iso: '2022-10-20'
published_venue: TMLR 2022
published_conference: TMLR 2022
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Graph attention networks estimate the relational importance of node neighbors
  to aggregate relevant information over local neighborhoods for a prediction task.
  However, the inferred attentions are vulnerable to spurious correlations and connectivity
  in the training data, hampering the generalizability of models. We introduce CAR,
  a general-purpose regularization framework for graph attention networks. Embodying
  a causal inference approach based on invariance prediction, CAR aligns the attention
  mechanism with the causal effects of active interventions on graph connectivity
  in a scalable manner. CAR is compatible with a variety of graph attention architectures,
  and we show that it systematically improves generalizability on various node classification
  tasks. Our ablation studies indicate that CAR hones in on the aspects of graph structure
  most pertinent to the prediction (e.g., homophily), and does so more effectively
  than alternative approaches. Finally, we also show that CAR enhances interpretability
  of attention coefficients by accentuating node-neighbor relations that point to
  causal hypotheses.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  - model: GATv2 + CAR
    model_key: gatv2 + car
    model_plain: GATv2 + CAR
    value: 1.63
    std: 0.59
    paper_value: 1.63
    paper_std: 0.59
    metric: Loss
    higher_is_better: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.63
    true_std: 0.59
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.63
    sort_std: 0.59
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
  - model: Transformer + CAR
    model_key: transformer + car
    model_plain: Transformer + CAR
    value: 1.71
    std: 0.5
    paper_value: 1.71
    paper_std: 0.5
    metric: Loss
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.71
    true_std: 0.5
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.71
    sort_std: 0.5
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT + CAR
    model_key: gat + car
    model_plain: GAT + CAR
    value: 1.82
    std: 0.77
    paper_value: 1.82
    paper_std: 0.77
    metric: Loss
    higher_is_better: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.82
    true_std: 0.77
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.82
    sort_std: 0.77
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 2.26
    std: 0.54
    paper_value: 2.26
    paper_std: 0.54
    metric: Loss
    higher_is_better: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.26
    true_std: 0.54
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.26
    sort_std: 0.54
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 2.33
    std: 0.75
    paper_value: 2.33
    paper_std: 0.75
    metric: Loss
    higher_is_better: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.33
    true_std: 0.75
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.33
    sort_std: 0.75
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Transformer
    model_key: transformer
    model_plain: Transformer
    value: 3.43
    std: 1.61
    paper_value: 3.43
    paper_std: 1.61
    metric: Loss
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Cora
    date: Oct 20, 2022
    date_display: Oct 2022
    date_iso: '2022-10-20'
    published_venue: TMLR 2022
    published_conference: TMLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-20'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.43
    true_std: 1.61
    value_gap_source_arxiv: '2210.10946'
    value_gap_source_title: Causally-guided Regularization of Graph Attention Improves
      Generalizability
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.43
    sort_std: 1.61
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  rank_metric: Loss
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Loss
  metric: Loss
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
main_figure: /figures/2210.10946/main_figure.jpegoptim.jpg
---

