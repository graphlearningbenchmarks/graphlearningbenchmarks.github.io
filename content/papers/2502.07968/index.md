---
title: Generative Risk Minimization for Out-of-Distribution Generalization on Graphs
arxiv_id: '2502.07968'
source_url: ''
authors:
- name: Song Wang
  orcid: null
  s2_author_id: '2117075272'
  s2_url: null
- name: Zhen Tan
  orcid: null
  s2_author_id: '2309805899'
  s2_url: null
- name: Yaochen Zhu
  orcid: null
  s2_author_id: '2261804201'
  s2_url: null
- name: Chuxu Zhang
  orcid: null
  s2_author_id: '2117879943'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '2343590951'
  s2_url: null
published_date: Feb 11, 2025
published_date_iso: '2025-02-11'
published_venue: TMLR 2025
published_conference: TMLR 2025
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Out-of-distribution (OOD) generalization on graphs aims at dealing with
  scenarios where the test graph distribution differs from the training graph distributions.
  Compared to i.i.d. data like images, the OOD generalization problem on graph-structured
  data remains challenging due to the non-i.i.d. property and complex structural information
  on graphs. Recently, several works on graph OOD generalization have explored extracting
  invariant subgraphs that share crucial classification information across different
  distributions. Nevertheless, such a strategy could be suboptimal for entirely capturing
  the invariant information, as the extraction of discrete structures could potentially
  lead to the loss of invariant information or the involvement of spurious information.
  In this paper, we propose an innovative framework, named Generative Risk Minimization
  (GRM), designed to generate an invariant subgraph for each input graph to be classified,
  instead of extraction. To address the challenge of optimization in the absence of
  optimal invariant subgraphs (i.e., ground truths), we derive a tractable form of
  the proposed GRM objective by introducing a latent causal variable, and its effectiveness
  is validated by our theoretical analysis. We further conduct extensive experiments
  across a variety of real-world graph datasets for both node-level and graph-level
  OOD generalization, and the results demonstrate the superiority of our framework
  GRM. Our code is provided at https://github.com/SongW-SW/GRM.
codebase_url: https://github.com/SongW-SW/GRM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GRM
mrr: 0.0714
adjusted_mrr: 0.0238
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
  - model: MEG
    model_key: clear
    model_plain: MEG
    value: 0.997
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.08443'
    title: 'CLEAR: Generative Counterfactual Explanations on Graphs'
    date: Oct 16, 2022
    date_display: Oct 2022
    date_iso: '2022-10-16'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.997
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MEG
    model_key: random
    model_plain: MEG
    value: 0.897
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.08443'
    title: 'CLEAR: Generative Counterfactual Explanations on Graphs'
    date: Oct 16, 2022
    date_display: Oct 2022
    date_iso: '2022-10-16'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.897
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MEG
    model_key: eg-ist
    model_plain: MEG
    value: 0.897
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.08443'
    title: 'CLEAR: Generative Counterfactual Explanations on Graphs'
    date: Oct 16, 2022
    date_display: Oct 2022
    date_iso: '2022-10-16'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.897
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRM
    model_key: grm
    model_plain: GRM
    value: 0.8102
    std: null
    paper_value: 0.8102
    paper_std: null
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
    protocol_note: OGB scaffold split
    date: Feb 11, 2025
    date_display: Feb 2025
    date_iso: '2025-02-11'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
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
    true_value: 0.8102
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8102
    sort_std: null
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
  - model: GALA
    model_key: gala
    model_plain: GALA
    value: 0.8053
    std: null
    paper_value: 0.8053
    paper_std: null
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
    source_ref: chen2023does
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Feb 11, 2025
    date_display: Feb 2025
    date_iso: '2025-02-11'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
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
    true_value: 0.8053
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8053
    sort_std: null
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
  - model: CIGA
    model_key: ciga
    model_plain: CIGA
    value: 0.7975
    std: null
    paper_value: 0.7975
    paper_std: null
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
    source_ref: chen2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Feb 11, 2025
    date_display: Feb 2025
    date_iso: '2025-02-11'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.797
    at_pub_std: 0.0192
    at_pub_source_arxiv: '2501.04102'
    at_pub_source_title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
      Generalization
    at_pub_source_date_iso: '2024-12-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-02-11'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7975
    true_std: null
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7975
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.7908
    std: null
    paper_value: 0.7908
    paper_std: null
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
    source_ref: li2022learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Feb 11, 2025
    date_display: Feb 2025
    date_iso: '2025-02-11'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7908
    at_pub_std: 0.0247
    at_pub_source_arxiv: '2501.04102'
    at_pub_source_title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
      Generalization
    at_pub_source_date_iso: '2024-12-09'
    at_pub_source_date_label: '2024'
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
    true_value: 0.7908
    true_std: 0.0247
    value_gap_source_arxiv: '2501.04102'
    value_gap_source_title: Enhancing Distribution and Label Consistency for Graph
      Out-of-Distribution Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7908
    sort_std: 0.0247
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
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.7705
    std: null
    paper_value: 0.7705
    paper_std: null
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
    source_ref: wudiscovering
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Feb 11, 2025
    date_display: Feb 2025
    date_iso: '2025-02-11'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7705
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7705
    true_std: 0.0057
    value_gap_source_arxiv: '2201.12872'
    value_gap_source_title: Discovering Invariant Rationales for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7705
    sort_std: 0.0057
    global_rank: 166
    paper_rank: 166
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
single_proposed_model: GRM
---

