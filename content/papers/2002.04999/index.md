---
title: Differentiable Graph Module (DGM) for Graph Convolutional Networks
arxiv_id: '2002.04999'
source_url: ''
authors:
- name: Anees Kazi
  orcid: null
  s2_author_id: '32868927'
  s2_url: null
- name: Luca Cosmo
  orcid: null
  s2_author_id: '1904895'
  s2_url: null
- name: Seyed-Ahmad Ahmadi
  orcid: null
  s2_author_id: '145774206'
  s2_url: null
- name: N. Navab
  orcid: null
  s2_author_id: '145587209'
  s2_url: null
- name: M. Bronstein
  orcid: null
  s2_author_id: '1732570'
  s2_url: null
published_date: Feb 11, 2020
published_date_iso: '2020-02-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph deep learning has recently emerged as a powerful ML concept allowing
  to generalize successful deep neural architectures to non-Euclidean structured data.
  Such methods have shown promising results on a broad spectrum of applications ranging
  from social science, biomedicine, and particle physics to computer vision, graphics,
  and chemistry. One of the limitations of the majority of current graph neural network
  architectures is that they are often restricted to the transductive setting and
  rely on the assumption that the underlying graph is known and fixed. Often, this
  assumption is not true since the graph may be noisy, or partially and even completely
  unknown. In such cases, it would be helpful to infer the graph directly from the
  data, especially in inductive settings where some nodes were not present in the
  graph at training time. Furthermore, learning a graph may become an end in itself,
  as the inferred structure may provide complementary insights next to the downstream
  task. In this paper, we introduce Differentiable Graph Module (DGM), a learnable
  function that predicts edge probabilities in the graph which are optimal for the
  downstream task. DGM can be combined with convolutional graph neural network layers
  and trained in an end-to-end fashion. We provide an extensive evaluation of applications
  from the domains of healthcare (disease prediction), brain imaging (age prediction),
  computer graphics (3D point cloud segmentation), and computer vision (zero-shot
  learning). We show that our model provides a significant improvement over baselines
  both in transductive and inductive settings and achieves state-of-the-art results.
codebase_url: https://github.com/lcosmo/DGM_pytorch
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ShapeNet-Part
  rows:
  - model: dDGM
    model_key: ddgm
    model_plain: dDGM
    value: 0.856
    std: null
    paper_value: 0.856
    paper_std: null
    metric: mIoU
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 11, 2020
    date_display: Feb 2020
    date_iso: '2020-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.856
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.852
    std: null
    paper_value: 0.852
    paper_std: null
    metric: mIoU
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
    date: Feb 11, 2020
    date_display: Feb 2020
    date_iso: '2020-02-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.852
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: mIoU
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - mIoU
  metric: mIoU
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: ShapeNet-Part
      dataset_slug: shapenet-part
---

