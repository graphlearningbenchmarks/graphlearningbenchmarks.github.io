---
title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node Classification'
arxiv_id: '2605.20248'
source_url: ''
authors:
- name: Brown Zaz
  orcid: null
  s2_author_id: '2292199135'
  s2_url: null
- name: M. Catala
  orcid: null
  s2_author_id: '2287757766'
  s2_url: null
- name: Ferran Hernandez Caralt
  orcid: null
  s2_author_id: '2313728813'
  s2_url: null
- name: Moshe Eliasof
  orcid: null
  s2_author_id: '104172497'
  s2_url: null
- name: Pietro Liò
  orcid: null
  s2_author_id: '2313728673'
  s2_url: null
published_date: May 18, 2026
published_date_iso: '2026-05-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'In the transductive setting, where the full graph is observed but node
  labels are only partially available, progress in semi-supervised node classification
  has largely focused on architectural innovation. In this paper, we revisit an orthogonal
  axis: the training objective. We start from a simple observation: transductive models
  produce predictions for every node during training, including nodes without labels.
  These unlabeled-node predictions may contain useful training signal, but standard
  supervised objectives discard them because no ground-truth labels are available.
  Inspired by the decomposition of cross-entropy into a label-dependent alignment
  term and a label-independent entropy term, we propose prediction confidence as a
  natural way to extract this signal in the absence of labels. This motivates Transductive
  Sharpening (TS): a loss-level modification that minimizes prediction entropy on
  unlabeled nodes while counterbalancing this effect on labeled nodes. We evaluate
  Transductive Sharpening across a wide range of node-classification benchmarks and
  observe consistent performance improvements without requiring any changes to the
  backbone architecture. Code is available at.'
codebase_url: https://github.com/transductive-sharpening/tunedGNN
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Heterophilic Graphs
- Heterophily Benchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 6
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 3
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
    paper_value: 0.9461
    paper_std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9461
    true_std: 0.0017
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9461
    sort_std: 0.0017
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9412
    std: 0.0008
    paper_value: 0.9412
    paper_std: 0.0008
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
    source_ref: kipf2017semisupervisedclassificationgraphconvolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.916
    at_pub_std: 0.016
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0252
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9398
    std: 0.0022
    paper_value: 0.9398
    paper_std: 0.0022
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
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.924
    at_pub_std: 0.013
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.015799999999999925
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.9398
    std: 0.0026
    paper_value: 0.9398
    paper_std: 0.0026
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9398
    true_std: 0.0026
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0026
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
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.9386
    std: 0.0013
    paper_value: 0.9386
    paper_std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9386
    true_std: 0.0013
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9386
    sort_std: 0.0013
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
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9378
    std: 0.001
    paper_value: 0.9378
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9318
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9378
    true_std: 0.001
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9378
    sort_std: 0.001
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9351
    std: 0.0006
    paper_value: 0.9351
    paper_std: 0.0006
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9052
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2405.19779'
    at_pub_source_title: Automatic Graph Topology-Aware Transformer
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.029900000000000038
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9351
    true_std: 0.0006
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9351
    sort_std: 0.0006
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Automatic Graph Topology-Aware Transformer
    comparison_source_arxiv: '2405.19779'
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.9343
    std: 0.0011
    paper_value: 0.9343
    paper_std: 0.0011
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9343
    true_std: 0.0011
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9343
    sort_std: 0.0011
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
  - model: OGFormer
    model_key: ogformer
    model_plain: OGFormer
    value: 0.929
    std: 0.003
    paper_value: 0.929
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: ogformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.929
    true_std: 0.003
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.929
    sort_std: 0.003
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9242
    std: 0.0066
    paper_value: 0.9242
    paper_std: 0.0066
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9075
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.016700000000000048
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9242
    true_std: 0.0066
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9242
    sort_std: 0.0066
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    comparison_source_arxiv: '2602.19622'
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.9229
    std: 0.0037
    paper_value: 0.9229
    paper_std: 0.0037
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9096
    at_pub_std: 0.009
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.01330000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9229
    true_std: 0.0037
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0037
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.918
    std: 0.0035
    paper_value: 0.918
    paper_std: 0.0035
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.916
    at_pub_std: 0.003
    at_pub_source_arxiv: '2412.06173'
    at_pub_source_title: Revisiting the Necessity of Graph Learning and Common Graph
      Benchmarks
    at_pub_source_date_iso: '2024-12-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.918
    true_std: 0.0035
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.0035
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.9179
    std: 0.0063
    paper_value: 0.9179
    paper_std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9119
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9179
    true_std: 0.0063
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9179
    sort_std: 0.0063
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.9169
    std: 0.003
    paper_value: 0.9169
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9122
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2310.05296'
    at_pub_source_title: Tailoring Self-Attention for Graph via Rooted Subtrees
    at_pub_source_date_iso: '2023-10-08'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0047000000000000375
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9169
    true_std: 0.003
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9169
    sort_std: 0.003
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Tailoring Self-Attention for Graph via Rooted Subtrees
    comparison_source_arxiv: '2310.05296'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.912
    std: 0.0029
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.08798'
    title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
    date: Dec 9, 2025
    date_display: Dec 2025
    date_iso: '2025-12-09'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 64
    sort_value: 0.912
    sort_std: 0.0029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8729
    std: 0.0058
    paper_value: 0.8729
    paper_std: 0.0058
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9112
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0383
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9112
    true_std: 0.0019
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0383
    has_value_note: false
    value_note: ''
    sort_value: 0.9112
    sort_std: 0.0019
    global_rank: 67
    paper_rank: 288
    rank_delta: 221
    rank_delta_abs: 221
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8246
    std: 0.0045
    paper_value: 0.8246
    paper_std: 0.0045
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8463
    at_pub_std: null
    at_pub_source_arxiv: '2407.11907'
    at_pub_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    at_pub_source_date_iso: '2024-07-16'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.021700000000000053
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8463
    true_std: null
    value_gap_source_arxiv: '2407.11907'
    value_gap_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    value_gap_source_is_current_paper: false
    value_gap: 0.021700000000000053
    has_value_note: false
    value_note: ''
    sort_value: 0.8463
    sort_std: null
    global_rank: 365
    paper_rank: 440
    rank_delta: 75
    rank_delta_abs: 75
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphFM: A generalist graph transformer that learns
      transferable representations across diverse domains'
    comparison_source_arxiv: '2407.11907'
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.8287
    std: 0.0056
    paper_value: 0.8287
    paper_std: 0.0056
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for the Computer dataset.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8287
    true_std: 0.0056
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8287
    sort_std: 0.0056
    global_rank: 436
    paper_rank: 436
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
- &id003
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    paper_value: 0.9703
    paper_std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9703
    at_pub_std: null
    at_pub_source_arxiv: '2510.10631'
    at_pub_source_title: 'GraphTARIF: Linear Graph Transformer with Augmented Rank
      and Improved Focus'
    at_pub_source_date_iso: '2025-10-12'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9703
    true_std: 0.0019
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9703
    sort_std: 0.0019
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9669
    std: 0.0014
    paper_value: 0.9669
    paper_std: 0.0014
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
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9498
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.017100000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.966
    std: 0.0007
    paper_value: 0.966
    paper_std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: TS-augmented GAT
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.0007
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
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9657
    std: 0.0023
    paper_value: 0.9657
    paper_std: 0.0023
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9611
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0046000000000000485
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9657
    true_std: 0.0023
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9657
    sort_std: 0.0023
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.9651
    std: 0.0023
    paper_value: 0.9651
    paper_std: 0.0023
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: TS-augmented SAGE
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9651
    true_std: 0.0023
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9651
    sort_std: 0.0023
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
    paper_value: 0.9643
    paper_std: 0.0027
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
    source_ref: hamilton2018inductiverepresentationlearninglarge
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9403
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02400000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9643
    true_std: 0.0027
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9643
    sort_std: 0.0027
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    comparison_source_arxiv: '2602.19622'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9632
    std: 0.0008
    paper_value: 0.9632
    paper_std: 0.0008
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for TS-augmented GCN at lambda=0.25
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9476
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.015599999999999947
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.9621
    std: 0.0011
    paper_value: 0.9621
    paper_std: 0.0011
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: TS-augmented GCN
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9621
    true_std: 0.0011
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9621
    sort_std: 0.0011
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
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.9614
    std: 0.0016
    paper_value: 0.9614
    paper_std: 0.0016
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9594
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9614
    true_std: 0.0016
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9614
    sort_std: 0.0016
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9569
    std: 0.0039
    paper_value: 0.9569
    paper_std: 0.0039
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9536
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2411.16278'
    at_pub_source_title: Even Sparser Graph Transformers
    at_pub_source_date_iso: '2024-11-25'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0032999999999999696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9569
    true_std: 0.0039
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9569
    sort_std: 0.0039
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9558
    std: 0.0036
    paper_value: 0.9558
    paper_std: 0.0036
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9481
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007699999999999929
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9558
    true_std: 0.0036
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9558
    sort_std: 0.0036
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OGFormer
    model_key: ogformer
    model_plain: OGFormer
    value: 0.955
    std: 0.0
    paper_value: 0.955
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: ogformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.955
    true_std: 0.0
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.955
    sort_std: 0.0
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.9343
    std: 0.0056
    paper_value: 0.9343
    paper_std: 0.0056
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9527
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.018399999999999972
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9527
    true_std: 0.0017
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.018399999999999972
    has_value_note: false
    value_note: ''
    sort_value: 0.9527
    sort_std: 0.0017
    global_rank: 51
    paper_rank: 184
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9508
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 68
    sort_value: 0.9508
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.9489
    std: 0.0014
    paper_value: 0.9489
    paper_std: 0.0014
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9506
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2310.05296'
    at_pub_source_title: Tailoring Self-Attention for Graph via Rooted Subtrees
    at_pub_source_date_iso: '2023-10-08'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-12-09'
    value_gap_source_date_label: LoG 2025
    gap_vs_at_pub: 0.0017000000000000348
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9506
    true_std: 0.0013
    value_gap_source_arxiv: '2512.08798'
    value_gap_source_title: Can TabPFN Compete with GNNs for Node Classification via
      Graph Tabularization?
    value_gap_source_is_current_paper: false
    value_gap: 0.0017000000000000348
    has_value_note: false
    value_note: ''
    sort_value: 0.9506
    sort_std: 0.0013
    global_rank: 69
    paper_rank: 80
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.9433
    std: 0.0021
    paper_value: 0.9433
    paper_std: 0.0021
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9296
    at_pub_std: 0.0148
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.013700000000000045
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9433
    true_std: 0.0021
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9433
    sort_std: 0.0021
    global_rank: 111
    paper_rank: 111
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8757
    std: 0.0052
    paper_value: 0.8757
    paper_std: 0.0052
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification on Photo
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9128
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03709999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.03709999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0063
    global_rank: 426
    paper_rank: 543
    rank_delta: 117
    rank_delta_abs: 117
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.8765
    std: 0.0022
    paper_value: 0.8765
    paper_std: 0.0022
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: TS-augmented MLP
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8765
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8765
    sort_std: 0.0022
    global_rank: 541
    paper_rank: 541
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
- &id010
  dataset: Amazon-ratings
  rows:
  - model: UniGAP
    model_key: unigap
    model_plain: UniGAP
    value: 0.6375
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6375
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN + HalfHop
    model_key: h2gcn + halfhop
    model_plain: H2GCN + HalfHop
    value: 0.5961
    std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.5961
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE + HalfHop
    model_key: graphsage + halfhop
    model_plain: GraphSAGE + HalfHop
    value: 0.5897
    std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5897
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.3647
    std: 0.0023
    paper_value: 0.3647
    paper_std: 0.0023
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
    source_ref: h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5681
    at_pub_std: 0.009
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.20340000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5681
    true_std: 0.009
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.20340000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5681
    sort_std: 0.009
    global_rank: 7
    paper_rank: 210
    rank_delta: 203
    rank_delta_abs: 203
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.5672
    std: 0.0035
    paper_value: 0.5672
    paper_std: 0.0035
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5672
    true_std: 0.0035
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5672
    sort_std: 0.0035
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.5586
    std: 0.0042
    paper_value: 0.5586
    paper_std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5586
    true_std: 0.0042
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5586
    sort_std: 0.0042
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
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.5573
    std: 0.0031
    paper_value: 0.5573
    paper_std: 0.0031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5573
    true_std: 0.0031
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5573
    sort_std: 0.0031
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.5569
    std: 0.0023
    paper_value: 0.5569
    paper_std: 0.0023
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5363
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02059999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5569
    true_std: 0.0023
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5569
    sort_std: 0.0023
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5559
    std: 0.0027
    paper_value: 0.5559
    paper_std: 0.0027
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.527
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2510.21267'
    at_pub_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    at_pub_source_date_iso: '2025-10-24'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.028899999999999926
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5559
    true_std: 0.0027
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5559
    sort_std: 0.0027
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    comparison_source_arxiv: '2510.21267'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.554
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
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 15
    sort_value: 0.554
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.5496
    std: 0.0022
    paper_value: 0.5496
    paper_std: 0.0022
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5471
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2510.21267'
    at_pub_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    at_pub_source_date_iso: '2025-10-24'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0024999999999999467
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5496
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5496
    sort_std: 0.0022
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.5414
    std: 0.0062
    paper_value: 0.5414
    paper_std: 0.0062
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5238
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2510.21267'
    at_pub_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    at_pub_source_date_iso: '2025-10-24'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.01759999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5414
    true_std: 0.0062
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5414
    sort_std: 0.0062
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    comparison_source_arxiv: '2510.21267'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5411
    std: 0.0034
    paper_value: 0.5411
    paper_std: 0.0034
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=83)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.538
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0030999999999999917
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5411
    true_std: 0.0034
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5411
    sort_std: 0.0034
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.5406
    std: 0.0058
    paper_value: 0.5406
    paper_std: 0.0058
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5406
    true_std: 0.0058
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5406
    sort_std: 0.0058
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.5374
    std: 0.0051
    paper_value: 0.5374
    paper_std: 0.0051
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: bunn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5374
    at_pub_std: 0.0051
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5374
    true_std: 0.0051
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5374
    sort_std: 0.0051
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.5327
    std: 0.0066
    paper_value: 0.5327
    paper_std: 0.0066
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.531
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0016999999999999238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5327
    true_std: 0.0066
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5327
    sort_std: 0.0066
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+ReP
    model_key: gcn+rep
    model_plain: GCN+ReP
    value: 0.5275
    std: 0.0062
    paper_value: 0.5275
    paper_std: 0.0062
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
    source_ref: gcn-rep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5275
    true_std: 0.0062
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5275
    sort_std: 0.0062
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.5274
    std: 0.0083
    paper_value: 0.5274
    paper_std: 0.0083
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
    source_ref: fsgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5274
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5274
    true_std: 0.0083
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5274
    sort_std: 0.0083
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    value: 0.5073
    std: 0.0056
    paper_value: 0.5073
    paper_std: 0.0056
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
    source_ref: dir-poly
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5073
    true_std: 0.0056
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5073
    sort_std: 0.0056
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4885
    std: 0.0055
    paper_value: 0.4885
    paper_std: 0.0055
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5058
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.017300000000000038
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5058
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.017300000000000038
    has_value_note: false
    value_note: ''
    sort_value: 0.5058
    sort_std: null
    global_rank: 85
    paper_rank: 111
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.3689
    std: 0.0014
    paper_value: 0.3689
    paper_std: 0.0014
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
    source_ref: glognn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4988
    at_pub_std: 0.004
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12990000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4988
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.12990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4988
    sort_std: 0.004
    global_rank: 96
    paper_rank: 210
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.4488
    std: 0.0034
    paper_value: 0.4488
    paper_std: 0.0034
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
    source_ref: gprgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4956
    at_pub_std: 0.004
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.04680000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4956
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.04680000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.4956
    sort_std: 0.004
    global_rank: 101
    paper_rank: 157
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.495
    std: 0.0027
    paper_value: 0.495
    paper_std: 0.0027
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.495
    true_std: 0.0027
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.495
    sort_std: 0.0027
    global_rank: 103
    paper_rank: 103
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.4379
    std: 0.0057
    paper_value: 0.4379
    paper_std: 0.0057
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4548
    at_pub_std: 0.005
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01689999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4548
    true_std: 0.005
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.01689999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4548
    sort_std: 0.005
    global_rank: 151
    paper_rank: 171
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.3979
    std: 0.0077
    paper_value: 0.3979
    paper_std: 0.0077
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
    source_ref: cpgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4436
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.04570000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4436
    true_std: 0.0035
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04570000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4436
    sort_std: 0.0035
    global_rank: 162
    paper_rank: 203
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
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
- &id007
  dataset: Chameleon
  rows:
  - model: Hetero-S (GAT 8-layer)
    model_key: hetero-s (gat 8-layer)
    model_plain: Hetero-S (GAT 8-layer)
    value: 0.8693
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8693
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.8586
    std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8586
    sort_std: 0.018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4387
    std: 0.052
    paper_value: 0.4387
    paper_std: 0.052
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.856
    at_pub_std: null
    at_pub_source_arxiv: '2406.12539'
    at_pub_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    at_pub_source_date_iso: '2024-06-18'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-06-18'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.4173
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.856
    true_std: null
    value_gap_source_arxiv: '2406.12539'
    value_gap_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.4173
    has_value_note: false
    value_note: ''
    sort_value: 0.856
    sort_std: null
    global_rank: 3
    paper_rank: 275
    rank_delta: 272
    rank_delta_abs: 272
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'The Heterophilic Snowflake Hypothesis: Training and
      Empowering GNNs for Heterophilic Graphs'
    comparison_source_arxiv: '2406.12539'
    is_best: true
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.4061
    std: 0.0297
    paper_value: 0.4061
    paper_std: 0.0297
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
    source_ref: fsgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7827
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.37659999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7827
    true_std: 0.0128
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.37659999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7827
    sort_std: 0.0128
    global_rank: 25
    paper_rank: 299
    rank_delta: 274
    rank_delta_abs: 274
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.259
    std: 0.0358
    paper_value: 0.259
    paper_std: 0.0358
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
    source_ref: glognn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7133
    at_pub_std: 0.0242
    at_pub_source_arxiv: '2603.09195'
    at_pub_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    at_pub_source_date_iso: '2026-03-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.45430000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7133
    true_std: 0.0242
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.45430000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: 0.0242
    global_rank: 60
    paper_rank: 331
    rank_delta: 271
    rank_delta_abs: 271
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    comparison_source_arxiv: '2603.09195'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.453
    std: 0.023
    paper_value: 0.453
    paper_std: 0.023
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
    source_ref: kipf2017semisupervisedclassificationgraphconvolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7033
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2503
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7033
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2503
    has_value_note: false
    value_note: ''
    sort_value: 0.7033
    sort_std: null
    global_rank: 69
    paper_rank: 270
    rank_delta: 201
    rank_delta_abs: 201
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3993
    std: 0.033
    paper_value: 0.3993
    paper_std: 0.033
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
    source_ref: gprgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6748
    at_pub_std: 0.004
    at_pub_source_arxiv: '2603.09195'
    at_pub_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    at_pub_source_date_iso: '2026-03-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.27549999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6748
    true_std: 0.004
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.27549999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6748
    sort_std: 0.004
    global_rank: 97
    paper_rank: 302
    rank_delta: 205
    rank_delta_abs: 205
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    comparison_source_arxiv: '2603.09195'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.4432
    std: 0.0455
    paper_value: 0.4432
    paper_std: 0.0455
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
    source_ref: hamilton2018inductiverepresentationlearninglarge
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.634
    at_pub_std: 0.03
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.19080000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.634
    true_std: 0.03
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.19080000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.634
    sort_std: 0.03
    global_rank: 136
    paper_rank: 275
    rank_delta: 139
    rank_delta_abs: 139
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6215
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.03930'
    title: Hierarchical Graph Transformer with Adaptive Node Sampling
    date: Oct 8, 2022
    date_display: Oct 2022
    date_iso: '2022-10-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/zaixizhang/ANS-GT
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 145
    sort_value: 0.6215
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.2675
    std: 0.0364
    paper_value: 0.2675
    paper_std: 0.0364
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
    source_ref: h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.603
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2206.14418'
    at_pub_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    at_pub_source_date_iso: '2022-06-29'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-06-29'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.33549999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.603
    true_std: 0.0231
    value_gap_source_arxiv: '2206.14418'
    value_gap_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    value_gap_source_is_current_paper: false
    value_gap: 0.33549999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.0231
    global_rank: 164
    paper_rank: 328
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    comparison_source_arxiv: '2206.14418'
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.4197
    std: 0.0318
    paper_value: 0.4197
    paper_std: 0.0318
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6
    at_pub_std: 0.018
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.18029999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6
    true_std: 0.018
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.18029999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: 0.018
    global_rank: 170
    paper_rank: 293
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.4155
    std: 0.0391
    paper_value: 0.4155
    paper_std: 0.0391
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.562
    at_pub_std: 0.038
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.14650000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.562
    true_std: 0.038
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.14650000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.562
    sort_std: 0.038
    global_rank: 198
    paper_rank: 294
    rank_delta: 96
    rank_delta_abs: 96
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4386
    std: 0.0523
    paper_value: 0.4386
    paper_std: 0.0523
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5429
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.10430000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5429
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10430000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.5429
    sort_std: null
    global_rank: 208
    paper_rank: 275
    rank_delta: 67
    rank_delta_abs: 67
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.4521
    std: 0.0372
    paper_value: 0.4521
    paper_std: 0.0372
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.514
    at_pub_std: 0.017
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06190000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.514
    true_std: 0.017
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.06190000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.514
    sort_std: 0.017
    global_rank: 228
    paper_rank: 271
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
  - model: GCN+ReP
    model_key: gcn+rep
    model_plain: GCN+ReP
    value: 0.4757
    std: 0.039
    paper_value: 0.4757
    paper_std: 0.039
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
    source_ref: gcn-rep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4757
    true_std: 0.039
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4757
    sort_std: 0.039
    global_rank: 259
    paper_rank: 259
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoED
    model_key: coed
    model_plain: CoED
    value: 0.4727
    std: 0.0362
    paper_value: 0.4727
    paper_std: 0.0362
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
    source_ref: coed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4727
    true_std: 0.0362
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4727
    sort_std: 0.0362
    global_rank: 260
    paper_rank: 260
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.4709
    std: 0.0405
    paper_value: 0.4709
    paper_std: 0.0405
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: m3dphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4709
    true_std: 0.0405
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4709
    sort_std: 0.0405
    global_rank: 262
    paper_rank: 262
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.4527
    std: 0.0474
    paper_value: 0.4527
    paper_std: 0.0474
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4527
    true_std: 0.0474
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4527
    sort_std: 0.0474
    global_rank: 271
    paper_rank: 271
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.4452
    std: 0.0369
    paper_value: 0.4452
    paper_std: 0.0369
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4452
    true_std: 0.0369
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4452
    sort_std: 0.0369
    global_rank: 274
    paper_rank: 274
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.4386
    std: 0.0523
    paper_value: 0.4386
    paper_std: 0.0523
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4386
    true_std: 0.0523
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4386
    sort_std: 0.0523
    global_rank: 276
    paper_rank: 276
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.4332
    std: 0.0467
    paper_value: 0.4332
    paper_std: 0.0467
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4332
    true_std: 0.0467
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4332
    sort_std: 0.0467
    global_rank: 283
    paper_rank: 283
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.3638
    std: 0.0385
    paper_value: 0.3638
    paper_std: 0.0385
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3492
    at_pub_std: 0.0408
    at_pub_source_arxiv: '2509.12530'
    at_pub_source_title: 'Graph Homophily Booster: Rethinking the Role of Discrete
      Features on Heterophilic Graphs'
    at_pub_source_date_iso: '2025-09-16'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.014600000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3638
    true_std: 0.0385
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3638
    sort_std: 0.0385
    global_rank: 316
    paper_rank: 316
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.33
    std: 0.0315
    paper_value: 0.33
    paper_std: 0.0315
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
    source_ref: cpgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2 for Chameleon
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.33
    at_pub_std: 0.0315
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.33
    true_std: 0.0315
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.33
    sort_std: 0.0315
    global_rank: 319
    paper_rank: 319
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
- &id005
  dataset: Coauthor-Physics
  rows:
  - model: GrokFormer
    model_key: grokformer
    model_plain: GrokFormer
    value: 0.9831
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9831
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PolyFormer
    model_key: polyformer
    model_plain: PolyFormer
    value: 0.9808
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_display: Nov 2024
    date_iso: '2024-11-26'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/GGA23/GrokFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9808
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9675
    std: 0.0026
    paper_value: 0.9675
    paper_std: 0.0026
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9796
    at_pub_std: 0.0081
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0121
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9796
    true_std: 0.0081
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0121
    has_value_note: false
    value_note: ''
    sort_value: 0.9796
    sort_std: 0.0081
    global_rank: 3
    paper_rank: 46
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: true
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.9735
    std: 0.0012
    paper_value: 0.9735
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9785
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9785
    true_std: 0.0026
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.9785
    sort_std: 0.0026
    global_rank: 5
    paper_rank: 21
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9732
    std: 0.0006
    paper_value: 0.9732
    paper_std: 0.0006
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9782
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9782
    true_std: 0.0028
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.9782
    sort_std: 0.0028
    global_rank: 6
    paper_rank: 22
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9744
    std: 0.0014
    paper_value: 0.9744
    paper_std: 0.0014
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9774
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9774
    true_std: 0.0035
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.9774
    sort_std: 0.0035
    global_rank: 9
    paper_rank: 15
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.9671
    std: 0.0015
    paper_value: 0.9671
    paper_std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.976
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.008900000000000019
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.976
    true_std: 0.0005
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.008900000000000019
    has_value_note: false
    value_note: ''
    sort_value: 0.976
    sort_std: 0.0005
    global_rank: 13
    paper_rank: 48
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.9744
    std: 0.0014
    paper_value: 0.9744
    paper_std: 0.0014
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9744
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0014
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9725
    std: 0.0008
    paper_value: 0.9725
    paper_std: 0.0008
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
    source_ref: hamilton2018inductiverepresentationlearninglarge
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9739
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9739
    true_std: 0.0018
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0013999999999999568
    has_value_note: false
    value_note: ''
    sort_value: 0.9739
    sort_std: 0.0018
    global_rank: 18
    paper_rank: 25
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9739
    std: 0.0007
    paper_value: 0.9739
    paper_std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9739
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9739
    sort_std: 0.0007
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
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.9726
    std: 0.0003
    paper_value: 0.9726
    paper_std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9726
    true_std: 0.0003
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9726
    sort_std: 0.0003
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.9723
    std: 0.0
    paper_value: 0.9723
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9723
    true_std: 0.0
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9723
    sort_std: 0.0
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9718
    std: 0.0011
    paper_value: 0.9718
    paper_std: 0.0011
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9722
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9722
    true_std: 0.0006
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9722
    sort_std: 0.0006
    global_rank: 28
    paper_rank: 30
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9706
    std: 0.0013
    paper_value: 0.9706
    paper_std: 0.0013
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.972
    at_pub_std: 0.001
    at_pub_source_arxiv: '2412.06173'
    at_pub_source_title: Revisiting the Necessity of Graph Learning and Common Graph
      Benchmarks
    at_pub_source_date_iso: '2024-12-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0013999999999999568
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.972
    true_std: 0.001
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: 0.0013999999999999568
    has_value_note: false
    value_note: ''
    sort_value: 0.972
    sort_std: 0.001
    global_rank: 29
    paper_rank: 36
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.9648
    std: 0.0034
    paper_value: 0.9648
    paper_std: 0.0034
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9719
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2505.17660'
    at_pub_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2025-05-23'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.007099999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9719
    true_std: 0.0004
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.007099999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9719
    sort_std: 0.0004
    global_rank: 30
    paper_rank: 57
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    comparison_source_arxiv: '2505.17660'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9649
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.16278'
    title: Even Sparser Graph Transformers
    date: Nov 25, 2024
    date_display: Nov 2024
    date_iso: '2024-11-25'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/hamed1375/Sp_Exphormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 57
    sort_value: 0.9649
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.9647
    std: 0.0016
    paper_value: 0.9647
    paper_std: 0.0016
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9627
    at_pub_std: 0.003
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9647
    true_std: 0.0016
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9647
    sort_std: 0.0016
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.9598
    std: 0.0008
    paper_value: 0.9598
    paper_std: 0.0008
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9598
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9598
    sort_std: 0.0008
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9597
    std: 0.0007
    paper_value: 0.9597
    paper_std: 0.0007
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Physics dataset
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9563
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0033999999999999586
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9597
    true_std: 0.0007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9597
    sort_std: 0.0007
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
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
- &id001
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8516
    std: 0.0036
    paper_value: 0.8516
    paper_std: 0.0036
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.048799999999999955
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.048799999999999955
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 280
    rank_delta: 249
    rank_delta_abs: 249
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8494
    std: 0.0089
    paper_value: 0.8494
    paper_std: 0.0089
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8911
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2506.07168'
    at_pub_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    at_pub_source_date_iso: '2025-06-08'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.04169999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8911
    true_std: 0.0012
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: false
    value_gap: 0.04169999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8911
    sort_std: 0.0012
    global_rank: 61
    paper_rank: 291
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    comparison_source_arxiv: '2506.07168'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.837
    std: 0.0119
    paper_value: 0.837
    paper_std: 0.0119
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8897
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05270000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.05270000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 389
    rank_delta: 322
    rank_delta_abs: 322
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8273
    std: 0.0075
    paper_value: 0.8273
    paper_std: 0.0075
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8848
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.057499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8848
    true_std: 0.0033
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.057499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8848
    sort_std: 0.0033
    global_rank: 97
    paper_rank: 524
    rank_delta: 427
    rank_delta_abs: 427
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    comparison_source_arxiv: '2401.15569'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8777
    std: 0.0183
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.15777'
    title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling Both Homophily
      and Heterophily'
    date: Oct 29, 2021
    date_display: Oct 2021
    date_iso: '2021-10-29'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 146
    sort_value: 0.8777
    sort_std: 0.0183
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OGFormer
    model_key: ogformer
    model_plain: OGFormer
    value: 0.864
    std: 0.003
    paper_value: 0.864
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: ogformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.864
    true_std: 0.003
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: 0.003
    global_rank: 224
    paper_rank: 224
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.8546
    std: 0.0051
    paper_value: 0.8546
    paper_std: 0.0051
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
    source_ref: normprop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8607
    at_pub_std: 0.0
    at_pub_source_arxiv: '2511.19976'
    at_pub_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    at_pub_source_date_iso: '2025-11-25'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8607
    true_std: 0.0
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.006099999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8607
    sort_std: 0.0
    global_rank: 237
    paper_rank: 259
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    comparison_source_arxiv: '2511.19976'
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.8574
    std: 0.0054
    paper_value: 0.8574
    paper_std: 0.0054
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.851
    at_pub_std: null
    at_pub_source_arxiv: '2408.03152'
    at_pub_source_title: 'TSC: A Simple Two-Sided Constraint against Over-Smoothing'
    at_pub_source_date_iso: '2024-08-06'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.006400000000000072
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8574
    true_std: 0.0054
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0054
    global_rank: 248
    paper_rank: 248
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'TSC: A Simple Two-Sided Constraint against Over-Smoothing'
    comparison_source_arxiv: '2408.03152'
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.8528
    std: 0.0111
    paper_value: 0.8528
    paper_std: 0.0111
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8528
    true_std: 0.0111
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8528
    sort_std: 0.0111
    global_rank: 271
    paper_rank: 271
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.8482
    std: 0.0085
    paper_value: 0.8482
    paper_std: 0.0085
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8459
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2604.24293'
    at_pub_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    at_pub_source_date_iso: '2026-04-27'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0022999999999999687
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8482
    true_std: 0.0085
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8482
    sort_std: 0.0085
    global_rank: 298
    paper_rank: 298
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.8462
    std: 0.0089
    paper_value: 0.8462
    paper_std: 0.0089
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8462
    true_std: 0.0089
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8462
    sort_std: 0.0089
    global_rank: 308
    paper_rank: 308
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ELU-GCN
    model_key: elu-gcn
    model_plain: ELU-GCN
    value: 0.8429
    std: 0.0039
    paper_value: 0.8429
    paper_std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: elu-gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8429
    true_std: 0.0039
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8429
    sort_std: 0.0039
    global_rank: 341
    paper_rank: 341
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.8329
    std: 0.0136
    paper_value: 0.8329
    paper_std: 0.0136
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.841
    at_pub_std: 0.008
    at_pub_source_arxiv: '2503.12563'
    at_pub_source_title: 'Diffusion on Graph: Augmentation of Graph Structure for
      Node Classification'
    at_pub_source_date_iso: '2025-03-16'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2025-03-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.008099999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.841
    true_std: 0.008
    value_gap_source_arxiv: '2503.12563'
    value_gap_source_title: 'Diffusion on Graph: Augmentation of Graph Structure for
      Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.008099999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.841
    sort_std: 0.008
    global_rank: 352
    paper_rank: 473
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.8387
    std: 0.0096
    paper_value: 0.8387
    paper_std: 0.0096
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8295
    at_pub_std: 0.0123
    at_pub_source_arxiv: '2604.24293'
    at_pub_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    at_pub_source_date_iso: '2026-04-27'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.009199999999999986
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8387
    true_std: 0.0096
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8387
    sort_std: 0.0096
    global_rank: 379
    paper_rank: 379
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.8343
    std: 0.0089
    paper_value: 0.8343
    paper_std: 0.0089
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8324
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2604.24293'
    at_pub_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    at_pub_source_date_iso: '2026-04-27'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0019000000000000128
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8343
    true_std: 0.0089
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8343
    sort_std: 0.0089
    global_rank: 452
    paper_rank: 452
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8326
    std: 0.0124
    paper_value: 0.8326
    paper_std: 0.0124
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8326
    true_std: 0.0124
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8326
    sort_std: 0.0124
    global_rank: 474
    paper_rank: 474
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.8092
    std: 0.0117
    paper_value: 0.8092
    paper_std: 0.0117
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8213
    at_pub_std: 0.0118
    at_pub_source_arxiv: '2510.04522'
    at_pub_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    at_pub_source_date_iso: '2025-10-06'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-10-06'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.0121
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8213
    true_std: 0.0118
    value_gap_source_arxiv: '2510.04522'
    value_gap_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.0121
    has_value_note: false
    value_note: ''
    sort_value: 0.8213
    sort_std: 0.0118
    global_rank: 597
    paper_rank: 700
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6096
    std: 0.0251
    paper_value: 0.6096
    paper_std: 0.0251
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.16720000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.16720000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 956
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.6448
    std: 0.0283
    paper_value: 0.6448
    paper_std: 0.0283
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for Cora
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6448
    true_std: 0.0283
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6448
    sort_std: 0.0283
    global_rank: 949
    paper_rank: 949
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
- &id011
  dataset: Minesweeper
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9903
    std: 0.0019
    paper_value: 0.9903
    paper_std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9903
    true_std: 0.0019
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9903
    sort_std: 0.0019
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
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9899
    std: 0.0016
    paper_value: 0.9899
    paper_std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: bunn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9899
    true_std: 0.0016
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9899
    sort_std: 0.0016
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
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.9827
    std: 0.002
    paper_value: 0.9827
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: m3dphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9827
    true_std: 0.002
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9827
    sort_std: 0.002
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9786
    std: 0.0037
    paper_value: 0.9786
    paper_std: 0.0037
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
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9201
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.058499999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9786
    true_std: 0.0037
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9786
    sort_std: 0.0037
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.9786
    std: 0.0037
    paper_value: 0.9786
    paper_std: 0.0037
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9786
    true_std: 0.0037
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9786
    sort_std: 0.0037
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
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.978
    std: 0.002
    paper_value: 0.978
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.978
    true_std: 0.002
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.978
    sort_std: 0.002
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9749
    std: 0.0048
    paper_value: 0.9749
    paper_std: 0.0048
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9746
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2604.08980'
    at_pub_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    at_pub_source_date_iso: '2026-04-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9749
    true_std: 0.0048
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9749
    sort_std: 0.0048
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9744
    std: 0.0017
    paper_value: 0.9744
    paper_std: 0.0017
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8975
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.07690000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9744
    true_std: 0.0017
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0017
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.9733
    std: 0.0094
    paper_value: 0.9733
    paper_std: 0.0094
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9733
    true_std: 0.0094
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9733
    sort_std: 0.0094
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9709
    std: 0.01
    paper_value: 0.9709
    paper_std: 0.01
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
    source_ref: hamilton2018inductiverepresentationlearninglarge
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9351
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03579999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9709
    true_std: 0.01
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9709
    sort_std: 0.01
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    comparison_source_arxiv: '2507.14484'
    is_best: false
    is_std_outlier: false
  - model: GCN+ReP
    model_key: gcn+rep
    model_plain: GCN+ReP
    value: 0.9605
    std: 0.0019
    paper_value: 0.9605
    paper_std: 0.0019
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
    source_ref: gcn-rep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9605
    true_std: 0.0019
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9605
    sort_std: 0.0019
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    value: 0.9374
    std: 0.007
    paper_value: 0.9374
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
    table_ref: Table 2
    source_ref: dir-poly
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9374
    true_std: 0.007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9374
    sort_std: 0.007
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.9075
    std: 0.0089
    paper_value: 0.9075
    paper_std: 0.0089
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9229
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.01540000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9229
    true_std: 0.0061
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.01540000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0061
    global_rank: 20
    paper_rank: 26
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.9142
    std: 0.0041
    paper_value: 0.9142
    paper_std: 0.0041
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9142
    true_std: 0.0041
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9142
    sort_std: 0.0041
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.9008
    std: 0.007
    paper_value: 0.9008
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
    table_ref: Table 2
    source_ref: fsgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9008
    at_pub_std: 0.007
    at_pub_source_arxiv: '2603.26178'
    at_pub_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    at_pub_source_date_iso: '2026-03-27'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9008
    true_std: 0.007
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9008
    sort_std: 0.007
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8971
    std: 0.0031
    paper_value: 0.8971
    paper_std: 0.0031
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
    source_ref: h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8971
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2603.26178'
    at_pub_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    at_pub_source_date_iso: '2026-03-27'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8971
    true_std: 0.0031
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8971
    sort_std: 0.0031
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8771
    std: 0.0069
    paper_value: 0.8771
    paper_std: 0.0069
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8671
    at_pub_std: 0.0088
    at_pub_source_arxiv: '2604.08980'
    at_pub_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    at_pub_source_date_iso: '2026-04-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8771
    true_std: 0.0069
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8771
    sort_std: 0.0069
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.8624
    std: 0.0061
    paper_value: 0.8624
    paper_std: 0.0061
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
    source_ref: gprgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8624
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8624
    true_std: 0.0061
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8624
    sort_std: 0.0061
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5106
    std: 0.0176
    paper_value: 0.5106
    paper_std: 0.0176
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: 0.0
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.2894
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: false
    value_gap: 0.2894
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.0
    global_rank: 49
    paper_rank: 64
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HyperAggregation: Aggregating over Graph Edges with
      Hypernetworks'
    comparison_source_arxiv: '2407.11596'
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.5203
    std: 0.0546
    paper_value: 0.5203
    paper_std: 0.0546
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
    source_ref: cpgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5203
    at_pub_std: 0.0546
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5203
    true_std: 0.0546
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5203
    sort_std: 0.0546
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.5108
    std: 0.0123
    paper_value: 0.5108
    paper_std: 0.0123
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
    source_ref: glognn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5108
    at_pub_std: 0.0123
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5108
    true_std: 0.0123
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5108
    sort_std: 0.0123
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.5097
    std: 0.0156
    paper_value: 0.5097
    paper_std: 0.0156
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5097
    true_std: 0.0156
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5097
    sort_std: 0.0156
    global_rank: 65
    paper_rank: 65
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7959
    std: 0.0092
    paper_value: 0.7959
    paper_std: 0.0092
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.949
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1530999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: 0.0019
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.1530999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0019
    global_rank: 7
    paper_rank: 552
    rank_delta: 545
    rank_delta_abs: 545
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8088
    std: 0.0031
    paper_value: 0.8088
    paper_std: 0.0031
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9296
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.12080000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: 0.0015
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.12080000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 430
    rank_delta: 411
    rank_delta_abs: 411
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.798
    std: 0.0093
    paper_value: 0.798
    paper_std: 0.0093
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9233
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.12529999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: 0.0018
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.12529999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 525
    rank_delta: 502
    rank_delta_abs: 502
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.8014
    std: 0.0106
    paper_value: 0.8014
    paper_std: 0.0106
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9176
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2510.04522'
    at_pub_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    at_pub_source_date_iso: '2025-10-06'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-10-06'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.11619999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9176
    true_std: 0.0049
    value_gap_source_arxiv: '2510.04522'
    value_gap_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.11619999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9176
    sort_std: 0.0049
    global_rank: 26
    paper_rank: 489
    rank_delta: 463
    rank_delta_abs: 463
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Toward a Unified Geometry Understanding: Riemannian
      Diffusion Framework for Graph Generation and Prediction'
    comparison_source_arxiv: '2510.04522'
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.7967
    std: 0.0073
    paper_value: 0.7967
    paper_std: 0.0073
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9144
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2510.04522'
    at_pub_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    at_pub_source_date_iso: '2025-10-06'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-10-06'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.11770000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9144
    true_std: 0.0059
    value_gap_source_arxiv: '2510.04522'
    value_gap_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.11770000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9144
    sort_std: 0.0059
    global_rank: 34
    paper_rank: 534
    rank_delta: 500
    rank_delta_abs: 500
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Toward a Unified Geometry Understanding: Riemannian
      Diffusion Framework for Graph Generation and Prediction'
    comparison_source_arxiv: '2510.04522'
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.7935
    std: 0.0073
    paper_value: 0.7935
    paper_std: 0.0073
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9044
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.1109
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9044
    true_std: 0.0021
    value_gap_source_arxiv: '2602.19622'
    value_gap_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.1109
    has_value_note: false
    value_note: ''
    sort_value: 0.9044
    sort_std: 0.0021
    global_rank: 63
    paper_rank: 594
    rank_delta: 531
    rank_delta_abs: 531
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    comparison_source_arxiv: '2602.19622'
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.806
    std: 0.0049
    paper_value: 0.806
    paper_std: 0.0049
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9037
    at_pub_std: 0.002
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.0976999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9037
    true_std: 0.002
    value_gap_source_arxiv: '2602.19622'
    value_gap_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.0976999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9037
    sort_std: 0.002
    global_rank: 65
    paper_rank: 448
    rank_delta: 383
    rank_delta_abs: 383
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    comparison_source_arxiv: '2602.19622'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.7994
    std: 0.0026
    paper_value: 0.7994
    paper_std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9028
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2510.04522'
    at_pub_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    at_pub_source_date_iso: '2025-10-06'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-10-06'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.10340000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9028
    true_std: 0.0062
    value_gap_source_arxiv: '2510.04522'
    value_gap_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.10340000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9028
    sort_std: 0.0062
    global_rank: 72
    paper_rank: 509
    rank_delta: 437
    rank_delta_abs: 437
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Toward a Unified Geometry Understanding: Riemannian
      Diffusion Framework for Graph Generation and Prediction'
    comparison_source_arxiv: '2510.04522'
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8006
    std: 0.0067
    paper_value: 0.8006
    paper_std: 0.0067
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8915
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2602.19622'
    at_pub_source_title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer
      with Graph Token Attention'
    at_pub_source_date_iso: '2026-02-23'
    at_pub_source_date_label: WWW 2026
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: WWW 2026
    gap_vs_at_pub: 0.09089999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8915
    true_std: 0.0039
    value_gap_source_arxiv: '2602.19622'
    value_gap_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.09089999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8915
    sort_std: 0.0039
    global_rank: 120
    paper_rank: 497
    rank_delta: 377
    rank_delta_abs: 377
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'VecFormer: Towards Efficient and Generalizable Graph
      Transformer with Graph Token Attention'
    comparison_source_arxiv: '2602.19622'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.784
    std: 0.0112
    paper_value: 0.784
    paper_std: 0.0112
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8881
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2506.07168'
    at_pub_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    at_pub_source_date_iso: '2025-06-08'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2025-06-08'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.10409999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8881
    true_std: 0.0015
    value_gap_source_arxiv: '2506.07168'
    value_gap_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    value_gap_source_is_current_paper: false
    value_gap: 0.10409999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8881
    sort_std: 0.0015
    global_rank: 134
    paper_rank: 711
    rank_delta: 577
    rank_delta_abs: 577
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Text-Attributed Graph Learning through Selective
      Annotation and Graph Alignment
    comparison_source_arxiv: '2506.07168'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8864
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
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_display: Oct 2023
    date_iso: '2023-10-11'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/seonghyun26/nba-gnn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 144
    sort_value: 0.8864
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6896
    std: 0.0116
    paper_value: 0.6896
    paper_std: 0.0116
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.1794
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.1794
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 931
    rank_delta: 688
    rank_delta_abs: 688
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.8072
    std: 0.0109
    paper_value: 0.8072
    paper_std: 0.0109
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
    source_ref: normprop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8153
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2511.19976'
    at_pub_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    at_pub_source_date_iso: '2025-11-25'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.008099999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8153
    true_std: 0.0001
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.008099999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8153
    sort_std: 0.0001
    global_rank: 390
    paper_rank: 443
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OGFormer
    model_key: ogformer
    model_plain: OGFormer
    value: 0.815
    std: 0.005
    paper_value: 0.815
    paper_std: 0.005
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: ogformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.815
    true_std: 0.005
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.815
    sort_std: 0.005
    global_rank: 395
    paper_rank: 395
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.8074
    std: 0.003
    paper_value: 0.8074
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.807
    at_pub_std: null
    at_pub_source_arxiv: '2408.03152'
    at_pub_source_title: 'TSC: A Simple Two-Sided Constraint against Over-Smoothing'
    at_pub_source_date_iso: '2024-08-06'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8074
    true_std: 0.003
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8074
    sort_std: 0.003
    global_rank: 442
    paper_rank: 442
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ELU-GCN
    model_key: elu-gcn
    model_plain: ELU-GCN
    value: 0.8051
    std: 0.0021
    paper_value: 0.8051
    paper_std: 0.0021
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: elu-gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8051
    true_std: 0.0021
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8051
    sort_std: 0.0021
    global_rank: 453
    paper_rank: 453
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.7972
    std: 0.0069
    paper_value: 0.7972
    paper_std: 0.0069
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7972
    true_std: 0.0069
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7972
    sort_std: 0.0069
    global_rank: 533
    paper_rank: 533
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.7884
    std: 0.0067
    paper_value: 0.7884
    paper_std: 0.0067
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7884
    true_std: 0.0067
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7884
    sort_std: 0.0067
    global_rank: 671
    paper_rank: 671
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.723
    std: 0.0189
    paper_value: 0.723
    paper_std: 0.0189
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.723
    true_std: 0.0189
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.0189
    global_rank: 905
    paper_rank: 905
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
- &id009
  dataset: Roman-empire
  rows:
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    value: 0.9451
    std: 0.0022
    paper_value: 0.9451
    paper_std: 0.0022
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
    source_ref: dir-poly
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9451
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9451
    sort_std: 0.0022
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
  - model: D-CDE
    model_key: d-cde
    model_plain: D-CDE
    value: 0.9387
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_display: Nov 2024
    date_iso: '2024-11-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9387
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeScaleNet
    model_key: largescalenet
    model_plain: LargeScaleNet
    value: 0.9358
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_display: Nov 2024
    date_iso: '2024-11-28'
    venue: null
    codebase_url: https://github.com/Qin87/ScaleNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9358
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9323
    std: 0.0038
    paper_value: 0.9323
    paper_std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9323
    true_std: 0.0038
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9323
    sort_std: 0.0038
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
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.9266
    std: 0.006
    paper_value: 0.9266
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9255
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2505.17939'
    at_pub_source_title: Directed Semi-Simplicial Learning with Applications to Brain
      Activity Decoding
    at_pub_source_date_iso: '2025-05-23'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0010999999999999899
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9266
    true_std: 0.006
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9266
    sort_std: 0.006
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoED
    model_key: coed
    model_plain: CoED
    value: 0.9217
    std: 0.0029
    paper_value: 0.9217
    paper_std: 0.0029
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
    source_ref: coed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9217
    true_std: 0.0029
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9217
    sort_std: 0.0029
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9175
    std: 0.0039
    paper_value: 0.9175
    paper_std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: bunn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9175
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9175
    true_std: 0.0039
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9175
    sort_std: 0.0039
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.9166
    std: 0.002
    paper_value: 0.9166
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9166
    true_std: 0.002
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9166
    sort_std: 0.002
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.9127
    std: 0.0036
    paper_value: 0.9127
    paper_std: 0.0036
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9127
    true_std: 0.0036
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9127
    sort_std: 0.0036
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9106
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.17939'
    title: Directed Semi-Simplicial Learning with Applications to Brain Activity Decoding
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: https://github.com/ManuelLecha/ssn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 24
    sort_value: 0.9106
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.9093
    std: 0.002
    paper_value: 0.9093
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9093
    true_std: 0.002
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9093
    sort_std: 0.002
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+ReP
    model_key: gcn+rep
    model_plain: GCN+ReP
    value: 0.8643
    std: 0.0074
    paper_value: 0.8643
    paper_std: 0.0074
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
    source_ref: gcn-rep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8643
    true_std: 0.0074
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8643
    sort_std: 0.0074
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.5569
    std: 0.0023
    paper_value: 0.5569
    paper_std: 0.0023
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
    variant_inference_reason: 'dataset: fuzzy match to roman-empire (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8574
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.3005000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8574
    true_std: 0.0067
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.3005000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0067
    global_rank: 64
    paper_rank: 185
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5411
    std: 0.0034
    paper_value: 0.5411
    paper_std: 0.0034
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
    variant_inference_reason: 'dataset: fuzzy match to roman-empire (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8272
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2861
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8272
    true_std: 0.0082
    value_gap_source_arxiv: '2407.11596'
    value_gap_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    value_gap_source_is_current_paper: false
    value_gap: 0.2861
    has_value_note: false
    value_note: ''
    sort_value: 0.8272
    sort_std: 0.0082
    global_rank: 75
    paper_rank: 186
    rank_delta: 111
    rank_delta_abs: 111
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HyperAggregation: Aggregating over Graph Edges with
      Hypernetworks'
    comparison_source_arxiv: '2407.11596'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.8272
    std: 0.0068
    paper_value: 0.8272
    paper_std: 0.0068
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8272
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8272
    true_std: 0.0068
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8272
    sort_std: 0.0068
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5559
    std: 0.0027
    paper_value: 0.5559
    paper_std: 0.0027
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
    variant_inference_reason: 'dataset: fuzzy match to roman-empire (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8145
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2508.17531'
    at_pub_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    at_pub_source_date_iso: '2025-08-24'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.25860000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8145
    true_std: 0.0009
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.25860000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8145
    sort_std: 0.0009
    global_rank: 82
    paper_rank: 185
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    comparison_source_arxiv: '2508.17531'
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.8001
    std: 0.0044
    paper_value: 0.8001
    paper_std: 0.0044
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6539
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1462
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8001
    true_std: 0.0044
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8001
    sort_std: 0.0044
    global_rank: 89
    paper_rank: 89
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.7992
    std: 0.0056
    paper_value: 0.7992
    paper_std: 0.0056
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
    source_ref: fsgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7992
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7992
    true_std: 0.0056
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7992
    sort_std: 0.0056
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7483
    std: 0.0081
    paper_value: 0.7483
    paper_std: 0.0081
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7342
    at_pub_std: 0.006
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.014100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7483
    true_std: 0.0081
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7483
    sort_std: 0.0081
    global_rank: 109
    paper_rank: 109
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6485
    std: 0.0027
    paper_value: 0.6485
    paper_std: 0.0027
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
    source_ref: gprgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7344
    at_pub_std: 0.003
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08590000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7344
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.08590000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.7344
    sort_std: 0.003
    global_rank: 117
    paper_rank: 150
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.6011
    std: 0.0052
    paper_value: 0.6011
    paper_std: 0.0052
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
    source_ref: h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6809
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.07979999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6809
    true_std: 0.0029
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.07979999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6809
    sort_std: 0.0029
    global_rank: 136
    paper_rank: 170
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.5963
    std: 0.0069
    paper_value: 0.5963
    paper_std: 0.0069
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
    source_ref: glognn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6739
    at_pub_std: 0.003
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0776
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6739
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.0776
    has_value_note: false
    value_note: ''
    sort_value: 0.6739
    sort_std: 0.003
    global_rank: 138
    paper_rank: 174
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.661
    std: 0.0044
    paper_value: 0.661
    paper_std: 0.0044
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6665
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.005499999999999949
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6665
    true_std: 0.0047
    value_gap_source_arxiv: '2407.11596'
    value_gap_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    value_gap_source_is_current_paper: false
    value_gap: 0.005499999999999949
    has_value_note: false
    value_note: ''
    sort_value: 0.6665
    sort_std: 0.0047
    global_rank: 141
    paper_rank: 144
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.6612
    std: 0.0029
    paper_value: 0.6612
    paper_std: 0.0029
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6612
    true_std: 0.0029
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6612
    sort_std: 0.0029
    global_rank: 144
    paper_rank: 144
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.6396
    std: 0.0062
    paper_value: 0.6396
    paper_std: 0.0062
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
    source_ref: cpgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6396
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6396
    true_std: 0.0062
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6396
    sort_std: 0.0062
    global_rank: 159
    paper_rank: 159
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
- &id008
  dataset: Squirrel
  rows:
  - model: IBG-NN
    model_key: ibg-nn
    model_plain: IBG-NN
    value: 0.7763
    std: 0.0179
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_display: Apr 2025
    date_iso: '2025-04-25'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7763
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.7747
    std: 0.0128
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7747
    sort_std: 0.0128
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DHGNN
    model_key: dhgnn
    model_plain: DHGNN
    value: 0.7684
    std: 0.0161
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7684
    sort_std: 0.0161
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.3592
    std: 0.0132
    paper_value: 0.3592
    paper_std: 0.0132
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
    source_ref: fsgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7416
    at_pub_std: null
    at_pub_source_arxiv: '2111.06748'
    at_pub_source_title: Simplifying approach to Node Classification in Graph Neural
      Networks
    at_pub_source_date_iso: '2021-11-12'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-11-12'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.3824
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7416
    true_std: null
    value_gap_source_arxiv: '2111.06748'
    value_gap_source_title: Simplifying approach to Node Classification in Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.3824
    has_value_note: false
    value_note: ''
    sort_value: 0.7416
    sort_std: null
    global_rank: 11
    paper_rank: 234
    rank_delta: 223
    rank_delta_abs: 223
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simplifying approach to Node Classification in Graph
      Neural Networks
    comparison_source_arxiv: '2111.06748'
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.3511
    std: 0.0124
    paper_value: 0.3511
    paper_std: 0.0124
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
    source_ref: glognn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7121
    at_pub_std: 0.0184
    at_pub_source_arxiv: '2505.22362'
    at_pub_source_title: Directed Homophily-Aware Graph Neural Network
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.36099999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7121
    true_std: 0.0184
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.36099999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7121
    sort_std: 0.0184
    global_rank: 19
    paper_rank: 248
    rank_delta: 229
    rank_delta_abs: 229
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directed Homophily-Aware Graph Neural Network
    comparison_source_arxiv: '2505.22362'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.351
    std: 0.0115
    paper_value: 0.351
    paper_std: 0.0115
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
    source_ref: h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.619
    at_pub_std: 0.014
    at_pub_source_arxiv: '2504.18273'
    at_pub_source_title: Efficient Learning on Large Graphs using a Densifying Regularity
      Lemma
    at_pub_source_date_iso: '2025-04-25'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.268
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.619
    true_std: 0.014
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.268
    has_value_note: false
    value_note: ''
    sort_value: 0.619
    sort_std: 0.014
    global_rank: 42
    paper_rank: 248
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    comparison_source_arxiv: '2504.18273'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4425
    std: 0.0204
    paper_value: 0.4425
    paper_std: 0.0204
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 1
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6067
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.1642
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6067
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1642
    has_value_note: false
    value_note: ''
    sort_value: 0.6067
    sort_std: null
    global_rank: 51
    paper_rank: 141
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.3981
    std: 0.0228
    paper_value: 0.3981
    paper_std: 0.0228
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.569
    at_pub_std: 0.03
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.17089999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.569
    true_std: 0.03
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.17089999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.569
    sort_std: 0.03
    global_rank: 69
    paper_rank: 188
    rank_delta: 119
    rank_delta_abs: 119
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4151
    std: 0.0234
    paper_value: 0.4151
    paper_std: 0.0234
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
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.563
    at_pub_std: 0.022
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.14789999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.563
    true_std: 0.022
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.14789999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.563
    sort_std: 0.022
    global_rank: 77
    paper_rank: 171
    rank_delta: 94
    rank_delta_abs: 94
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3895
    std: 0.0199
    paper_value: 0.3895
    paper_std: 0.0199
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
    source_ref: gprgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5435
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2505.22362'
    at_pub_source_title: Directed Homophily-Aware Graph Neural Network
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15399999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5435
    true_std: 0.0087
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.15399999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5435
    sort_std: 0.0087
    global_rank: 86
    paper_rank: 195
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directed Homophily-Aware Graph Neural Network
    comparison_source_arxiv: '2505.22362'
    is_best: false
    is_std_outlier: false
  - model: GCN+ReP
    model_key: gcn+rep
    model_plain: GCN+ReP
    value: 0.4589
    std: 0.0145
    paper_value: 0.4589
    paper_std: 0.0145
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
    source_ref: gcn-rep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4589
    true_std: 0.0145
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4589
    sort_std: 0.0145
    global_rank: 127
    paper_rank: 127
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.4558
    std: 0.0191
    paper_value: 0.4558
    paper_std: 0.0191
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4558
    true_std: 0.0191
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4558
    sort_std: 0.0191
    global_rank: 130
    paper_rank: 130
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoED
    model_key: coed
    model_plain: CoED
    value: 0.455
    std: 0.0162
    paper_value: 0.455
    paper_std: 0.0162
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
    source_ref: coed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.455
    true_std: 0.0162
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.455
    sort_std: 0.0162
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.4048
    std: 0.029
    paper_value: 0.4048
    paper_std: 0.029
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
    source_ref: hamilton2018inductiverepresentationlearninglarge
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.446
    at_pub_std: 0.013
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-11-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.041200000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.446
    true_std: 0.013
    value_gap_source_arxiv: '2411.19392'
    value_gap_source_title: Scale-aware Message Passing For Graph Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.041200000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.446
    sort_std: 0.013
    global_rank: 137
    paper_rank: 182
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.4457
    std: 0.0204
    paper_value: 0.4457
    paper_std: 0.0204
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4457
    true_std: 0.0204
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4457
    sort_std: 0.0204
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.4434
    std: 0.0194
    paper_value: 0.4434
    paper_std: 0.0194
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: m3dphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4434
    true_std: 0.0194
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4434
    sort_std: 0.0194
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.4378
    std: 0.019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 145
    sort_value: 0.4378
    sort_std: 0.019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.4265
    std: 0.0241
    paper_value: 0.4265
    paper_std: 0.0241
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3581
    at_pub_std: 0.0202
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.06840000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4265
    true_std: 0.0241
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4265
    sort_std: 0.0241
    global_rank: 158
    paper_rank: 158
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    comparison_source_arxiv: '2410.02158'
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.4197
    std: 0.0214
    paper_value: 0.4197
    paper_std: 0.0214
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4087
    at_pub_std: 0.0196
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4197
    true_std: 0.0214
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4197
    sort_std: 0.0214
    global_rank: 166
    paper_rank: 166
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.4132
    std: 0.0235
    paper_value: 0.4132
    paper_std: 0.0235
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4132
    true_std: 0.0235
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4132
    sort_std: 0.0235
    global_rank: 172
    paper_rank: 172
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+T
    model_key: gat+t
    model_plain: GAT+T
    value: 0.4036
    std: 0.0166
    paper_value: 0.4036
    paper_std: 0.0166
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4036
    true_std: 0.0166
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4036
    sort_std: 0.0166
    global_rank: 184
    paper_rank: 184
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.3939
    std: 0.0091
    paper_value: 0.3939
    paper_std: 0.0091
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3939
    true_std: 0.0091
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3939
    sort_std: 0.0091
    global_rank: 193
    paper_rank: 193
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.393
    std: 0.0079
    paper_value: 0.393
    paper_std: 0.0079
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3663
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0267
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.393
    true_std: 0.0079
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.393
    sort_std: 0.0079
    global_rank: 194
    paper_rank: 194
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.3889
    std: 0.0267
    paper_value: 0.3889
    paper_std: 0.0267
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3852
    at_pub_std: 0.0157
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0037000000000000366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3889
    true_std: 0.0267
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3889
    sort_std: 0.0267
    global_rank: 197
    paper_rank: 197
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.3004
    std: 0.0203
    paper_value: 0.3004
    paper_std: 0.0203
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
    source_ref: cpgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3004
    at_pub_std: 0.0203
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3004
    true_std: 0.0203
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3004
    sort_std: 0.0203
    global_rank: 281
    paper_rank: 281
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
- &id006
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8017
    std: 0.0048
    paper_value: 0.8017
    paper_std: 0.0048
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9302
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.12850000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.12850000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 91
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+T
    model_key: sage+t
    model_plain: SAGE+T
    value: 0.811
    std: 0.0032
    paper_value: 0.811
    paper_std: 0.0032
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8823
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.07129999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8823
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07129999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8823
    sort_std: null
    global_rank: 5
    paper_rank: 73
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8077
    std: 0.0014
    paper_value: 0.8077
    paper_std: 0.0014
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8771
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.06940000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8771
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06940000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8771
    sort_std: null
    global_rank: 9
    paper_rank: 78
    rank_delta: 69
    rank_delta_abs: 69
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8103
    std: 0.0092
    paper_value: 0.8103
    paper_std: 0.0092
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8533
    at_pub_std: null
    at_pub_source_arxiv: '2505.19762'
    at_pub_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    at_pub_source_date_iso: '2025-05-26'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.04299999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8533
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04299999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8533
    sort_std: null
    global_rank: 31
    paper_rank: 73
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    comparison_source_arxiv: '2505.19762'
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.7792
    std: 0.0093
    paper_value: 0.7792
    paper_std: 0.0093
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nagphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8341
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05489999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8341
    true_std: 0.0034
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.05489999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8341
    sort_std: 0.0034
    global_rank: 48
    paper_rank: 177
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.8303
    std: 0.0021
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 54
    sort_value: 0.8303
    sort_std: 0.0021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: sgformer
    model_plain: SGFormer
    value: 0.8005
    std: 0.0046
    paper_value: 0.8005
    paper_std: 0.0046
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: sgformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8271
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.026599999999999957
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8271
    true_std: 0.0056
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.026599999999999957
    has_value_note: false
    value_note: ''
    sort_value: 0.8271
    sort_std: 0.0056
    global_rank: 57
    paper_rank: 97
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7513
    std: 0.0093
    paper_value: 0.7513
    paper_std: 0.0093
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: nodeformer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8103
    at_pub_std: 0.0094
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05900000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8103
    true_std: 0.0094
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.05900000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8103
    sort_std: 0.0094
    global_rank: 74
    paper_rank: 231
    rank_delta: 157
    rank_delta_abs: 157
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.8093
    std: 0.0057
    paper_value: 0.8093
    paper_std: 0.0057
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graph-tarif
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8093
    true_std: 0.0057
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8093
    sort_std: 0.0057
    global_rank: 77
    paper_rank: 77
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+TS
    model_key: gcn+ts
    model_plain: GCN+TS
    value: 0.8031
    std: 0.0044
    paper_value: 0.8031
    paper_std: 0.0044
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8031
    true_std: 0.0044
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8031
    sort_std: 0.0044
    global_rank: 88
    paper_rank: 88
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.8026
    std: 0.0092
    paper_value: 0.8026
    paper_std: 0.0092
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: polynormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7953
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007299999999999973
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8026
    true_std: 0.0092
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8026
    sort_std: 0.0092
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.7938
    std: 0.0062
    paper_value: 0.7938
    paper_std: 0.0062
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7854
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.008399999999999963
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7938
    true_std: 0.0062
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7938
    sort_std: 0.0062
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.7866
    std: 0.0049
    paper_value: 0.7866
    paper_std: 0.0049
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    source_ref: graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7926
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7926
    true_std: 0.0057
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7926
    sort_std: 0.0057
    global_rank: 121
    paper_rank: 151
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.7796
    std: 0.0063
    paper_value: 0.7796
    paper_std: 0.0063
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 2
    source_ref: goat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.77
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.009599999999999942
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7796
    true_std: 0.0063
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7796
    sort_std: 0.0063
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7096
    std: 0.01
    paper_value: 0.7096
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7469
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2512.11561'
    at_pub_source_title: 'View Space: Learning Representation across Arbitrary Graphs'
    at_pub_source_date_iso: '2025-12-12'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-12-12'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.0373
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7469
    true_std: 0.0085
    value_gap_source_arxiv: '2512.11561'
    value_gap_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0373
    has_value_note: false
    value_note: ''
    sort_value: 0.7469
    sort_std: 0.0085
    global_rank: 237
    paper_rank: 265
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    comparison_source_arxiv: '2512.11561'
    is_best: false
    is_std_outlier: false
  - model: MLP+TS
    model_key: mlp+ts
    model_plain: MLP+TS
    value: 0.7248
    std: 0.0083
    paper_value: 0.7248
    paper_std: 0.0083
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for WikiCS
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7248
    true_std: 0.0083
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7248
    sort_std: 0.0083
    global_rank: 250
    paper_rank: 250
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
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
  - *id006
- benchmark: Heterophilic Graphs
  datasets:
  - *id007
  - *id008
- benchmark: Heterophily Benchmark
  datasets:
  - *id009
  - *id010
  - *id011
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
    - dataset: Minesweeper
      dataset_slug: minesweeper
main_figure: /figures/2605.20248/main_figure.jpegoptim.jpg
---

