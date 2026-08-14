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
mrr: 0.0244
adjusted_mrr: 0.0081
mrr_dataset_count: 1
benchmark_categories:
- Heterophily Benchmark
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 1
  total: 5
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
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    comparison_source_arxiv: '2506.15448'
    is_best: true
    is_std_outlier: false
  - model: GGAD
    model_key: ggad
    model_plain: GGAD
    value: 0.9443
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
    arxiv_id: '2506.15448'
    title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
    date: Jun 18, 2025
    date_display: Jun 2025
    date_iso: '2025-06-18'
    venue: Accepted at NeurIPS 2025
    codebase_url: https://github.com/mala-lab/RHO
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9443
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    true_value: 0.918
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.01
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
    true_value: 0.91
    true_std: 0.01
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.91
    sort_std: 0.01
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
    at_pub_value: 0.8312
    at_pub_std: null
    at_pub_source_arxiv: '2506.15448'
    at_pub_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    at_pub_source_date_iso: '2025-06-18'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05379999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
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
    global_rank: 15
    paper_rank: 15
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
    global_rank: 18
    paper_rank: 18
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
    at_pub_value: 0.7345
    at_pub_std: null
    at_pub_source_arxiv: '2506.15448'
    at_pub_source_title: Semi-supervised Graph Anomaly Detection via Robust Homophily
      Learning
    at_pub_source_date_iso: '2025-06-18'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2026-04-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08749999999999991
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.0
    value_gap_source_arxiv: '2605.11749'
    value_gap_source_title: Learning Feature Encoder with Synthetic Anomalies for
      Weakly Supervised Graph Anomaly Detection
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.0
    global_rank: 21
    paper_rank: 21
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
  - model: UniGAP
    model_key: unigap
    model_plain: UniGAP
    value: 0.8421
    std: 0.008
    metric: ROC-AUC
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
    sort_value: 0.8421
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN + AdaEdge
    model_key: h2gcn + adaedge
    model_plain: H2GCN + AdaEdge
    value: 0.8134
    std: 0.007
    metric: ROC-AUC
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
    sort_value: 0.8134
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN +AdaEdge
    model_key: gcn +adaedge
    model_plain: GCN +AdaEdge
    value: 0.8085
    std: 0.008
    metric: ROC-AUC
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
    sort_value: 0.8085
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
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
    at_pub_value: 0.7902
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.31720000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7902
    true_std: 0.006
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.31720000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7902
    sort_std: 0.006
    global_rank: 12
    paper_rank: 160
    rank_delta: 148
    rank_delta_abs: 148
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
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
    at_pub_value: 0.7743
    at_pub_std: 0.012
    at_pub_source_arxiv: '2403.12529'
    at_pub_source_title: Contextualized Messages Boost Graph Representations
    at_pub_source_date_iso: '2024-03-19'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1703
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7743
    true_std: 0.012
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: 0.1703
    has_value_note: false
    value_note: ''
    sort_value: 0.7743
    sort_std: 0.012
    global_rank: 33
    paper_rank: 132
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Contextualized Messages Boost Graph Representations
    comparison_source_arxiv: '2403.12529'
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
    at_pub_value: 0.7721
    at_pub_std: 0.013
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2701
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7721
    true_std: 0.013
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.2701
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: 0.013
    global_rank: 41
    paper_rank: 159
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7644
    std: 0.0062
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: null
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 51
    sort_value: 0.7644
    sort_std: 0.0062
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
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
    at_pub_value: 0.7082
    at_pub_std: 0.001
    at_pub_source_arxiv: '2508.17531'
    at_pub_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    at_pub_source_date_iso: '2025-08-24'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.09920000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7082
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.09920000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.7082
    sort_std: 0.001
    global_rank: 91
    paper_rank: 131
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    comparison_source_arxiv: '2508.17531'
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
    global_rank: 100
    paper_rank: 128
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    comparison_source_arxiv: '2312.17679'
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
    at_pub_value: 0.6947
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.0837
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6947
    true_std: null
    value_gap_source_arxiv: '2312.17679'
    value_gap_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0837
    has_value_note: false
    value_note: ''
    sort_value: 0.6947
    sort_std: null
    global_rank: 105
    paper_rank: 131
    rank_delta: 26
    rank_delta_abs: 26
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
    global_rank: 109
    paper_rank: 138
    rank_delta: 29
    rank_delta_abs: 29
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
    global_rank: 110
    paper_rank: 132
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
    at_pub_value: 0.6776
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.08860000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6776
    true_std: null
    value_gap_source_arxiv: '2312.17679'
    value_gap_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    value_gap_source_is_current_paper: false
    value_gap: 0.08860000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.6776
    sort_std: null
    global_rank: 114
    paper_rank: 136
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
    global_rank: 127
    paper_rank: 127
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
    global_rank: 132
    paper_rank: 132
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
    global_rank: 134
    paper_rank: 134
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
    global_rank: 141
    paper_rank: 141
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
- benchmark: Heterophily Benchmark
  datasets:
  - *id001
- benchmark: Other Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Questions
      dataset_slug: questions
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
main_figure: /figures/2605.11749/main_figure.jpegoptim.jpg
---

