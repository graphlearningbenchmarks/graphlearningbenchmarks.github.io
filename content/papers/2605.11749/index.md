---
title: Learning Feature Encoder with Synthetic Anomalies for Weakly Supervised Graph
  Anomaly Detection
arxiv_id: '2605.11749'
source_url: ''
authors:
- name: Yingjie Zhou
  orcid: null
  s2_author_id: '2336860881'
  s2_url: null
- name: Yuqin Xie
  orcid: null
  s2_author_id: '2357060175'
  s2_url: null
- name: Fanxing Liu
  orcid: null
  s2_author_id: '1752776622'
  s2_url: null
- name: Dongjin Song
  orcid: null
  s2_author_id: '2276324326'
  s2_url: null
- name: Ce Zhu
  orcid: null
  s2_author_id: '2240554014'
  s2_url: null
- name: Lingqiao Liu
  orcid: null
  s2_author_id: '2382732818'
  s2_url: null
published_date: Apr 1, 2026
published_date_iso: '2026-04-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Weakly supervised graph anomaly detection aims to unveil unusual graph instances,
  e.g., nodes, whose behaviors are significantly different from the normal ones, under
  the condition that only a limited number of annotated anomalies but abundant unlabeled
  samples are available. A major challenge for this task is to learn a meaningful
  latent feature representation that reduces intra-class variance among normal data
  while remaining highly sensitive to anomalies. Although recent works have applied
  self-supervised feature learning methods for graph anomaly detection, their strategies
  are not specifically tailored to the unique requirements of graph anomaly detection,
  which motivates our exploration of a more domain-specific feature learning approach.
  In this paper, we introduce a weakly supervised graph anomaly detection method that
  leverages a feature learning strategy specifically tailored for graph anomalies.
  Our approach is built upon a multi-task learning scheme designed to extract robust
  feature representations, through synthesized anomalies. We generate these synthetic
  anomalies by perturbing the normal graph in various ways and assign a dedicated
  detection head to each anomaly type. This design ensures that the learned features
  are sensitive to potential deviations from normal patterns. Although synthetic anomalies
  may not perfectly replicate real-world patterns, they provide valuable auxiliary
  data for effective feature learning—much like the way features learned from classifying
  ImageNet images are used in various downstream computer vision tasks. Additionally,
  we adopt a two-phase learning strategy to balance the influence of synthetic anomalies
  and real data. The process begins with an initial warm-up phase using only synthetic
  samples, followed by a full-training phase that integrates both tasks. Numerous
  experiments on public datasets demonstrate the superior performance of our proposed
  strategy, in comparison with those of its competitors. Code is available at.
codebase_url: https://github.com/yj-zhou/SAWGAD
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphSAGE
- weakly supervised graph anomaly detection method
mrr: 0.0345
adjusted_mrr: 0.0115
mrr_dataset_count: 1
benchmark_categories:
- Heterophilic Graphs
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 13
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Amazon2M
  rows:
  - model: weakly supervised graph anomaly detection method
    model_key: unigad - bwg
    model_plain: weakly supervised graph anomaly detection method
    value: 0.9784
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_display: Nov 2024
    date_iso: '2024-11-10'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/lllyyq1121/UniGAD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9784
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.885
    std: 0.02
    paper_value: 0.885
    paper_std: 0.02
    metric: AUROC
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
    source_ref: tang2022bwgnn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.978
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.09299999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.978
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.09299999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.978
    sort_std: null
    global_rank: 2
    paper_rank: 18
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: true
    is_std_outlier: false
  - model: weakly supervised graph anomaly detection method
    model_key: amnet
    model_plain: weakly supervised graph anomaly detection method
    value: 0.9731
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_display: Nov 2024
    date_iso: '2024-11-10'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/lllyyq1121/UniGAD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9731
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: weakly supervised graph anomaly detection method
    model_key: weakly supervised graph anomaly detection method
    model_plain: weakly supervised graph anomaly detection method
    value: 0.969
    std: 0.01
    paper_value: 0.969
    paper_std: 0.01
    metric: AUROC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset; uses synthetic
      anomalies for feature learning
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.969
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.969
    sort_std: 0.01
    global_rank: 4
    paper_rank: 4
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
    value: 0.918
    std: 0.01
    paper_value: 0.918
    paper_std: 0.01
    metric: AUROC
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
    source_ref: veličković2018gat
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9624
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.044399999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9624
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.044399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9624
    sort_std: null
    global_rank: 6
    paper_rank: 11
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: ConsisGAD
    model_key: consisgad
    model_plain: ConsisGAD
    value: 0.952
    std: 0.01
    paper_value: 0.952
    paper_std: 0.01
    metric: AUROC
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
    source_ref: chen2024consisgad
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8715
    at_pub_std: null
    at_pub_source_arxiv: '2506.15448'
    at_pub_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    at_pub_source_date_iso: '2025-06-18'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0804999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.952
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.01
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    comparison_source_arxiv: '2506.15448'
    is_best: false
    is_std_outlier: false
  - model: GATSep
    model_key: gatsep
    model_plain: GATSep
    value: 0.937
    std: 0.01
    paper_value: 0.937
    paper_std: 0.01
    metric: AUROC
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
    source_ref: platonov2023gatsep
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.937
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: 0.01
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.91
    std: 0.01
    paper_value: 0.91
    paper_std: 0.01
    metric: AUROC
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
    source_ref: xu2018gin
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9217
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.011699999999999933
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9217
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.011699999999999933
    has_value_note: false
    value_note: ''
    sort_value: 0.9217
    sort_std: null
    global_rank: 11
    paper_rank: 12
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: CGNN
    model_key: cgnn
    model_plain: CGNN
    value: 0.909
    std: 0.02
    paper_value: 0.909
    paper_std: 0.02
    metric: AUROC
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
    source_ref: li2025cgnn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.909
    true_std: 0.02
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.909
    sort_std: 0.02
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PCGNN
    model_key: pcgnn
    model_plain: PCGNN
    value: 0.907
    std: 0.01
    paper_value: 0.907
    paper_std: 0.01
    metric: AUROC
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
    source_ref: liu2021pcgnn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.907
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.907
    sort_std: 0.01
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.903
    std: 0.01
    paper_value: 0.903
    paper_std: 0.01
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.01
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
  - model: CAREGNN
    model_key: caregnn
    model_plain: CAREGNN
    value: 0.899
    std: 0.01
    paper_value: 0.899
    paper_std: 0.01
    metric: AUROC
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
    source_ref: dou2020caregnn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.899
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.899
    sort_std: 0.01
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.894
    std: 0.01
    paper_value: 0.894
    paper_std: 0.01
    metric: AUROC
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
    source_ref: hamilton2017graphsage
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8453
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.048699999999999966
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.01
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: GHRN
    model_key: ghrn
    model_plain: GHRN
    value: 0.885
    std: 0.02
    paper_value: 0.885
    paper_std: 0.02
    metric: AUROC
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
    source_ref: gao2023ghrn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.885
    true_std: 0.02
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.885
    sort_std: 0.02
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
  - model: H2FD
    model_key: h2fd
    model_plain: H2FD
    value: 0.87
    std: 0.01
    paper_value: 0.87
    paper_std: 0.01
    metric: AUROC
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
    source_ref: shi2022h2
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.87
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.87
    sort_std: 0.01
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.822
    std: 0.0
    paper_value: 0.822
    paper_std: 0.0
    metric: AUROC
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
    source_ref: kipf2017gcn
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard anomaly detection task on Amazon dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8237
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0017000000000000348
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8237
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.0017000000000000348
    has_value_note: false
    value_note: ''
    sort_value: 0.8237
    sort_std: null
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Questions
  rows:
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.609
    std: 0.03
    paper_value: 0.609
    paper_std: 0.03
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9733
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.36430000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9733
    true_std: 0.0006
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.36430000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9733
    sort_std: 0.0006
    global_rank: 1
    paper_rank: 119
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: true
    is_std_outlier: false
  - model: topk
    model_key: ags-gnn
    model_plain: topk
    value: 0.9727
    std: 0.0004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9727
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.473
    std: 0.08
    paper_value: 0.473
    paper_std: 0.08
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
    source_ref: kipf2017gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9715
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.49850000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9715
    true_std: 0.0004
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.49850000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9715
    sort_std: 0.0004
    global_rank: 3
    paper_rank: 148
    rank_delta: 145
    rank_delta_abs: 145
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.604
    std: 0.02
    paper_value: 0.604
    paper_std: 0.02
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
    source_ref: veličković2018gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9711
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.3671
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9711
    true_std: 0.0002
    value_gap_source_arxiv: '2405.20445'
    value_gap_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.3671
    has_value_note: false
    value_note: ''
    sort_value: 0.9711
    sort_std: 0.0002
    global_rank: 4
    paper_rank: 120
    rank_delta: 116
    rank_delta_abs: 116
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.611
    std: 0.03
    paper_value: 0.611
    paper_std: 0.03
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
    source_ref: tang2022bwgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9603
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.34930000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9603
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.34930000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9603
    sort_std: null
    global_rank: 8
    paper_rank: 119
    rank_delta: 111
    rank_delta_abs: 111
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.589
    std: 0.04
    paper_value: 0.589
    paper_std: 0.04
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
    source_ref: xu2018gin
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8643
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.2753
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8643
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.2753
    has_value_note: false
    value_note: ''
    sort_value: 0.8643
    sort_std: null
    global_rank: 11
    paper_rank: 123
    rank_delta: 112
    rank_delta_abs: 112
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.502
    std: 0.09
    paper_value: 0.502
    paper_std: 0.09
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
    source_ref: hamilton2017graphsage
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7816
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.27959999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7816
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.27959999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7816
    sort_std: null
    global_rank: 29
    paper_rank: 147
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: GATSep
    model_key: gatsep
    model_plain: GATSep
    value: 0.631
    std: 0.01
    paper_value: 0.631
    paper_std: 0.01
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
    source_ref: platonov2023gatsep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6996
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.0686
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6996
    true_std: null
    value_gap_source_arxiv: '2312.17679'
    value_gap_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0686
    has_value_note: false
    value_note: ''
    sort_value: 0.6996
    sort_std: null
    global_rank: 101
    paper_rank: 117
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    comparison_source_arxiv: '2312.17679'
    is_best: false
    is_std_outlier: false
  - model: PCGNN
    model_key: pcgnn
    model_plain: PCGNN
    value: 0.576
    std: 0.02
    paper_value: 0.576
    paper_std: 0.02
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
    source_ref: liu2021pcgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6838
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.1078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6838
    true_std: null
    value_gap_source_arxiv: '2312.17679'
    value_gap_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    value_gap_source_is_current_paper: false
    value_gap: 0.1078
    has_value_note: false
    value_note: ''
    sort_value: 0.6838
    sort_std: null
    global_rank: 103
    paper_rank: 125
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    comparison_source_arxiv: '2312.17679'
    is_best: false
    is_std_outlier: false
  - model: GHRN
    model_key: ghrn
    model_plain: GHRN
    value: 0.605
    std: 0.02
    paper_value: 0.605
    paper_std: 0.02
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
    source_ref: gao2023ghrn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6824
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.07740000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6824
    true_std: null
    value_gap_source_arxiv: '2312.17679'
    value_gap_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    value_gap_source_is_current_paper: false
    value_gap: 0.07740000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6824
    sort_std: null
    global_rank: 104
    paper_rank: 120
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    comparison_source_arxiv: '2312.17679'
    is_best: false
    is_std_outlier: false
  - model: weakly supervised graph anomaly detection method
    model_key: weakly supervised graph anomaly detection method
    model_plain: weakly supervised graph anomaly detection method
    value: 0.657
    std: 0.02
    paper_value: 0.657
    paper_std: 0.02
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset. Uses synthetic anomalies as auxiliary data.
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.657
    true_std: 0.02
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.02
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConsisGAD
    model_key: consisgad
    model_plain: ConsisGAD
    value: 0.638
    std: 0.06
    paper_value: 0.638
    paper_std: 0.06
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
    source_ref: chen2024consisgad
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5737
    at_pub_std: null
    at_pub_source_arxiv: '2506.15448'
    at_pub_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    at_pub_source_date_iso: '2025-06-18'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.06430000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.638
    true_std: 0.06
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.638
    sort_std: 0.06
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    comparison_source_arxiv: '2506.15448'
    is_best: false
    is_std_outlier: false
  - model: CAREGNN
    model_key: caregnn
    model_plain: CAREGNN
    value: 0.606
    std: 0.01
    paper_value: 0.606
    paper_std: 0.01
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
    source_ref: dou2020caregnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.606
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.606
    sort_std: 0.01
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGNN
    model_key: cgnn
    model_plain: CGNN
    value: 0.595
    std: 0.06
    paper_value: 0.595
    paper_std: 0.06
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
    source_ref: li2025cgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.595
    true_std: 0.06
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.595
    sort_std: 0.06
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
  - model: H2FD
    model_key: h2fd
    model_plain: H2FD
    value: 0.565
    std: 0.01
    paper_value: 0.565
    paper_std: 0.01
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
    source_ref: shi2022h2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification for anomaly detection on Questions
      dataset
    date: Apr 1, 2026
    date_display: Apr 2026
    date_iso: '2026-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.565
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.565
    sort_std: 0.01
    global_rank: 128
    paper_rank: 128
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
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: Other Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Questions
      dataset_slug: questions
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
---

