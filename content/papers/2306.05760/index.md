---
title: Efficient GNN Explanation via Learning Removal-based Attribution
arxiv_id: '2306.05760'
source_url: ''
authors:
- name: Yao Rong
  orcid: null
  s2_author_id: '2057815422'
  s2_url: null
- name: Guanchu Wang
  orcid: null
  s2_author_id: '32780441'
  s2_url: null
- name: Qizhang Feng
  orcid: null
  s2_author_id: '2151233715'
  s2_url: null
- name: Ninghao Liu
  orcid: null
  s2_author_id: '47717322'
  s2_url: null
- name: Zirui Liu
  orcid: null
  s2_author_id: '47781070'
  s2_url: null
- name: Enkelejda Kasneci
  orcid: null
  s2_author_id: '1884159'
  s2_url: null
- name: Xia Hu
  orcid: null
  s2_author_id: '2276449057'
  s2_url: null
published_date: Jun 9, 2023
published_date_iso: '2023-06-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: As Graph Neural Networks (GNNs) have been widely used in real-world applications,
  model explanations are required not only by users but also by legal regulations.
  However, simultaneously achieving high fidelity and low computational costs in generating
  explanations has been a challenge for current methods. In this work, we propose
  a framework of GNN explanation named to address this problem. Specifically, we introduce
  removal-based attribution and demonstrate its substantiated link to interpretability
  fidelity theoretically and experimentally. The explainer in learns to generate removal-based
  attribution which enables providing explanations with high fidelity. A strategy
  of subgraph sampling is designed in to improve the scalability of the training process.
  In the deployment, can efficiently generate the explanation through a feed-forward
  pass. We benchmark our approach with other state-of-the-art GNN explanation methods
  on six datasets. Results highlight the effectiveness of our framework regarding
  both efficiency and fidelity. In particular, is 3.5$ $ faster and achieves higher
  fidelity than the state-of-the-art method on the large dataset ogbn-arxiv (more
  than 160K nodes and 1M edges), showing its great potential in real-world applications.
  Our source code is available at.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MI
mrr: 0.0017
adjusted_mrr: 0.0006
mrr_dataset_count: 1
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
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
  - model: MI
    model_key: mi
    model_plain: MI
    value: 0.81
    std: null
    paper_value: 0.81
    paper_std: null
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy of the target model used for explanation.
    date: Jun 9, 2023
    date_display: Jun 2023
    date_iso: '2023-06-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: 0.011
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2023-06-09'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08699999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.81
    true_std: null
    value_gap_source_arxiv: '2306.05760'
    value_gap_source_title: Efficient GNN Explanation via Learning Removal-based Attribution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: null
    global_rank: 597
    paper_rank: 597
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Contrastive Multi-View Representation Learning on Graphs
    comparison_source_arxiv: '2006.05582'
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
single_proposed_model: MI
main_figure: /figures/2306.05760/main_figure.jpegoptim.jpg
---

