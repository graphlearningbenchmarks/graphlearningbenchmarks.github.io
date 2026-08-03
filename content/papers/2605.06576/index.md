---
title: On the Safety of Graph Representation Learning
arxiv_id: '2605.06576'
source_url: ''
authors:
- name: Xiaoguang Guo
  orcid: null
  s2_author_id: '2408379349'
  s2_url: null
- name: Zehong Wang
  orcid: null
  s2_author_id: '2284578810'
  s2_url: null
- name: Ziming Li
  orcid: null
  s2_author_id: '2258698077'
  s2_url: null
- name: Shawn Spitzel
  orcid: null
  s2_author_id: '2409928317'
  s2_url: null
- name: S. Kwon
  orcid: null
  s2_author_id: '2223120839'
  s2_url: null
- name: Tianyi Ma
  orcid: null
  s2_author_id: '2283516218'
  s2_url: null
- name: Yanfang Ye
  orcid: null
  s2_author_id: '2093920413'
  s2_url: null
- name: Chuxu Zhang
  orcid: null
  s2_author_id: '2117879943'
  s2_url: null
published_date: May 7, 2026
published_date_iso: '2026-05-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph representation learning (GRL) has evolved from topology-only graph
  embeddings to task-specific supervised GNNs, and more recently to reusable representations
  and graph foundation models (GFMs). However, existing evaluations mainly measure
  clean transfer, adaptation, and task coverage. It remains unclear whether GRL methods
  stay reliable when deployment stresses affect graph signals, graph contexts, label
  support, structural groups, or predictive evidence. We introduce GRL-Safety, a multi-axis
  safety evaluation benchmark for GRL. GRL-Safety evaluates twelve representative
  methods, spanning topology-only embedding methods, supervised GNNs, self-supervised
  graph models, and GFMs, on twenty-five graph datasets under standardized evaluation
  conditions while preserving method-native adaptation. The evaluation covers five
  safety axes: corruption robustness, OOD generalization, class imbalance, fairness,
  and interpretation, with per-axis and subcondition reporting rather than a single
  aggregate score. Our analysis yields three cross-axis insights that can inspire
  future research. First, safety behavior is shaped by the interaction between representation
  design and the stressed graph factor, rather than by method family alone. Second,
  foundation-era methods show axis-specific strengths rather than broad safety dominance.
  Third, several deployment regimes remain difficult even for the best evaluated method,
  revealing capability gaps that require new robustness, adaptation, or training objectives
  beyond model selection. The benchmark, evaluation protocols, and code are available
  at:.'
codebase_url: https://github.com/GXG-CS/GRL-Safety
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Heterophilic Graphs
- Knowledge Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 13
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
- node_classification
experiment_scopes:
- edge-level
- node-level
results:
- &id001
  dataset: Tolokers
  rows:
  - model: topk
    model_key: polynormer-r
    model_plain: topk
    value: 0.8591
    std: 0.0074
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8591
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: topk
    model_key: dc-gnn
    model_plain: topk
    value: 0.8588
    std: 0.0081
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16185'
    title: Differentiable Cluster Graph Neural Network
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8588
    sort_std: 0.0081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: topk
    model_key: polynormer + wideformer
    model_plain: topk
    value: 0.8533
    std: 0.0023
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8533
    sort_std: 0.0023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7001
    std: 0.0227
    paper_value: 0.7001
    paper_std: 0.0227
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8443
    at_pub_std: 0.01
    at_pub_source_arxiv: '2406.06642'
    at_pub_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    at_pub_source_date_iso: '2024-06-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1442000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8443
    true_std: 0.01
    value_gap_source_arxiv: '2406.06642'
    value_gap_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.1442000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8443
    sort_std: 0.01
    global_rank: 10
    paper_rank: 115
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TopoBench: A Framework for Benchmarking Topological
      Deep Learning'
    comparison_source_arxiv: '2406.06642'
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7478
    std: 0.0031
    paper_value: 0.7478
    paper_std: 0.0031
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8364
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.08860000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8364
    true_std: 0.0067
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.08860000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8364
    sort_std: 0.0067
    global_rank: 28
    paper_rank: 99
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7559
    std: 0.0045
    paper_value: 0.7559
    paper_std: 0.0045
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8243
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06840000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8243
    true_std: 0.0044
    value_gap_source_arxiv: '2202.07082'
    value_gap_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.06840000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8243
    sort_std: 0.0044
    global_rank: 55
    paper_rank: 99
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.8041
    std: 0.0036
    paper_value: 0.8041
    paper_std: 0.0036
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8041
    true_std: 0.0036
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8041
    sort_std: 0.0036
    global_rank: 74
    paper_rank: 74
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIT
    model_key: git
    model_plain: GIT
    value: 0.7666
    std: 0.0044
    paper_value: 0.7666
    paper_std: 0.0044
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7666
    true_std: 0.0044
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7666
    sort_std: 0.0044
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GFT
    model_key: gft
    model_plain: GFT
    value: 0.7242
    std: 0.0061
    paper_value: 0.7242
    paper_std: 0.0061
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7242
    true_std: 0.0061
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7242
    sort_std: 0.0061
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGraph2
    model_key: unigraph2
    model_plain: UniGraph2
    value: 0.6934
    std: 0.052
    paper_value: 0.6934
    paper_std: 0.052
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6934
    true_std: 0.052
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6934
    sort_std: 0.052
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.689
    std: 0.0346
    paper_value: 0.689
    paper_std: 0.0346
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Demographic fairness evaluation on tolokers (banned-user prediction)
      using Test AUC.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.689
    true_std: 0.0346
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.0346
    global_rank: 118
    paper_rank: 118
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
- &id002
  dataset: WN18RR
  rows:
  - model: GFT
    model_key: gft
    model_plain: GFT
    value: 0.157
    std: 0.005
    paper_value: 0.157
    paper_std: 0.005
    metric: MRR
    higher_is_better: true
    is_baseline: true
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
    source_ref: wang2024gft
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9191
    at_pub_std: null
    at_pub_source_arxiv: '2411.06070'
    at_pub_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    at_pub_source_date_iso: '2024-11-09'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.7621
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9191
    true_std: null
    value_gap_source_arxiv: '2411.06070'
    value_gap_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    value_gap_source_is_current_paper: false
    value_gap: 0.7621
    has_value_note: false
    value_note: ''
    sort_value: 0.9191
    sort_std: null
    global_rank: 1
    paper_rank: 82
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    comparison_source_arxiv: '2411.06070'
    is_best: true
    is_std_outlier: false
  - model: UniGraph2
    model_key: unigraph2
    model_plain: UniGraph2
    value: 0.148
    std: 0.007
    paper_value: 0.148
    paper_std: 0.007
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: he2025unigraph2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8786
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2502.00806'
    at_pub_source_title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal
      Graphs'
    at_pub_source_date_iso: '2025-02-02'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-02-02'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.7306
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8786
    true_std: 0.0006
    value_gap_source_arxiv: '2502.00806'
    value_gap_source_title: 'UniGraph2: Learning a Unified Embedding Space to Bind
      Multimodal Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.7306
    has_value_note: false
    value_note: ''
    sort_value: 0.8786
    sort_std: 0.0006
    global_rank: 2
    paper_rank: 83
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGraph2: Learning a Unified Embedding Space to Bind
      Multimodal Graphs'
    comparison_source_arxiv: '2502.00806'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.167
    std: 0.011
    paper_value: 0.167
    paper_std: 0.011
    metric: MRR
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
    source_ref: velickovic2018gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8552
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2505.12684'
    at_pub_source_title: Towards Effective Federated Graph Foundation Model via Mitigating
      Knowledge Entanglement
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.6881999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8552
    true_std: 0.0012
    value_gap_source_arxiv: '2505.12684'
    value_gap_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    value_gap_source_is_current_paper: false
    value_gap: 0.6881999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8552
    sort_std: 0.0012
    global_rank: 3
    paper_rank: 82
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    comparison_source_arxiv: '2505.12684'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.134
    std: 0.027
    paper_value: 0.134
    paper_std: 0.027
    metric: MRR
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
    source_ref: hamilton2017sage
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8298
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2505.12684'
    at_pub_source_title: Towards Effective Federated Graph Foundation Model via Mitigating
      Knowledge Entanglement
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.6958
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8298
    true_std: 0.0022
    value_gap_source_arxiv: '2505.12684'
    value_gap_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    value_gap_source_is_current_paper: false
    value_gap: 0.6958
    has_value_note: false
    value_note: ''
    sort_value: 0.8298
    sort_std: 0.0022
    global_rank: 11
    paper_rank: 83
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    comparison_source_arxiv: '2505.12684'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.192
    std: 0.014
    paper_value: 0.192
    paper_std: 0.014
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8227
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2505.12684'
    at_pub_source_title: Towards Effective Federated Graph Foundation Model via Mitigating
      Knowledge Entanglement
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.6307
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8227
    true_std: 0.0018
    value_gap_source_arxiv: '2505.12684'
    value_gap_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    value_gap_source_is_current_paper: false
    value_gap: 0.6307
    has_value_note: false
    value_note: ''
    sort_value: 0.8227
    sort_std: 0.0018
    global_rank: 12
    paper_rank: 82
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    comparison_source_arxiv: '2505.12684'
    is_best: false
    is_std_outlier: false
  - model: OFA
    model_key: ofa
    model_plain: OFA
    value: 0.075
    std: 0.011
    paper_value: 0.075
    paper_std: 0.011
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu2024ofa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: null
    at_pub_source_arxiv: '2601.21369'
    at_pub_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    at_pub_source_date_iso: '2026-01-29'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.7250000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: null
    value_gap_source_arxiv: '2601.21369'
    value_gap_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.7250000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: null
    global_rank: 14
    paper_rank: 84
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    comparison_source_arxiv: '2601.21369'
    is_best: false
    is_std_outlier: false
  - model: GraphMAE
    model_key: graphmae
    model_plain: GraphMAE
    value: 0.224
    std: 0.014
    paper_value: 0.224
    paper_std: 0.014
    metric: MRR
    higher_is_better: true
    is_baseline: true
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
    source_ref: hou2022graphmae
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7899
    at_pub_std: null
    at_pub_source_arxiv: '2411.06070'
    at_pub_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    at_pub_source_date_iso: '2024-11-09'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.5659000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7899
    true_std: null
    value_gap_source_arxiv: '2411.06070'
    value_gap_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    value_gap_source_is_current_paper: false
    value_gap: 0.5659000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7899
    sort_std: null
    global_rank: 15
    paper_rank: 78
    rank_delta: 63
    rank_delta_abs: 63
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    comparison_source_arxiv: '2411.06070'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.231
    std: 0.009
    paper_value: 0.231
    paper_std: 0.009
    metric: MRR
    higher_is_better: true
    is_baseline: true
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
    source_ref: thakoor2022bgrl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7544
    at_pub_std: null
    at_pub_source_arxiv: '2411.06070'
    at_pub_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    at_pub_source_date_iso: '2024-11-09'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.5234
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7544
    true_std: null
    value_gap_source_arxiv: '2411.06070'
    value_gap_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    value_gap_source_is_current_paper: false
    value_gap: 0.5234
    has_value_note: false
    value_note: ''
    sort_value: 0.7544
    sort_std: null
    global_rank: 18
    paper_rank: 77
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    comparison_source_arxiv: '2411.06070'
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.152
    std: 0.019
    paper_value: 0.152
    paper_std: 0.019
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chen2024llaga
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.152
    true_std: 0.019
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.152
    sort_std: 0.019
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIT
    model_key: git
    model_plain: GIT
    value: 0.094
    std: 0.013
    paper_value: 0.094
    paper_std: 0.013
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wang2024git
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Inductive-entity shift via KG completion with test-time candidate
      entities held out.
    date: May 7, 2026
    date_display: May 2026
    date_iso: '2026-05-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.094
    true_std: 0.013
    value_gap_source_arxiv: '2605.06576'
    value_gap_source_title: On the Safety of Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.094
    sort_std: 0.013
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: Knowledge Graphs
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Tolokers
      dataset_slug: tolokers
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
---

