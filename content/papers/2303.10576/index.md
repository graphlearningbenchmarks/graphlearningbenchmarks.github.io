---
title: An Efficient Subgraph GNN with Provable Substructure Counting Power
arxiv_id: '2303.10576'
source_url: ''
authors:
- name: Zuoyu Yan
  orcid: null
  s2_author_id: '2783105'
  s2_url: null
- name: Junru Zhou
  orcid: null
  s2_author_id: '30887404'
  s2_url: null
- name: Liangcai Gao
  orcid: null
  s2_author_id: '2165982472'
  s2_url: null
- name: Zhi Tang
  orcid: null
  s2_author_id: '143830636'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '1390814008'
  s2_url: null
published_date: Mar 19, 2023
published_date_iso: '2023-03-19'
published_venue: KDD 2023
published_conference: KDD 2023
published_conference_short: KDD
published_conference_slug: kdd
abstract: 'We investigate the enhancement of graph neural networks'' (GNNs) representation
  power through their ability in substructure counting. Recent advances have seen
  the adoption of subgraph GNNs, which partition an input graph into numerous subgraphs,
  subsequently applying GNNs to each to augment the graph''s overall representation.
  Despite their ability to identify various substructures, subgraph GNNs are hindered
  by significant computational and memory costs. In this paper, we tackle a critical
  question: Is it possible for GNNs to count substructures both efficiently and provably?
  Our approach begins with a theoretical demonstration that the distance to rooted
  nodes in subgraphs is key to boosting the counting power of subgraph GNNs. To avoid
  the need for repetitively applying GNN across all subgraphs, we introduce precomputed
  structural embeddings that encapsulate this crucial distance information. Experiments
  validate that our proposed model retains the counting power of subgraph GNNs while
  achieving significantly faster performance.'
codebase_url: https://github.com/pkuyzy/ESC-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ESC-GNN
mrr: 0.0333
adjusted_mrr: 0.0222
mrr_dataset_count: 2
benchmark_categories:
- OGB
- GNNBenchmark
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: CSL
  rows:
  - model: ESC-GNN
    model_key: esc-gnn
    model_plain: ESC-GNN
    value: 1.0
    std: null
    paper_value: 1.0
    paper_std: null
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on synthetic CSL dataset
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-30'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: null
    value_gap_source_arxiv: '2501.18739'
    value_gap_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: null
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: I^2-GNN
    model_key: i^2-gnn
    model_plain: I^2-GNN
    value: 1.0
    std: null
    paper_value: 1.0
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on synthetic CSL dataset
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: null
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: null
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PPGN
    model_key: ppgn
    model_plain: PPGN
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RW-AgentNet
    model_key: rw-agentnet
    model_plain: RW-AgentNet
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AgentNet
    model_key: agentnet
    model_plain: AgentNet
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 1.0
    std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Node Positional Encoding with Laplacian Eigenvectors
    is_global_top: true
    global_rank: 9
    sort_value: 1.0
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 3-GNN
    model_key: 3-gnn
    model_plain: 3-GNN
    value: 0.957
    std: null
    paper_value: 0.957
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on synthetic CSL dataset
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-30'
    value_gap_source_date_label: ICML 2025
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
    value_gap_source_arxiv: '2501.18739'
    value_gap_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.957
    sort_std: null
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
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.1
    std: null
    paper_value: 0.1
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on synthetic CSL dataset
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1
    sort_std: null
    global_rank: 80
    paper_rank: 80
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
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.8094
    std: 0.0057
    paper_value: 0.8094
    paper_std: 0.0057
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
    source_ref: bodnar2021weisfeiler1
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.8094
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2210.13978'
    at_pub_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    at_pub_source_date_iso: '2022-10-22'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8094
    true_std: 0.006
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8094
    sort_std: 0.006
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
    value: 0.7799
    std: 0.0001
    paper_value: 0.7799
    paper_std: 0.0001
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
    source_ref: bouritsas2022improving
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.8039
    at_pub_std: 0.009
    at_pub_source_arxiv: '2210.13978'
    at_pub_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    at_pub_source_date_iso: '2022-10-22'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-04-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.02399999999999991
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
    value_gap: 0.02399999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8039
    sort_std: 0.009
    global_rank: 22
    paper_rank: 112
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    comparison_source_arxiv: '2210.13978'
    is_best: false
    is_std_outlier: false
  - model: SUN
    model_key: sun
    model_plain: SUN
    value: 0.8003
    std: 0.0055
    paper_value: 0.8003
    paper_std: 0.0055
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
    source_ref: frascaunderstanding2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.8003
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2302.07090'
    at_pub_source_title: A Complete Expressiveness Hierarchy for Subgraph GNNs via
      Subgraph Weisfeiler-Lehman Tests
    at_pub_source_date_iso: '2023-02-14'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-29'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8003
    true_std: 0.0055
    value_gap_source_arxiv: '2310.19142'
    value_gap_source_title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8003
    sort_std: 0.0055
    global_rank: 35
    paper_rank: 35
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.797
    std: 0.0097
    paper_value: 0.797
    paper_std: 0.0097
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
    source_ref: beaini2021directional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.797
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.797
    true_std: 0.0097
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.0097
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
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.7961
    std: 0.0119
    paper_value: 0.7961
    paper_std: 0.0119
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
    source_ref: zhao2022stars
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.7822
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2210.02636'
    at_pub_source_title: Geodesic Graph Neural Network for Efficient Graph Representation
      Learning
    at_pub_source_date_iso: '2022-10-06'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.013900000000000023
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7961
    true_std: 0.0119
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7961
    sort_std: 0.0119
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ESC-GNN
    model_key: esc-gnn
    model_plain: ESC-GNN
    value: 0.7921
    std: 0.0084
    paper_value: 0.7921
    paper_std: 0.0084
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7921
    true_std: 0.0084
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7921
    sort_std: 0.0084
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.7905
    std: 0.0132
    paper_value: 0.7905
    paper_std: 0.0132
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.7905
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-04-19'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7905
    true_std: 0.0132
    value_gap_source_arxiv: '2604.17324'
    value_gap_source_title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers
      via Sigmoid-Gated Attention'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7905
    sort_std: 0.0132
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
  - model: I^2-GNN
    model_key: i^2-gnn
    model_plain: I^2-GNN
    value: 0.7868
    std: 0.0093
    paper_value: 0.7868
    paper_std: 0.0093
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
    source_ref: huang2023boosting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-08'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7868
    true_std: 0.0093
    value_gap_source_arxiv: '2305.04963'
    value_gap_source_title: 'From Relational Pooling to Subgraph GNNs: A Universal
      Framework for More Expressive Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7868
    sort_std: 0.0093
    global_rank: 81
    paper_rank: 81
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PL-GNN
    model_key: pl-gnn
    model_plain: PL-GNN
    value: 0.7849
    std: 0.0101
    paper_value: 0.7849
    paper_std: 0.0101
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
    source_ref: bevilacqua2024efficient
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7849
    true_std: 0.0101
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7849
    sort_std: 0.0101
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NGNN
    model_key: ngnn
    model_plain: NGNN
    value: 0.7834
    std: 0.0186
    paper_value: 0.7834
    paper_std: 0.0186
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
    source_ref: zhang2021nested
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-29'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7834
    true_std: 0.0186
    value_gap_source_arxiv: '2310.19142'
    value_gap_source_title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural
      Network'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7834
    sort_std: 0.0186
    global_rank: 94
    paper_rank: 94
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OSAN
    model_key: osan
    model_plain: OSAN
    value: 0.7801
    std: 0.0104
    paper_value: 0.7801
    paper_std: 0.0104
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
    source_ref: qianordered2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7801
    true_std: 0.0104
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7801
    sort_std: 0.0104
    global_rank: 111
    paper_rank: 111
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
    value: 0.7707
    std: 0.0149
    paper_value: 0.7707
    paper_std: 0.0149
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
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.778
    at_pub_std: 0.0182
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.007299999999999973
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.0182
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.007299999999999973
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0182
    global_rank: 120
    paper_rank: 163
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphtransformer
    model_key: graphtransformer
    model_plain: Graphtransformer
    value: 0.774
    std: 0.0177
    paper_value: 0.774
    paper_std: 0.0177
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
    table_ref: Table 1
    source_ref: rampavsek2022recipe
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.774
    true_std: 0.0177
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.774
    sort_std: 0.0177
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.769
    std: 0.0136
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_display: Oct 2021
    date_iso: '2021-10-14'
    venue: null
    codebase_url: https://github.com/yuehaowang/SoGCN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 172
    sort_value: 0.769
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSS-GNN
    model_key: dss-gnn
    model_plain: DSS-GNN
    value: 0.7678
    std: 0.0166
    paper_value: 0.7678
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
    source_ref: bevilacqua2022equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB scaffold split for HIV classification task.
    date: Mar 19, 2023
    date_display: Mar 2023
    date_iso: '2023-03-19'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-19'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7678
    true_std: 0.0166
    value_gap_source_arxiv: '2303.10576'
    value_gap_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7678
    sort_std: 0.0166
    global_rank: 180
    paper_rank: 180
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
- benchmark: GNNBenchmark
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CSL
      dataset_slug: csl
single_proposed_model: ESC-GNN
main_figure: /figures/2303.10576/main_figure.jpegoptim.jpg
---

