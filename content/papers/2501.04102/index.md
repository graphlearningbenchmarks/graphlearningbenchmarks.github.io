---
title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
  Generalization
arxiv_id: '2501.04102'
source_url: ''
authors:
- name: Song Wang
  orcid: null
  s2_author_id: '2117075272'
  s2_url: null
- name: Xiaodong Yang
  orcid: null
  s2_author_id: '2308048394'
  s2_url: null
- name: Rashidul Islam
  orcid: null
  s2_author_id: '2284868070'
  s2_url: null
- name: Huiyuan Chen
  orcid: null
  s2_author_id: '2284864789'
  s2_url: null
- name: Minghua Xu
  orcid: null
  s2_author_id: '2285001003'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '1737121128'
  s2_url: null
- name: Yiwei Cai
  orcid: null
  s2_author_id: '2232929519'
  s2_url: null
published_date: Dec 9, 2024
published_date_iso: '2024-12-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: To deal with distribution shifts in graph data, various graph out-of-distribution
  (OOD) generalization techniques have been recently proposed. These methods often
  employ a two-step strategy that first creates augmented environments and subsequently
  identifies invariant subgraphs to improve generalizability. Nevertheless, this approach
  could be suboptimal from the perspective of consistency. First, the process of augmenting
  environments by altering the graphs while preserving labels may lead to graphs that
  are not realistic or meaningfully related to the origin distribution, thus lacking
  distribution consistency. Second, the extracted subgraphs are obtained from directly
  modifying graphs, and may not necessarily maintain a consistent predictive relationship
  with their labels, thereby impacting label consistency. In response to these challenges,
  we introduce an innovative approach that aims to enhance these two types of consistency
  for graph OOD generalization. We propose a modifier to obtain both augmented and
  invariant graphs in a unified manner. With the augmented graphs, we enrich the training
  data without compromising the integrity of label-graph relationships. The label
  consistency enhancement in our framework further preserves the supervision information
  in the invariant graph. We conduct extensive experiments on real-world datasets
  to demonstrate the superiority of our framework over other state-of-the-art baselines.
codebase_url: https://github.com/SongW-SW/DLG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DLG
mrr: 0.025
adjusted_mrr: 0.0083
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ogbg-molhiv
  rows:
  - model: Multi-RF Fusion with Multi-GNN Blending
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: Multi-RF Fusion with Multi-GNN Blending
    value: 0.8476
    std: 0.0002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: Mixing pharmacophoric (FCFP) and structural (ECFP) fingerprints...
      GNNs contributing only 12%
    is_global_top: true
    global_rank: 1
    sort_value: 0.8476
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HyperFusion
    model_key: hyperfusion
    model_plain: HyperFusion
    value: 0.8475
    std: 0.0003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8475
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PAS+FPs
    model_key: pas+fps
    model_plain: PAS+FPs
    value: 0.842
    std: 0.0015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.842
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.809
    std: 0.016
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_display: Sep 2023
    date_iso: '2023-09-18'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 12
    sort_value: 0.809
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSN
    model_key: gsn
    model_plain: GSN
    value: 0.7453
    std: 0.0139
    paper_value: 0.7453
    paper_std: 0.0139
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8039
    at_pub_std: 0.009
    at_pub_source_arxiv: '2210.13978'
    at_pub_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    at_pub_source_date_iso: '2022-10-22'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-04-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.058599999999999985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8039
    true_std: 0.009
    value_gap_source_arxiv: '2404.13344'
    value_gap_source_title: 'GRANOLA: Adaptive Normalization for Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.058599999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.8039
    sort_std: 0.009
    global_rank: 22
    paper_rank: 263
    rank_delta: 241
    rank_delta_abs: 241
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    comparison_source_arxiv: '2210.13978'
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.8018
    std: 0.0182
    paper_value: 0.8018
    paper_std: 0.0182
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7982
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2406.07955'
    at_pub_source_title: How Interpretable Are Interpretable Graph Neural Networks?
    at_pub_source_date_iso: '2024-06-12'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8018
    true_std: 0.0182
    value_gap_source_arxiv: '2501.04102'
    value_gap_source_title: Enhancing Distribution and Label Consistency for Graph
      Out-of-Distribution Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8018
    sort_std: 0.0182
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DLG
    model_key: dlg
    model_plain: DLG
    value: 0.798
    std: 0.0178
    paper_value: 0.798
    paper_std: 0.0178
    metric: ROC-AUC
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.0178
    value_gap_source_arxiv: '2501.04102'
    value_gap_source_title: Enhancing Distribution and Label Consistency for Graph
      Out-of-Distribution Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.0178
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.797
    std: 0.0192
    paper_value: 0.797
    paper_std: 0.0192
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-11'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7975
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0004999999999999449
    has_value_note: false
    value_note: ''
    sort_value: 0.7975
    sort_std: null
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.7446
    std: 0.0105
    paper_value: 0.7446
    paper_std: 0.0105
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7947
    at_pub_std: 0.0186
    at_pub_source_arxiv: '2206.02886'
    at_pub_source_title: Graph Rationalization with Environment-based Augmentations
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.05009999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7947
    true_std: 0.0186
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: false
    value_gap: 0.05009999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.7947
    sort_std: 0.0186
    global_rank: 50
    paper_rank: 264
    rank_delta: 214
    rank_delta_abs: 214
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Rationalization with Environment-based Augmentations
    comparison_source_arxiv: '2206.02886'
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.7908
    std: 0.0247
    paper_value: 0.7908
    paper_std: 0.0247
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-11'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7908
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7908
    sort_std: null
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.778
    std: 0.0182
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 510.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 120
    sort_value: 0.778
    sort_std: 0.0182
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Attention
    model_key: attention
    model_plain: Attention
    value: 0.7584
    std: 0.0367
    paper_value: 0.7584
    paper_std: 0.0367
    metric: ROC-AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7744
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2205.15068'
    at_pub_source_title: Embedding Graphs on Grassmann Manifold
    at_pub_source_date_iso: '2022-05-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7744
    true_std: 0.0127
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.016000000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.7744
    sort_std: 0.0127
    global_rank: 137
    paper_rank: 227
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.7705
    std: 0.0398
    paper_value: 0.7705
    paper_std: 0.0398
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7705
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-02-11'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7705
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7705
    sort_std: null
    global_rank: 165
    paper_rank: 165
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.762
    std: 0.0254
    paper_value: 0.762
    paper_std: 0.0254
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.762
    at_pub_std: 0.0114
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.762
    true_std: 0.0254
    value_gap_source_arxiv: '2501.04102'
    value_gap_source_title: Enhancing Distribution and Label Consistency for Graph
      Out-of-Distribution Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.0254
    global_rank: 207
    paper_rank: 207
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: V-REx
    model_key: v-rex
    model_plain: V-REx
    value: 0.7562
    std: 0.0331
    paper_value: 0.7562
    paper_std: 0.0331
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test AUC-ROC reported in Table 2
    date: Dec 9, 2024
    date_display: Dec 2024
    date_iso: '2024-12-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7562
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7562
    true_std: 0.0331
    value_gap_source_arxiv: '2501.04102'
    value_gap_source_title: Enhancing Distribution and Label Consistency for Graph
      Out-of-Distribution Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7562
    sort_std: 0.0331
    global_rank: 236
    paper_rank: 236
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
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
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
single_proposed_model: DLG
main_figure: /figures/2501.04102/main_figure.jpegoptim.jpg
---

