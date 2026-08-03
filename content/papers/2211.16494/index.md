---
title: On the Ability of Graph Neural Networks to Model Interactions Between Vertices
arxiv_id: '2211.16494'
source_url: ''
authors:
- name: Noam Razin
  orcid: null
  s2_author_id: '1388726511'
  s2_url: null
- name: Tom Verbin
  orcid: null
  s2_author_id: '2192703037'
  s2_url: null
- name: Nadav Cohen
  orcid: null
  s2_author_id: '32289606'
  s2_url: null
published_date: Nov 29, 2022
published_date_iso: '2022-11-29'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph neural networks (GNNs) are widely used for modeling complex interactions
  between entities represented as vertices of a graph. Despite recent efforts to theoretically
  analyze the expressive power of GNNs, a formal characterization of their ability
  to model interactions is lacking. The current paper aims to address this gap. Formalizing
  strength of interactions through an established measure known as separation rank,
  we quantify the ability of certain GNNs to model interaction between a given subset
  of vertices and its complement, i.e. between the sides of a given partition of input
  vertices. Our results reveal that the ability to model interaction is primarily
  determined by the partition's walk index -- a graph-theoretical characteristic defined
  by the number of walks originating from the boundary of the partition. Experiments
  with common GNN architectures corroborate this finding. As a practical application
  of our theory, we design an edge sparsification algorithm named Walk Index Sparsification
  (WIS), which preserves the ability of a GNN to model interactions when input edges
  are removed. WIS is simple, computationally efficient, and in our experiments has
  markedly outperformed alternative methods in terms of induced prediction accuracy.
  More broadly, it showcases the potential of improving GNNs by theoretically analyzing
  the interactions they can model.
codebase_url: https://github.com/noamrazin/gnn_interactions
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
mrr: 0.1795
adjusted_mrr: 0.1795
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
  - model: Matrix-valued
    model_key: graphtarif
    model_plain: Matrix-valued
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
    value: 0.662
    std: 0.011
    paper_value: 0.662
    paper_std: 0.011
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on the 'High' walk index partition of Amazon Computers
    date: Nov 29, 2022
    date_display: Nov 2022
    date_iso: '2022-11-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.8803
    at_pub_std: 0.0141
    at_pub_source_arxiv: '2208.06956'
    at_pub_source_title: 'ArieL: Adversarial Graph Contrastive Learning'
    at_pub_source_date_iso: '2022-08-15'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.21829999999999994
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
    value_gap: 0.2792
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 520
    rank_delta: 518
    rank_delta_abs: 518
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ArieL: Adversarial Graph Contrastive Learning'
    comparison_source_arxiv: '2208.06956'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.721
    std: 0.012
    paper_value: 0.721
    paper_std: 0.012
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on the 'High' walk index partition of Amazon Computers
    date: Nov 29, 2022
    date_display: Nov 2022
    date_iso: '2022-11-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.871
    at_pub_std: 0.004
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.15000000000000002
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
    value_gap: 0.2188
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 502
    rank_delta: 499
    rank_delta_abs: 499
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    comparison_source_arxiv: '2210.08792'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.648
    std: 0.014
    paper_value: 0.648
    paper_std: 0.014
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on the 'High' walk index partition of Amazon Computers
    date: Nov 29, 2022
    date_display: Nov 2022
    date_iso: '2022-11-29'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.7964
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2210.09789'
    at_pub_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    at_pub_source_date_iso: '2022-10-18'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-05-25'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.14839999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8626
    true_std: 0.0056
    value_gap_source_arxiv: '2305.15747'
    value_gap_source_title: Union Subgraph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2146
    has_value_note: false
    value_note: ''
    sort_value: 0.8626
    sort_std: 0.0056
    global_rank: 324
    paper_rank: 520
    rank_delta: 196
    rank_delta_abs: 196
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph
      Networks'
    comparison_source_arxiv: '2210.09789'
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
single_proposed_model: GCN
---

