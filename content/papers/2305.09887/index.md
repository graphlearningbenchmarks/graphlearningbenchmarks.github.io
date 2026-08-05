---
title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
  Partitions Improve Model Aggregation'
arxiv_id: '2305.09887'
source_url: ''
authors:
- name: Jiong Zhu
  orcid: null
  s2_author_id: '50077183'
  s2_url: null
- name: Aishwarya Reganti
  orcid: null
  s2_author_id: '8856206'
  s2_url: null
- name: Edward Huang
  orcid: null
  s2_author_id: '2057479333'
  s2_url: null
- name: Charles Dickens
  orcid: null
  s2_author_id: '51118486'
  s2_url: null
- name: Nikhil Rao
  orcid: null
  s2_author_id: '145850291'
  s2_url: null
- name: Karthik Subbian
  orcid: null
  s2_author_id: '2691095'
  s2_url: null
- name: Danai Koutra
  orcid: null
  s2_author_id: '2479152'
  s2_url: null
published_date: May 17, 2023
published_date_iso: '2023-05-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Distributed training of GNNs enables learning on massive graphs (e.g., social
  and e-commerce networks) that exceed the storage and computational capacity of a
  single machine. To reach performance comparable to centralized training, distributed
  frameworks focus on maximally recovering cross-instance node dependencies with either
  communication across instances or periodic fallback to centralized training, which
  create overhead and limit the framework scalability. In this work, we present a
  simplified framework for distributed GNN training that does not rely on the aforementioned
  costly operations, and has improved scalability, convergence speed and performance
  over the state-of-the-art approaches. Specifically, our framework (1) assembles
  independent trainers, each of which asynchronously learns a local model on locally-available
  parts of the training graph, and (2) only conducts periodic (time-based) model aggregation
  to synchronize the local models. Backed by our theoretical analysis, instead of
  maximizing the recovery of cross-instance node dependencies---which has been considered
  the key behind closing the performance gap between model aggregation and centralized
  training---, our framework leverages randomized assignment of nodes or super-nodes
  (i.e., collections of original nodes) to partition the training graph such that
  it improves data uniformity and minimizes the discrepancy of gradient and loss function
  across instances. In our experiments on social and e-commerce networks with up to
  1.3 billion edges, our proposed RandomTMA and SuperTMA approaches---despite using
  less training data---achieve state-of-the-art performance and 2.31x speedup compared
  to the fastest baseline, and show better robustness to trainer failures.
codebase_url: https://github.com/amazon-science/random-tma
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: ogbl-citation2
  rows:
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.9072
    std: 0.0012
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/GraphPKU/Refined-GAE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9072
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CFG
    model_key: cfg
    model_plain: CFG
    value: 0.8997
    std: 0.0015
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_display: Sep 2023
    date_iso: '2023-09-11'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features
    is_global_top: true
    global_rank: 2
    sort_value: 0.8997
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIEG
    model_key: sieg
    model_plain: SIEG
    value: 0.8987
    std: 0.0018
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_display: Sep 2023
    date_iso: '2023-09-11'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8987
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8705
    std: 0.0004
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.17475'
    title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
      Networks
    date: Sep 26, 2024
    date_display: Sep 2024
    date_iso: '2024-09-26'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/tensor-gales/HeteLinkPred
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.8705
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SuperTMA
    model_key: supertma
    model_plain: SuperTMA
    value: 0.8375
    std: 0.0043
    paper_value: 0.8375
    paper_std: 0.0043
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard ogbl-citation2 split as provided by OGB
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
    true_value: 0.8375
    true_std: 0.0043
    value_gap_source_arxiv: '2305.09887'
    value_gap_source_title: 'Simplifying Distributed Neural Network Training on Massive
      Graphs: Randomized Partitions Improve Model Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8375
    sort_std: 0.0043
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RandomTMA
    model_key: randomtma
    model_plain: RandomTMA
    value: 0.8328
    std: 0.0024
    paper_value: 0.8328
    paper_std: 0.0024
    metric: MRR
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard ogbl-citation2 split as provided by OGB
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
    true_value: 0.8328
    true_std: 0.0024
    value_gap_source_arxiv: '2305.09887'
    value_gap_source_title: 'Simplifying Distributed Neural Network Training on Massive
      Graphs: Randomized Partitions Improve Model Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8328
    sort_std: 0.0024
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
  - model: PSGD-PA
    model_key: psgd-pa
    model_plain: PSGD-PA
    value: 0.824
    std: 0.0028
    paper_value: 0.824
    paper_std: 0.0028
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
    source_ref: DistDGL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard ogbl-citation2 split as provided by OGB
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
    true_value: 0.824
    true_std: 0.0028
    value_gap_source_arxiv: '2305.09887'
    value_gap_source_title: 'Simplifying Distributed Neural Network Training on Massive
      Graphs: Randomized Partitions Improve Model Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.824
    sort_std: 0.0028
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GGS
    model_key: ggs
    model_plain: GGS
    value: 0.8195
    std: 0.002
    paper_value: 0.8195
    paper_std: 0.002
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
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard ogbl-citation2 split as provided by OGB
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
    true_value: 0.8195
    true_std: 0.002
    value_gap_source_arxiv: '2305.09887'
    value_gap_source_title: 'Simplifying Distributed Neural Network Training on Massive
      Graphs: Randomized Partitions Improve Model Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8195
    sort_std: 0.002
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLCG
    model_key: llcg
    model_plain: LLCG
    value: 0.8188
    std: 0.0002
    paper_value: 0.8188
    paper_std: 0.0002
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
    source_ref: ramezani2021learn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard ogbl-citation2 split as provided by OGB
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
    true_value: 0.8188
    true_std: 0.0002
    value_gap_source_arxiv: '2305.09887'
    value_gap_source_title: 'Simplifying Distributed Neural Network Training on Massive
      Graphs: Randomized Partitions Improve Model Aggregation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8188
    sort_std: 0.0002
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.3917
    std: 0.0044
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.06193'
    title: 'Weak Models Can be Good Teachers: A Case Study on Link Prediction with
      MLPs'
    date: Apr 8, 2025
    date_display: Apr 2025
    date_iso: '2025-04-08'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 78
    sort_value: 0.3917
    sort_std: 0.0044
    comparison_type: global_top
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
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-citation2
      dataset_slug: ogbl-citation2
main_figure: /figures/2305.09887/main_figure.jpegoptim.jpg
---

