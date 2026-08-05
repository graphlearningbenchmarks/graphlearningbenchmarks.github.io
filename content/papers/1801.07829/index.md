---
title: Dynamic Graph CNN for Learning on Point Clouds
arxiv_id: '1801.07829'
source_url: ''
authors:
- name: Yue Wang
  orcid: null
  s2_author_id: '2118462083'
  s2_url: null
- name: Yongbin Sun
  orcid: null
  s2_author_id: '1409692637'
  s2_url: null
- name: Ziwei Liu
  orcid: null
  s2_author_id: '2117940996'
  s2_url: null
- name: Sanjay E. Sarma
  orcid: null
  s2_author_id: '1934849'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '1732570'
  s2_url: null
- name: Justin M. Solomon
  orcid: null
  s2_author_id: '1932072'
  s2_url: null
published_date: Jan 24, 2018
published_date_iso: '2018-01-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Point clouds provide a flexible geometric representation suitable for countless
  applications in computer graphics; they also comprise the raw output of most 3D
  data acquisition devices. While hand-designed features on point clouds have long
  been proposed in graphics and vision, however, the recent overwhelming success of
  convolutional neural networks (CNNs) for image analysis suggests the value of adapting
  insight from CNN to the point cloud world. Point clouds inherently lack topological
  information so designing a model to recover topology can enrich the representation
  power of point clouds. To this end, we propose a new neural network module dubbed
  EdgeConv suitable for CNN-based high-level tasks on point clouds including classification
  and segmentation. EdgeConv acts on graphs dynamically computed in each layer of
  the network. It is differentiable and can be plugged into existing architectures.
  Compared to existing modules operating in extrinsic space or treating each point
  independently, EdgeConv has several appealing properties: It incorporates local
  neighborhood information; it can be stacked applied to learn global shape properties;
  and in multi-layer systems affinity in feature space captures semantic characteristics
  over potentially long distances in the original embedding. We show the performance
  of our model on standard benchmarks including ModelNet40, ShapeNetPart, and S3DIS.'
codebase_url: https://github.com/WangYueFt/dgcnn
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DGCNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ShapeNet-Part
  rows:
  - model: PointCNN
    model_key: pointcnn
    model_plain: PointCNN
    value: 0.861
    std: null
    paper_value: 0.861
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.861
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.861
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
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.852
    std: null
    paper_value: 0.852
    paper_std: null
    metric: mIoU
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.852
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.852
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
  - model: PointNet++
    model_key: pointnet++
    model_plain: PointNet++
    value: 0.851
    std: null
    paper_value: 0.851
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.851
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.851
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
  - model: PCNN
    model_key: pcnn
    model_plain: PCNN
    value: 0.851
    std: null
    paper_value: 0.851
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.851
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.851
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
  - model: LocalFeatureNet
    model_key: localfeaturenet
    model_plain: LocalFeatureNet
    value: 0.843
    std: null
    paper_value: 0.843
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.843
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.843
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
  - model: Kd-Net
    model_key: kd-net
    model_plain: Kd-Net
    value: 0.823
    std: null
    paper_value: 0.823
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: mIoU on ShapeNet-Part test set
    date: Jan 24, 2018
    date_display: Jan 2018
    date_iso: '2018-01-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-01-24'
    value_gap_source_date_label: '2018'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.823
    true_std: null
    value_gap_source_arxiv: '1801.07829'
    value_gap_source_title: Dynamic Graph CNN for Learning on Point Clouds
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.823
    sort_std: null
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
single_proposed_model: DGCNN
main_figure: /figures/1801.07829/main_figure.jpegoptim.jpg
---

