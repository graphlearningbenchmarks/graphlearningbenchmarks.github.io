---
title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency Response Filter'
arxiv_id: '2104.12840'
source_url: ''
authors:
- name: Yushun Dong
  orcid: null
  s2_author_id: '123918726'
  s2_url: null
- name: Kaize Ding
  orcid: null
  s2_author_id: '66807781'
  s2_url: null
- name: Brian Jalaian
  orcid: null
  s2_author_id: '3116427'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '1743600'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '1737121128'
  s2_url: null
published_date: Apr 26, 2021
published_date_iso: '2021-04-26'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks have recently become a prevailing paradigm for various
  high-impact graph analytical problems. Existing efforts can be mainly categorized
  as spectral-based and spatial-based methods. The major challenge for the former
  is to find an appropriate graph filter to distill discriminative information from
  input signals for learning. Recently, myriads of explorations are made to achieve
  better graph filters, e.g., Graph Convolutional Network (GCN), which leverages Chebyshev
  polynomial truncation to seek an approximation of graph filters and bridge these
  two families of methods. Nevertheless, it has been shown in recent studies that
  GCN and its variants are essentially employing fixed low-pass filters to perform
  information denoising. Thus their learning capability is rather limited and may
  over-smooth node representations at deeper layers. To tackle these problems, we
  develop a novel graph neural network framework AdaGNN with a well-designed adaptive
  frequency response filter. At its core, AdaGNN leverages a simple but elegant trainable
  filter that spans across multiple layers to capture the varying importance of different
  frequency components for node representation learning. The inherent differences
  among different feature channels are also well captured by the filter. As such,
  it empowers AdaGNN with stronger expressiveness and naturally alleviates the over-smoothing
  problem. We empirically validate the effectiveness of the proposed framework on
  various benchmark datasets. Theoretical analysis is also provided to show the superiority
  of the proposed AdaGNN. The open-source implementation of AdaGNN can be found here:
  https://github.com/yushundong/AdaGNN.'
codebase_url: https://github.com/yushundong/AdaGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AdaGNN-R
- AdaGNN-S
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ACM
  rows:
  - model: GCN+P+D
    model_key: signgt
    model_plain: GCN+P+D
    value: 0.9545
    std: 0.0049
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9545
    sort_std: 0.0049
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN+P+D
    model_key: nodeformer
    model_plain: GCN+P+D
    value: 0.9493
    std: 0.0035
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9493
    sort_std: 0.0035
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN+P+D
    model_key: fagcn
    model_plain: GCN+P+D
    value: 0.9487
    std: 0.0059
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9487
    sort_std: 0.0059
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7514
    std: 0.001
    paper_value: 0.7514
    paper_std: 0.001
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
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9324
    true_std: 0.0049
    value_gap_source_arxiv: '2406.19258'
    value_gap_source_title: Leveraging Contrastive Learning for Enhanced Node Representations
      in Tokenized Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.18100000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9324
    sort_std: 0.0049
    global_rank: 29
    paper_rank: 70
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7555
    std: 0.002
    paper_value: 0.7555
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: 0.0038
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.16780000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0038
    global_rank: 41
    paper_rank: 67
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGNN-S
    model_key: adagnn-s
    model_plain: AdaGNN-S
    value: 0.7583
    std: 0.004
    paper_value: 0.7583
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7583
    true_std: 0.004
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7583
    sort_std: 0.004
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pairnorm-GCN-SCS
    model_key: pairnorm-gcn-scs
    model_plain: Pairnorm-GCN-SCS
    value: 0.7544
    std: 0.001
    paper_value: 0.7544
    paper_std: 0.001
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
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7544
    true_std: 0.001
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7544
    sort_std: 0.001
    global_rank: 68
    paper_rank: 68
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
    value: 0.7529
    std: 0.002
    paper_value: 0.7529
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7529
    true_std: 0.002
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7529
    sort_std: 0.002
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGNN-R
    model_key: adagnn-r
    model_plain: AdaGNN-R
    value: 0.7527
    std: 0.001
    paper_value: 0.7527
    paper_std: 0.001
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7527
    true_std: 0.001
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7527
    sort_std: 0.001
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pairnorm-GCN-SI
    model_key: pairnorm-gcn-si
    model_plain: Pairnorm-GCN-SI
    value: 0.7487
    std: 0.003
    paper_value: 0.7487
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7487
    true_std: 0.003
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7487
    sort_std: 0.003
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DropEdge-GCN
    model_key: dropedge-gcn
    model_plain: DropEdge-GCN
    value: 0.7305
    std: 0.006
    paper_value: 0.7305
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10% train, 20% val, 70% test split
    date: Apr 26, 2021
    date_display: Apr 2021
    date_iso: '2021-04-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-26'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7305
    true_std: 0.006
    value_gap_source_arxiv: '2104.12840'
    value_gap_source_title: 'AdaGNN: Graph Neural Networks with Adaptive Frequency
      Response Filter'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7305
    sort_std: 0.006
    global_rank: 73
    paper_rank: 73
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
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: ACM
      dataset_slug: acm
main_figure: /figures/2104.12840/main_figure.jpegoptim.jpg
---

