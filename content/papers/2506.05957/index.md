---
title: Pruning Spurious Subgraphs for Graph Out-of-Distribution Generalization
arxiv_id: '2506.05957'
source_url: ''
authors:
- name: Tianjun Yao
  orcid: null
  s2_author_id: '2301313448'
  s2_url: null
- name: Haoxuan Li
  orcid: null
  s2_author_id: '2359469600'
  s2_url: null
- name: Yongqiang Chen
  orcid: null
  s2_author_id: '2311967834'
  s2_url: null
- name: Tongliang Liu
  orcid: null
  s2_author_id: '2273817890'
  s2_url: null
- name: Le Song
  orcid: null
  s2_author_id: '2335080624'
  s2_url: null
- name: Eric P. Xing
  orcid: null
  s2_author_id: '2269472187'
  s2_url: null
- name: Zhiqiang Shen
  orcid: null
  s2_author_id: '2301791904'
  s2_url: null
published_date: Jun 6, 2025
published_date_iso: '2025-06-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks (GNNs) often encounter significant performance degradation
  under distribution shifts between training and test data, hindering their applicability
  in real-world scenarios. Recent studies have proposed various methods to address
  the out-of-distribution (OOD) generalization challenge, with many methods in the
  graph domain focusing on directly identifying an invariant subgraph that is predictive
  of the target label. However, we argue that identifying the edges from the invariant
  subgraph directly is challenging and error-prone, especially when some spurious
  edges exhibit strong correlations with the targets. In this paper, we propose PrunE,
  the first pruning-based graph OOD method that eliminates spurious edges to improve
  OOD generalizability. By pruning spurious edges, PrunE retains the invariant subgraph
  more comprehensively, which is critical for OOD generalization. Specifically, PrunE
  employs two regularization terms to prune spurious edges: 1) to exclude uninformative
  spurious edges, and 2) to further suppress the occurrence of spurious edges. Through
  theoretical analysis and extensive experiments, we show that PrunE achieves superior
  OOD performance and outperforms previous state-of-the-art methods significantly.
  Codes are available at: https://github.com/tianyao-aka/PrunE-GraphOOD.'
codebase_url: https://github.com/tianyao-aka/PrunE-GraphOOD
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PrunE
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
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
  dataset: ogbg-molpcba
  rows:
  - model: PrunE
    model_key: prune
    model_plain: PrunE
    value: 0.8159
    std: 0.0535
    paper_value: 0.8159
    paper_std: 0.0535
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8159
    true_std: 0.0535
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8159
    sort_std: 0.0535
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
  - model: UGTs
    model_key: egtas
    model_plain: UGTs
    value: 0.7919
    std: 0.0137
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.19779'
    title: Automatic Graph Topology-Aware Transformer
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: https://github.com/xiaofangxd/EGTAS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7919
    sort_std: 0.0137
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: UGTs
    model_key: ugts
    model_plain: UGTs
    value: 0.784
    std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.15335'
    title: 'You Can Have Better Graph Neural Networks by Not Training Weights at All:
      Finding Untrained GNNs Tickets'
    date: Nov 28, 2022
    date_display: Nov 2022
    date_iso: '2022-11-28'
    venue: Learning on Graphs Conference
    codebase_url: https://github.com/TianjinYellow/UGTs-LoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.784
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.6649
    std: 0.0155
    paper_value: 0.6649
    paper_std: 0.0155
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7531
    at_pub_std: 0.0457
    at_pub_source_arxiv: '2306.15963'
    at_pub_source_title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
    at_pub_source_date_iso: '2023-06-28'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-28'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.08819999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7531
    true_std: 0.0457
    value_gap_source_arxiv: '2306.15963'
    value_gap_source_title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
    value_gap_source_is_current_paper: false
    value_gap: 0.08819999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7531
    sort_std: 0.0457
    global_rank: 9
    paper_rank: 29
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fused Gromov-Wasserstein Graph Mixup for Graph-level
      Classifications
    comparison_source_arxiv: '2306.15963'
    is_best: true
    is_std_outlier: false
  - model: G-Mixup
    model_key: g-mixup
    model_plain: G-Mixup
    value: 0.6744
    std: 0.0162
    paper_value: 0.6744
    paper_std: 0.0162
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7374
    at_pub_std: 0.0707
    at_pub_source_arxiv: '2306.15963'
    at_pub_source_title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
    at_pub_source_date_iso: '2023-06-28'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-28'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.06300000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7374
    true_std: 0.0707
    value_gap_source_arxiv: '2306.15963'
    value_gap_source_title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
    value_gap_source_is_current_paper: false
    value_gap: 0.06300000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7374
    sort_std: 0.0707
    global_rank: 10
    paper_rank: 23
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AIA
    model_key: aia
    model_plain: AIA
    value: 0.7079
    std: 0.0153
    paper_value: 0.7079
    paper_std: 0.0153
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7079
    true_std: 0.0153
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7079
    sort_std: 0.0153
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
  - model: GREA
    model_key: grea
    model_plain: GREA
    value: 0.6972
    std: 0.0166
    paper_value: 0.6972
    paper_std: 0.0166
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6972
    true_std: 0.0166
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6972
    sort_std: 0.0166
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
  - model: VREx
    model_key: vrex
    model_plain: VREx
    value: 0.6874
    std: 0.0103
    paper_value: 0.6874
    paper_std: 0.0103
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
    table_ref: Table 1
    source_ref: gui2022good
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6874
    true_std: 0.0103
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6874
    sort_std: 0.0103
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LiSA
    model_key: lisa
    model_plain: LiSA
    value: 0.6811
    std: 0.0052
    paper_value: 0.6811
    paper_std: 0.0052
    metric: ROC-AUC
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6811
    true_std: 0.0052
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6811
    sort_std: 0.0052
    global_rank: 20
    paper_rank: 20
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
    value: 0.681
    std: 0.0168
    paper_value: 0.681
    paper_std: 0.0168
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
    table_ref: Table 1
    source_ref: gui2022good
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.681
    true_std: 0.0168
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.681
    sort_std: 0.0168
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cal
    model_key: cal
    model_plain: Cal
    value: 0.6806
    std: 0.026
    paper_value: 0.6806
    paper_std: 0.026
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6806
    true_std: 0.026
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6806
    sort_std: 0.026
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
  - model: FLAG
    model_key: flag
    model_plain: FLAG
    value: 0.6769
    std: 0.0236
    paper_value: 0.6769
    paper_std: 0.0236
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6769
    true_std: 0.0236
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6769
    sort_std: 0.0236
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
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.6722
    std: 0.0115
    paper_value: 0.6722
    paper_std: 0.0115
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
    table_ref: Table 1
    source_ref: gui2022good
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6722
    true_std: 0.0115
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6722
    sort_std: 0.0115
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
  - model: DisC
    model_key: disc
    model_plain: DisC
    value: 0.6712
    std: 0.0211
    paper_value: 0.6712
    paper_std: 0.0211
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6712
    true_std: 0.0211
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6712
    sort_std: 0.0211
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
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.6686
    std: 0.0225
    paper_value: 0.6686
    paper_std: 0.0225
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6686
    true_std: 0.0225
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6686
    sort_std: 0.0225
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
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.6678
    std: 0.0145
    paper_value: 0.6678
    paper_std: 0.0145
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6678
    true_std: 0.0145
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6678
    sort_std: 0.0145
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
  - model: GroupDRO
    model_key: groupdro
    model_plain: GroupDRO
    value: 0.6647
    std: 0.0239
    paper_value: 0.6647
    paper_std: 0.0239
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
    table_ref: Table 1
    source_ref: gui2022good
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6647
    true_std: 0.0239
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6647
    sort_std: 0.0239
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
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.6492
    std: 0.0209
    paper_value: 0.6492
    paper_std: 0.0209
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
    table_ref: Table 1
    source_ref: sui2023unleashing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molpcba (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB split for OGBG-Molbbbp
    date: Jun 6, 2025
    date_display: Jun 2025
    date_iso: '2025-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6492
    true_std: 0.0209
    value_gap_source_arxiv: '2506.05957'
    value_gap_source_title: Pruning Spurious Subgraphs for Graph Out-of-Distribution
      Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6492
    sort_std: 0.0209
    global_rank: 32
    paper_rank: 32
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
  dataset_primary_metric: AP
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: ogbg-molpcba
      dataset_slug: ogbg-molpcba
single_proposed_model: PrunE
main_figure: /figures/2506.05957/main_figure.jpegoptim.jpg
---

