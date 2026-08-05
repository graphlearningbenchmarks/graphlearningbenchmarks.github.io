---
title: Towards Few-shot Self-explaining Graph Neural Networks
arxiv_id: '2408.07340'
source_url: ''
authors:
- name: Jingyu Peng
  orcid: null
  s2_author_id: '2228304875'
  s2_url: null
- name: Qi Liu
  orcid: null
  s2_author_id: '2253854596'
  s2_url: null
- name: Linan Yue
  orcid: null
  s2_author_id: '2118940856'
  s2_url: null
- name: Zaixin Zhang
  orcid: null
  s2_author_id: '2129455190'
  s2_url: null
- name: Kai Zhang
  orcid: null
  s2_author_id: '2263584690'
  s2_url: null
- name: Yunhao Sha
  orcid: null
  s2_author_id: '2316050509'
  s2_url: null
published_date: Aug 14, 2024
published_date_iso: '2024-08-14'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Recent advancements in Graph Neural Networks (GNNs) have spurred an upsurge
  of research dedicated to enhancing the explainability of GNNs, particularly in critical
  domains such as medicine. A promising approach is the self-explaining method, which
  outputs explanations along with predictions. However, existing self-explaining models
  require a large amount of training data, rendering them unavailable in few-shot
  scenarios. To address this challenge, in this paper, we propose a Meta-learned Self-Explaining
  GNN (MSE-GNN), a novel framework that generates explanations to support predictions
  in few-shot settings. MSE-GNN adopts a two-stage self-explaining structure, consisting
  of an explainer and a predictor. Specifically, the explainer first imitates the
  attention mechanism of humans to select the explanation subgraph, whereby attention
  is naturally paid to regions containing important characteristics. Subsequently,
  the predictor mimics the decision-making process, which makes predictions based
  on the generated explanation. Moreover, with a novel meta-training process and a
  designed mechanism that exploits task information, MSE-GNN can achieve remarkable
  performance on new few-shot tasks. Extensive experimental results on four datasets
  demonstrate that MSE-GNN can achieve superior performance on prediction tasks while
  generating high-quality explanations compared with existing methods. The code is
  publicly available at.
codebase_url: https://github.com/jypeng28/MSE-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MSE-GNN
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
  dataset: ogbg-molhiv
  rows:
  - model: ASMAML
    model_key: asmaml
    model_plain: ASMAML
    value: 0.6818
    std: 0.008
    paper_value: 0.6818
    paper_std: 0.008
    metric: AUC-ROC
    higher_is_better: true
    is_baseline: true
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6818
    true_std: 0.008
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6818
    sort_std: 0.008
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
  - model: MSE-GNN
    model_key: mse-gnn
    model_plain: MSE-GNN
    value: 0.6673
    std: 0.007
    paper_value: 0.6673
    paper_std: 0.007
    metric: AUC-ROC
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6673
    true_std: 0.007
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6673
    sort_std: 0.007
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CAL_Meta
    model_key: cal_meta
    model_plain: CAL_Meta
    value: 0.658
    std: 0.012
    paper_value: 0.658
    paper_std: 0.012
    metric: AUC-ROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.658
    true_std: 0.012
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.658
    sort_std: 0.012
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREA_Meta
    model_key: grea_meta
    model_plain: GREA_Meta
    value: 0.6542
    std: 0.005
    paper_value: 0.6542
    paper_std: 0.005
    metric: AUC-ROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6542
    true_std: 0.005
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6542
    sort_std: 0.005
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
  - model: MAML
    model_key: maml
    model_plain: MAML
    value: 0.6538
    std: 0.016
    paper_value: 0.6538
    paper_std: 0.016
    metric: AUC-ROC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6538
    true_std: 0.016
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6538
    sort_std: 0.016
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CAL_Raw
    model_key: cal_raw
    model_plain: CAL_Raw
    value: 0.623
    std: 0.008
    paper_value: 0.623
    paper_std: 0.008
    metric: AUC-ROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.623
    true_std: 0.008
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.623
    sort_std: 0.008
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
  - model: ProtoNet
    model_key: protonet
    model_plain: ProtoNet
    value: 0.554
    std: 0.006
    paper_value: 0.554
    paper_std: 0.006
    metric: AUC-ROC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.554
    true_std: 0.006
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.554
    sort_std: 0.006
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GREA_Raw
    model_key: grea_raw
    model_plain: GREA_Raw
    value: 0.521
    std: 0.009
    paper_value: 0.521
    paper_std: 0.009
    metric: AUC-ROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=75)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 2-way 5-shot classification task
    date: Aug 14, 2024
    date_display: Aug 2024
    date_iso: '2024-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.521
    true_std: 0.009
    value_gap_source_arxiv: '2408.07340'
    value_gap_source_title: Towards Few-shot Self-explaining Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.521
    sort_std: 0.009
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
  rank_metric: AUC-ROC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - AUC-ROC
  metric: AUC-ROC
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
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
single_proposed_model: MSE-GNN
main_figure: /figures/2408.07340/main_figure.jpegoptim.jpg
---

