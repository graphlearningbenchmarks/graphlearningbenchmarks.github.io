---
title: Heterogeneous Graph Benchmarks
arxiv_id: '2112.14936'
source_url: ''
authors:
- name: Qingsong Lv
  orcid: null
  s2_author_id: '2053104889'
  s2_url: null
- name: Ming Ding
  orcid: null
  s2_author_id: '145573466'
  s2_url: null
- name: Qiang Liu
  orcid: null
  s2_author_id: '2146553789'
  s2_url: null
- name: Yuxiang Chen
  orcid: null
  s2_author_id: '2109168537'
  s2_url: null
- name: Wenzheng Feng
  orcid: null
  s2_author_id: '2114325306'
  s2_url: null
- name: Siming He
  orcid: null
  s2_author_id: '2148909280'
  s2_url: null
- name: Chang Zhou
  orcid: null
  s2_author_id: '144161025'
  s2_url: null
- name: Jianguo Jiang
  orcid: null
  s2_author_id: '152634491'
  s2_url: null
- name: Yuxiao Dong
  orcid: null
  s2_author_id: '2047998'
  s2_url: null
- name: Jie Tang
  orcid: null
  s2_author_id: '2109541439'
  s2_url: null
published_date: Aug 14, 2021
published_date_iso: '2021-08-14'
published_venue: KDD 2021
published_conference: KDD 2021
published_conference_short: KDD
published_conference_slug: kdd
abstract: Heterogeneous graph neural networks (HGNNs) have been blossoming in recent
  years, but the unique data processing and evaluation setups used by each work obstruct
  a full understanding of their advancements. In this work, we present a systematical
  reproduction of 12 recent HGNNs by using their official codes, datasets, settings,
  and hyperparameters, revealing surprising findings about the progress of HGNNs.
  We find that the simple homogeneous GNNs, e.g., GCN and GAT, are largely underestimated
  due to improper settings. GAT with proper inputs can generally match or outperform
  all existing HGNNs across various scenarios. To facilitate robust and reproducible
  HGNN research, we construct the Heterogeneous Graph Benchmark (HGB), and the HGB
  leaderboard is at linkcolor., consisting of 11 diverse datasets with three tasks.
  HGB standardizes the process of heterogeneous graph data splits, feature processing,
  and performance evaluation. Finally, we introduce a simple but very strong baseline
  Simple-HGN ---which significantly outperforms all previous models on HGB---to accelerate
  the advancement of HGNNs in the future.
codebase_url: https://github.com/THUDM/HGB
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 4
  total: 4
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id003
  dataset: ACM
  rows:
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.8605
    std: 0.0025
    paper_value: 0.8605
    paper_std: 0.0025
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.979
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.11849999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.979
    sort_std: null
    global_rank: 1
    paper_rank: 97
    rank_delta: 96
    rank_delta_abs: 96
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: comch
    model_plain: SlotGAT
    value: 0.947
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    venue: Knowledge-Based Systems
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: lmsps
    model_plain: SlotGAT
    value: 0.9469
    std: 0.0036
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9469
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9141
    std: 0.0075
    paper_value: 0.9141
    paper_std: 0.0075
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9402
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.026100000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.9402
    sort_std: null
    global_rank: 7
    paper_rank: 53
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9077
    std: 0.0065
    paper_value: 0.9077
    paper_std: 0.0065
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9361
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.028400000000000092
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: null
    global_rank: 17
    paper_rank: 59
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.9335
    std: 0.0045
    paper_value: 0.9335
    paper_std: 0.0045
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: 'Simple-HGN can be viewed as GAT enhanced by three existing
      techniques: (1) learnable type embedding... (2) residual connections... (3)
      L2 normalization...'
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9335
    true_std: 0.0045
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9335
    sort_std: 0.0045
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9219
    std: 0.0093
    paper_value: 0.9219
    paper_std: 0.0093
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9278
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.005899999999999905
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9278
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.005899999999999905
    has_value_note: false
    value_note: ''
    sort_value: 0.9278
    sort_std: null
    global_rank: 31
    paper_rank: 43
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.912
    std: 0.0071
    paper_value: 0.912
    paper_std: 0.0071
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9258
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.013799999999999923
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9258
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.013799999999999923
    has_value_note: false
    value_note: ''
    sort_value: 0.9258
    sort_std: null
    global_rank: 34
    paper_rank: 56
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9212
    std: 0.0023
    paper_value: 0.9212
    paper_std: 0.0023
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9246
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.0033999999999999586
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9246
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0033999999999999586
    has_value_note: false
    value_note: ''
    sort_value: 0.9246
    sort_std: null
    global_rank: 36
    paper_rank: 45
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9079
    std: 0.0043
    paper_value: 0.9079
    paper_std: 0.0043
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.879
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.028900000000000037
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9185
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.010599999999999943
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: null
    global_rank: 50
    paper_rank: 59
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.91
    std: 0.0076
    paper_value: 0.91
    paper_std: 0.0076
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.916
    true_std: 0.006
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: 0.006
    global_rank: 53
    paper_rank: 58
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.9032
    std: 0.0154
    paper_value: 0.9032
    paper_std: 0.0154
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9032
    true_std: 0.0154
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9032
    sort_std: 0.0154
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
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.8991
    std: 0.0037
    paper_value: 0.8991
    paper_std: 0.0037
    metric: Micro-F1
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
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8991
    true_std: 0.0037
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8991
    sort_std: 0.0037
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
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: DBLP
  rows:
  - model: SlotGAT
    model_key: herec
    model_plain: SlotGAT
    value: 0.9993
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9993
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.8056
    std: 0.015
    paper_value: 0.8056
    paper_std: 0.015
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9972
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.1916
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9972
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1916
    has_value_note: false
    value_note: ''
    sort_value: 0.9972
    sort_std: null
    global_rank: 2
    paper_rank: 125
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: deepwalk
    model_plain: SlotGAT
    value: 0.9941
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9941
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9207
    std: 0.005
    paper_value: 0.9207
    paper_std: 0.005
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.029299999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 18
    paper_rank: 71
    rank_delta: 53
    rank_delta_abs: 53
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
    value: 0.9147
    std: 0.0034
    paper_value: 0.9147
    paper_std: 0.0034
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.931
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.016300000000000092
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.946
    true_std: 0.0031
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.946
    sort_std: 0.0031
    global_rank: 28
    paper_rank: 76
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9339
    std: 0.003
    paper_value: 0.9339
    paper_std: 0.003
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9178
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.016100000000000003
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9448
    true_std: 0.0022
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.01090000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0022
    global_rank: 29
    paper_rank: 51
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.9446
    std: 0.0022
    paper_value: 0.9446
    paper_std: 0.0022
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: 'Simple-HGN can be viewed as GAT enhanced by three existing
      techniques: (1) learnable type embedding... (2) residual connections... (3)
      L2 normalization...'
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9448
    true_std: 0.0038
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0038
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.9397
    std: 0.0054
    paper_value: 0.9397
    paper_std: 0.0054
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9417
    true_std: 0.0026
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.9417
    sort_std: 0.0026
    global_rank: 39
    paper_rank: 40
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.9381
    std: 0.0055
    paper_value: 0.9381
    paper_std: 0.0055
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9381
    true_std: 0.0055
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9381
    sort_std: 0.0055
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9376
    std: 0.0045
    paper_value: 0.9376
    paper_std: 0.0045
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9456
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9376
    true_std: 0.0045
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9376
    sort_std: 0.0045
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9205
    std: 0.0062
    paper_value: 0.9205
    paper_std: 0.0062
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9291
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.008600000000000052
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9369
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: false
    value_gap: 0.01639999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9369
    sort_std: null
    global_rank: 46
    paper_rank: 71
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.9349
    std: 0.0025
    paper_value: 0.9349
    paper_std: 0.0025
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9365
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0016000000000000458
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9349
    true_std: 0.0025
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9349
    sort_std: 0.0025
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.9233
    std: 0.0041
    paper_value: 0.9233
    paper_std: 0.0041
    metric: Micro-F1
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
    protocol_note: Node classification task on DBLP using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.9336
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.010299999999999976
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9233
    true_std: 0.0041
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0041
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: Freebase
  rows:
  - model: SlotGAT
    model_key: gc-hgnn
    model_plain: SlotGAT
    value: 0.6247
    std: 0.0042
    metric: Macro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 1
    sort_value: 0.6247
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: hgmae
    model_plain: SlotGAT
    value: 0.6082
    std: 0.0051
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 2
    sort_value: 0.6082
    sort_std: 0.0051
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: heco
    model_plain: SlotGAT
    value: 0.5987
    std: 0.0033
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 3
    sort_value: 0.5987
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.2131
    std: 0.0168
    paper_value: 0.2131
    paper_std: 0.0168
    metric: Macro-F1
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6011
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.38799999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.585
    true_std: 0.0093
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.37189999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.585
    sort_std: 0.0093
    global_rank: 8
    paper_rank: 39
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.2928
    std: 0.0252
    paper_value: 0.2928
    paper_std: 0.0252
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6176
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32480000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.583
    true_std: 0.0072
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.29019999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.583
    sort_std: 0.0072
    global_rank: 9
    paper_rank: 35
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.4772
    std: 0.0148
    paper_value: 0.4772
    paper_std: 0.0148
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4772
    true_std: 0.0148
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4772
    sort_std: 0.0148
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.4678
    std: 0.0077
    paper_value: 0.4678
    paper_std: 0.0077
    metric: Macro-F1
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4678
    true_std: 0.0077
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4678
    sort_std: 0.0077
    global_rank: 26
    paper_rank: 26
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
    value: 0.4074
    std: 0.0258
    paper_value: 0.4074
    paper_std: 0.0258
    metric: Macro-F1
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.5109
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.10350000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4074
    true_std: 0.0258
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4074
    sort_std: 0.0258
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2784
    std: 0.0313
    paper_value: 0.2784
    paper_std: 0.0313
    metric: Macro-F1
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase test split; Macro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.609
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3306
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2935
    true_std: null
    value_gap_source_arxiv: '2403.04780'
    value_gap_source_title: Graph-oriented Instruction Tuning of Large Language Models
      for Generic Graph Mining
    value_gap_source_is_current_paper: false
    value_gap: 0.015100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2935
    sort_std: null
    global_rank: 35
    paper_rank: 36
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  rank_metric: Macro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Macro-F1
  paper_metrics:
  - Macro-F1
  metric: Macro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: IMDB
  rows:
  - model: SlotGAT
    model_key: gat bgnn(m)-sc
    model_plain: SlotGAT
    value: 0.8133
    std: 0.0179
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8133
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: sage ban
    model_plain: SlotGAT
    value: 0.8073
    std: 0.002
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8073
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: gat bgnn(m)-cs
    model_plain: SlotGAT
    value: 0.8033
    std: 0.0094
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8033
    sort_std: 0.0094
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.5768
    std: 0.0044
    paper_value: 0.5768
    paper_std: 0.0044
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.7311
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.1543
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7311
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1543
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: null
    global_rank: 34
    paper_rank: 100
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.6514
    std: 0.0045
    paper_value: 0.6514
    paper_std: 0.0045
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6827
    true_std: 0.0065
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6827
    sort_std: 0.0065
    global_rank: 43
    paper_rank: 64
    rank_delta: 21
    rank_delta_abs: 21
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
    value: 0.6482
    std: 0.0064
    paper_value: 0.6482
    paper_std: 0.0064
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6378
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.010399999999999965
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6813
    true_std: 0.0083
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03310000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6813
    sort_std: 0.0083
    global_rank: 45
    paper_rank: 67
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6486
    std: 0.0043
    paper_value: 0.6486
    paper_std: 0.0043
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6519
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0033000000000000806
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6808
    true_std: 0.0049
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.032200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0049
    global_rank: 46
    paper_rank: 66
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.6467
    std: 0.0167
    paper_value: 0.6467
    paper_std: 0.0167
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6782
    true_std: 0.0154
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03149999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6782
    sort_std: 0.0154
    global_rank: 48
    paper_rank: 70
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.6463
    std: 0.0058
    paper_value: 0.6463
    paper_std: 0.0058
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6298
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.01649999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6769
    true_std: 0.0064
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03059999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6769
    sort_std: 0.0064
    global_rank: 49
    paper_rank: 70
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.6736
    std: 0.0057
    paper_value: 0.6736
    paper_std: 0.0057
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: 'Simple-HGN can be viewed as GAT enhanced by three existing
      techniques: (1) learnable type embedding... (2) residual connections... and
      (3) L2 normalization...'
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6736
    true_std: 0.0057
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6736
    sort_std: 0.0057
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.672
    std: 0.0057
    paper_value: 0.672
    paper_std: 0.0057
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6365
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.03550000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.672
    true_std: 0.0057
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.672
    sort_std: 0.0057
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.6205
    std: 0.0015
    paper_value: 0.6205
    paper_std: 0.0015
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6359
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.01539999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6651
    true_std: 0.0028
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.04459999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6651
    sort_std: 0.0028
    global_rank: 61
    paper_rank: 82
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.6422
    std: 0.0103
    paper_value: 0.6422
    paper_std: 0.0103
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.6337
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.008499999999999952
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6422
    true_std: 0.0103
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6422
    sort_std: 0.0103
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.5116
    std: 0.0065
    paper_value: 0.5116
    paper_std: 0.0065
    metric: Micro-F1
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
    protocol_note: Node classification task on IMDB dataset using Micro-F1 metric.
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5116
    true_std: 0.0065
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5116
    sort_std: 0.0065
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
    value: 0.991
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: supcosine
    model_plain: ECC
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8088
    std: null
    paper_value: 0.8088
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.901
    at_pub_std: 0.0584
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.09220000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.901
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.09220000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.901
    sort_std: 0.058
    global_rank: 164
    paper_rank: 599
    rank_delta: 435
    rank_delta_abs: 435
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    comparison_source_arxiv: '2106.04319'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7941
    std: null
    paper_value: 0.7941
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: 0.891
    at_pub_std: 0.0581
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-08-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.09689999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.891
    true_std: 0.058
    value_gap_source_arxiv: '2308.08235'
    value_gap_source_title: 'The Expressive Power of Graph Neural Networks: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.09689999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.891
    sort_std: 0.058
    global_rank: 250
    paper_rank: 646
    rank_delta: 396
    rank_delta_abs: 396
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    comparison_source_arxiv: '2106.04319'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.8235
    std: null
    paper_value: 0.8235
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: han
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-14'
    value_gap_source_date_label: KDD 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8235
    true_std: null
    value_gap_source_arxiv: '2112.14936'
    value_gap_source_title: Heterogeneous Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8235
    sort_std: null
    global_rank: 561
    paper_rank: 561
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.8235
    std: null
    paper_value: 0.8235
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gtn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-14'
    value_gap_source_date_label: KDD 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8235
    true_std: null
    value_gap_source_arxiv: '2112.14936'
    value_gap_source_title: Heterogeneous Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8235
    sort_std: null
    global_rank: 562
    paper_rank: 562
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.8235
    std: null
    paper_value: 0.8235
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: rshn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV on MUTAG
    date: Aug 14, 2021
    date_display: Aug 2021
    date_iso: '2021-08-14'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-14'
    value_gap_source_date_label: KDD 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8235
    true_std: null
    value_gap_source_arxiv: '2112.14936'
    value_gap_source_title: Heterogeneous Graph Benchmarks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8235
    sort_std: null
    global_rank: 563
    paper_rank: 563
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: IMDB
      dataset_slug: imdb
    - dataset: Freebase
      dataset_slug: freebase
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
main_figure: /figures/2112.14936/main_figure.jpegoptim.jpg
---

