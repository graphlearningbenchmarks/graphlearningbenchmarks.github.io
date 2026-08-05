---
title: 'Everything Perturbed All at Once: Enabling Differentiable Graph Attacks'
arxiv_id: '2308.15614'
source_url: ''
authors:
- name: Haoran Liu
  orcid: null
  s2_author_id: '2143857491'
  s2_url: null
- name: Bokun Wang
  orcid: null
  s2_author_id: '30296838'
  s2_url: null
- name: Jianling Wang
  orcid: null
  s2_author_id: '2110273966'
  s2_url: null
- name: Xiangjue Dong
  orcid: null
  s2_author_id: '1716200686'
  s2_url: null
- name: Tianbao Yang
  orcid: null
  s2_author_id: '40381920'
  s2_url: null
- name: James Caverlee
  orcid: null
  s2_author_id: '1697232'
  s2_url: null
published_date: Aug 29, 2023
published_date_iso: '2023-08-29'
published_venue: WWW 2023
published_conference: WWW 2023
published_conference_short: WWW
published_conference_slug: www
abstract: As powerful tools for representation learning on graphs, graph neural networks
  (GNNs) have played an important role in applications including social networks,
  recommendation systems, and online web services. However, GNNs have been shown to
  be vulnerable to adversarial attacks, which can significantly degrade their effectiveness.
  Recent state-of-the-art approaches in adversarial attacks rely on gradient-based
  meta-learning to selectively perturb a single edge with the highest attack score
  until they reach the budget constraint. While effective in identifying vulnerable
  links, these methods are plagued by high computational costs. By leveraging continuous
  relaxation and parameterization of the graph structure, we propose a novel attack
  method called Differentiable Graph Attack (DGA) to efficiently generate effective
  attacks and meanwhile eliminate the need for costly retraining. Compared to the
  state-of-the-art, DGA achieves nearly equivalent attack performance with 6 times
  less training time and 11 times smaller GPU memory footprint on different benchmark
  datasets. Additionally, we provide extensive experimental analyses of the transferability
  of the DGA among different graph models, as well as its robustness against widely-used
  defense mechanisms.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DICE
    model_key: dice
    model_plain: DICE
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: waniek2018hiding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate (clean graph).
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 447
    paper_rank: 447
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Meta-Self
    model_key: meta-self
    model_plain: Meta-Self
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: zugner2019adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate.
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 448
    paper_rank: 448
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Meta-Train
    model_key: meta-train
    model_plain: Meta-Train
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: zugner2019adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate.
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 449
    paper_rank: 449
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-Meta-Self
    model_key: a-meta-self
    model_plain: A-Meta-Self
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: zugner2019adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate.
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 450
    paper_rank: 450
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-Meta-Train
    model_key: a-meta-train
    model_plain: A-Meta-Train
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: zugner2019adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate.
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 451
    paper_rank: 451
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAD
    model_key: grad
    model_plain: GRAD
    value: 0.8362
    std: null
    paper_value: 0.8362
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
    source_ref: liu2022towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Cora with 0% perturbation rate.
    date: Aug 29, 2023
    date_display: Aug 2023
    date_iso: '2023-08-29'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-29'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8362
    true_std: null
    value_gap_source_arxiv: '2308.15614'
    value_gap_source_title: 'Everything Perturbed All at Once: Enabling Differentiable
      Graph Attacks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8362
    sort_std: null
    global_rank: 452
    paper_rank: 452
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
main_figure: /figures/2308.15614/main_figure.jpegoptim.jpg
---

