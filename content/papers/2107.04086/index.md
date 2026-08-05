---
title: Robust Counterfactual Explanations on Graph Neural Networks
arxiv_id: '2107.04086'
source_url: ''
authors:
- name: Mohit Bajaj
  orcid: null
  s2_author_id: '2065738416'
  s2_url: null
- name: Lingyang Chu
  orcid: null
  s2_author_id: '2074100'
  s2_url: null
- name: Zihui Xue
  orcid: null
  s2_author_id: '2060445410'
  s2_url: null
- name: J. Pei
  orcid: null
  s2_author_id: '145525190'
  s2_url: null
- name: Lanjun Wang
  orcid: null
  s2_author_id: '49680751'
  s2_url: null
- name: P. C. Lam
  orcid: null
  s2_author_id: '23033976'
  s2_url: null
- name: Yong Zhang
  orcid: null
  s2_author_id: '2144288655'
  s2_url: null
published_date: Jul 8, 2021
published_date_iso: '2021-07-08'
published_venue: NeurIPS 2021
published_conference: NeurIPS 2021
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Massive deployment of Graph Neural Networks (GNNs) in high-stake applications
  generates a strong demand for explanations that are robust to noise and align well
  with human intuition. Most existing methods generate explanations by identifying
  a subgraph of an input graph that has a strong correlation with the prediction.
  These explanations are not robust to noise because independently optimizing the
  correlation for a single input can easily overfit noise. Moreover, they are not
  counterfactual because removing an identified subgraph from an input graph does
  not necessarily change the prediction result. In this paper, we propose a novel
  method to generate robust counterfactual explanations on GNNs by explicitly modelling
  the common decision logic of GNNs on similar input graphs. Our explanations are
  naturally robust to noise because they are produced from the common decision boundaries
  of a GNN that govern the predictions of many similar input graphs. The explanations
  are also counterfactual because removing the set of edges identified by an explanation
  from the input graph changes the prediction significantly. Exhaustive experiments
  on many public datasets demonstrate the superior performance of our method.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  dataset: NCI1
  rows:
  - model: ECC
    model_key: wl-mlp
    model_plain: ECC
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: gin
    model_plain: ECC
    value: 0.9934
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 2
    sort_value: 0.9934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.84
    std: null
    paper_value: 0.84
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy of the trained GCN model on the NCI1 dataset.
    date: Jul 8, 2021
    date_display: Jul 2021
    date_iso: '2021-07-08'
    published_venue: NeurIPS 2021
    published_conference: NeurIPS 2021
    at_pub_value: 0.8365
    at_pub_std: 0.0169
    at_pub_source_arxiv: '2012.08734'
    at_pub_source_title: Hierarchical Graph Capsule Network
    at_pub_source_date_iso: '2020-12-16'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0034999999999999476
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9727
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.13270000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9727
    sort_std: null
    global_rank: 3
    paper_rank: 38
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
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
    - dataset: NCI1
      dataset_slug: nci1
main_figure: /figures/2107.04086/main_figure.jpegoptim.jpg
---

