---
title: Edge Directionality Improves Learning on Heterophilic Graphs
arxiv_id: '2305.10498'
source_url: ''
authors:
- name: Emanuele Rossi
  orcid: null
  s2_author_id: '2056294358'
  s2_url: null
- name: Bertrand Charpentier
  orcid: null
  s2_author_id: '50997190'
  s2_url: null
- name: Francesco Di Giovanni
  orcid: null
  s2_author_id: '94290272'
  s2_url: null
- name: Fabrizio Frasca
  orcid: null
  s2_author_id: '51484149'
  s2_url: null
- name: Stephan Günnemann
  orcid: null
  s2_author_id: '3075189'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2149583375'
  s2_url: null
published_date: May 17, 2023
published_date_iso: '2023-05-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks (GNNs) have become the de-facto standard tool for
  modeling relational data. However, while many real-world graphs are directed, the
  majority of today''s GNN models discard this information altogether by simply making
  the graph undirected. The reasons for this are historical: 1) many early variants
  of spectral GNNs explicitly required undirected graphs, and 2) the first benchmarks
  on homophilic graphs did not find significant gain from using direction. In this
  paper, we show that in heterophilic settings, treating the graph as directed increases
  the effective homophily of the graph, suggesting a potential gain from the correct
  use of directionality information. To this end, we introduce Directed Graph Neural
  Network (Dir-GNN), a novel general framework for deep learning on directed graphs.
  Dir-GNN can be used to extend any Message Passing Neural Network (MPNN) to account
  for edge directionality information by performing separate aggregations of the incoming
  and outgoing edges. We prove that Dir-GNN matches the expressivity of the Directed
  Weisfeiler-Lehman test, exceeding that of conventional MPNNs. In extensive experiments,
  we validate that while our framework leaves performance unchanged on homophilic
  datasets, it leads to large gains over base models such as GCN, GAT and GraphSage
  on heterophilic benchmarks, outperforming much more complex methods and achieving
  new state-of-the-art results. The code for the paper can be found at.'
codebase_url: https://github.com/emalgorithm/directed-graph-neural-network
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- LINKX Benchmarks
benchmark_coverage:
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: snap-patents
  rows:
  - model: LargeGT-full
    model_key: fabernet
    model_plain: LargeGT-full
    value: 0.751
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.751
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: largescalenet
    model_plain: LargeGT-full
    value: 0.7505
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_display: Nov 2024
    date_iso: '2024-11-28'
    venue: null
    codebase_url: https://github.com/Qin87/ScaleNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7505
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: dirgnn
    model_plain: LargeGT-full
    value: 0.7395
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7395
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: dir-gcn
    model_key: dir-gcn
    model_plain: dir-gcn
    value: 0.7132
    std: 0.0006
    paper_value: 0.7132
    paper_std: 0.0006
    metric: Accuracy
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Ablation study on undirected vs directed versions
    date: May 17, 2023
    date_display: May 2023
    date_iso: '2023-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7132
    true_std: 0.0006
    value_gap_source_arxiv: '2305.10498'
    value_gap_source_title: Edge Directionality Improves Learning on Heterophilic
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7132
    sort_std: 0.0006
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
  - model: dir-sage
    model_key: dir-sage
    model_plain: dir-sage
    value: 0.7026
    std: 0.0014
    paper_value: 0.7026
    paper_std: 0.0014
    metric: Accuracy
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Ablation study on undirected vs directed versions
    date: May 17, 2023
    date_display: May 2023
    date_iso: '2023-05-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7026
    true_std: 0.0014
    value_gap_source_arxiv: '2305.10498'
    value_gap_source_title: Edge Directionality Improves Learning on Heterophilic
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7026
    sort_std: 0.0014
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
- benchmark: LINKX Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: snap-patents
      dataset_slug: snap-patents
main_figure: /figures/2305.10498/main_figure.jpegoptim.jpg
---

