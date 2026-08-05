---
title: Graph Sparsification via Mixture of Graphs
arxiv_id: '2405.14260'
source_url: ''
authors:
- name: Guibin Zhang
  orcid: null
  s2_author_id: '2232926268'
  s2_url: null
- name: Xiangguo Sun
  orcid: null
  s2_author_id: '2302792188'
  s2_url: null
- name: Yanwei Yue
  orcid: null
  s2_author_id: '2282473982'
  s2_url: null
- name: Kun Wang
  orcid: null
  s2_author_id: '2302315766'
  s2_url: null
- name: Tianlong Chen
  orcid: null
  s2_author_id: '2282507790'
  s2_url: null
- name: Shirui Pan
  orcid: null
  s2_author_id: '2302831053'
  s2_url: null
published_date: May 23, 2024
published_date_iso: '2024-05-23'
published_venue: ICLR 2024
published_conference: ICLR 2024
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Graph Neural Networks (GNNs) have demonstrated superior performance across
  various graph learning tasks but face significant computational challenges when
  applied to large-scale graphs. One effective approach to mitigate these challenges
  is graph sparsification, which involves removing non-essential edges to reduce computational
  overhead. However, previous graph sparsification methods often rely on a single
  global sparsity setting and uniform pruning criteria, failing to provide customized
  sparsification schemes for each node's complex local context. In this paper, we
  introduce Mixture-of-Graphs (MoG), leveraging the concept of Mixture-of-Experts
  (MoE), to dynamically select tailored pruning solutions for each node. Specifically,
  MoG incorporates multiple sparsifier experts, each characterized by unique sparsity
  levels and pruning criteria, and selects the appropriate experts for each node.
  Subsequently, MoG performs a mixture of the sparse graphs produced by different
  experts on the Grassmann manifold to derive an optimal sparse graph. One notable
  property of MoG is its entirely local nature, as it depends on the specific circumstances
  of each individual node. Extensive experiments on four large-scale OGB datasets
  and two superpixel datasets, equipped with five GNN backbones, demonstrate that
  MoG (I) identifies subgraphs at higher sparsity levels ($8.67\ anonymously available
  at.
codebase_url: https://github.com/yanweiyue/MoG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MoG
mrr: 0.3333
adjusted_mrr: 0.1111
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ogbn-proteins
  rows:
  - model: LD
    model_key: ld
    model_plain: LD
    value: 0.8942
    std: 0.0007
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8942
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: X_WO/LD
    model_key: x_wo/ld
    model_plain: X_WO/LD
    value: 0.8915
    std: 0.0012
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8915
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoG
    model_key: mog
    model_plain: MoG
    value: 0.8904
    std: 0.0072
    paper_value: 0.8904
    paper_std: 0.0072
    metric: ROC-AUC
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: MoG applied to RevGNN backbone
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    published_venue: ICLR 2024
    published_conference: ICLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8904
    true_std: 0.0072
    value_gap_source_arxiv: '2405.14260'
    value_gap_source_title: Graph Sparsification via Mixture of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.0072
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.843
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_display: Sep 2024
    date_iso: '2024-09-09'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: https://github.com/LirongWu/GSSC
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.843
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7204
    std: 0.0048
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 69
    sort_value: 0.7204
    sort_std: 0.0048
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-proteins
      dataset_slug: ogbn-proteins
single_proposed_model: MoG
main_figure: /figures/2405.14260/main_figure.jpegoptim.jpg
---

