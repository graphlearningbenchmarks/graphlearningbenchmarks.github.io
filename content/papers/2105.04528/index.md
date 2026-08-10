---
title: Accelerating Large Scale Real-Time GNN Inference using Channel Pruning
arxiv_id: '2105.04528'
source_url: ''
authors:
- name: Hongkuan Zhou
  orcid: null
  s2_author_id: '1443735039'
  s2_url: null
- name: Ajitesh Srivastava
  orcid: null
  s2_author_id: '2215594'
  s2_url: null
- name: Hanqing Zeng
  orcid: null
  s2_author_id: '1750905107'
  s2_url: null
- name: Rajgopal Kannan
  orcid: null
  s2_author_id: '2286832947'
  s2_url: null
- name: Viktor Prasanna
  orcid: null
  s2_author_id: '1728271'
  s2_url: null
published_date: May 10, 2021
published_date_iso: '2021-05-10'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) are proven to be powerful models to generate
  node embedding for downstream applications. However, due to the high computation
  complexity of GNN inference, it is hard to deploy GNNs for large-scale or real-time
  applications. In this paper, we propose to accelerate GNN inference by pruning the
  dimensions in each layer with negligible accuracy loss. Our pruning framework uses
  a novel LASSO regression formulation for GNNs to identify feature dimensions (channels)
  that have high influence on the output activation. We identify two inference scenarios
  and design pruning schemes based on their computation and memory usage for each.
  To further reduce the inference complexity, we effectively store and reuse hidden
  features of visited nodes, which significantly reduces the number of supporting
  nodes needed to compute the target embedding. We evaluate the proposed method with
  the node classification problem on five popular datasets and a real-time spam detection
  application. We demonstrate that the pruned GNN models greatly reduce computation
  and memory usage with little accuracy loss. For full inference, the proposed method
  achieves an average of $3.27 $ speedup with only $0.002$ drop in F1-Micro on GPU.
  For batched inference, the proposed method achieves an average of $6.67 $ speedup
  with only $0.003$ drop in F1-Micro on CPU. To the best of our knowledge, we are
  the first to accelerate large scale real-time GNN inference through channel pruning.
codebase_url: https://github.com/tedzhouhk/GCNP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LASSO 2x
- LASSO 4x
- LASSO 8x
- LASSO
mrr: 0.0435
adjusted_mrr: 0.0145
mrr_dataset_count: 1
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
  dataset: Reddit
  rows:
  - model: Node Sampled Soup
    model_key: node sampled soup
    model_plain: Node Sampled Soup
    value: 0.9728
    std: 0.0008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_display: Jun 2023
    date_iso: '2023-06-18'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/VITA-Group/graph_ladling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9728
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EnGCN
    model_key: engcn
    model_plain: EnGCN
    value: 0.9714
    std: 0.0003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9714
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.971
    std: 0.0
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.971
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LASSO 2x
    model_key: lasso 2x
    model_plain: LASSO 2x
    value: 0.966
    std: null
    paper_value: 0.966
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Full inference on Reddit dataset using standard split
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN(2,0,0)
    model_key: sign(2,0,0)
    model_plain: SIGN(2,0,0)
    value: 0.966
    std: null
    paper_value: 0.966
    paper_std: null
    metric: F1
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
    protocol_note: Full inference on Reddit dataset
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
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
    value: 0.966
    std: null
    paper_value: 0.966
    paper_std: null
    metric: F1
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
    protocol_note: Full inference on Reddit dataset using standard split
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.954
    at_pub_std: null
    at_pub_source_arxiv: '1803.07294'
    at_pub_source_title: 'GaAN: Gated Attention Networks for Learning on Large and
      Spatiotemporal Graphs'
    at_pub_source_date_iso: '2018-03-20'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.01200000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GaAN: Gated Attention Networks for Learning on Large
      and Spatiotemporal Graphs'
    comparison_source_arxiv: '1803.07294'
    is_best: false
    is_std_outlier: false
  - model: LASSO 4x
    model_key: lasso 4x
    model_plain: LASSO 4x
    value: 0.964
    std: null
    paper_value: 0.964
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Full inference on Reddit dataset using standard split
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.964
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.964
    sort_std: null
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LASSO
    model_key: lasso
    model_plain: LASSO
    value: 0.964
    std: null
    paper_value: 0.964
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Full inference on Reddit dataset
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.964
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.964
    sort_std: null
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LASSO 8x
    model_key: lasso 8x
    model_plain: LASSO 8x
    value: 0.959
    std: null
    paper_value: 0.959
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Full inference on Reddit dataset using standard split
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.959
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TinyGNN
    model_key: tinygnn
    model_plain: TinyGNN
    value: 0.957
    std: null
    paper_value: 0.957
    paper_std: null
    metric: F1
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
    protocol_note: Full inference on Reddit dataset
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.957
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.957
    sort_std: null
    global_rank: 59
    paper_rank: 59
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
    value: 0.953
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.10803'
    title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    date: May 22, 2022
    date_display: May 2022
    date_iso: '2022-05-22'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/THUDM/GraphMAE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 68
    sort_value: 0.953
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.949
    std: null
    paper_value: 0.949
    paper_std: null
    metric: F1
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
    protocol_note: Full inference on Reddit dataset
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.949
    at_pub_std: null
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.949
    true_std: 0.0
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0
    global_rank: 87
    paper_rank: 87
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPRGo
    model_key: pprgo
    model_plain: PPRGo
    value: 0.937
    std: null
    paper_value: 0.937
    paper_std: null
    metric: F1
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
    protocol_note: Full inference on Reddit dataset
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
    global_rank: 113
    paper_rank: 113
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
    value: 0.7216
    std: 0.0015
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/GraphAny
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 162
    sort_value: 0.7216
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
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
    - dataset: Reddit
      dataset_slug: reddit
main_figure: /figures/2105.04528/main_figure.jpegoptim.jpg
---

