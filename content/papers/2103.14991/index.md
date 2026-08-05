---
title: Graph Unlearning
arxiv_id: '2103.14991'
source_url: ''
authors:
- name: Min Chen
  orcid: null
  s2_author_id: '2145944749'
  s2_url: null
- name: Zhikun Zhang
  orcid: null
  s2_author_id: '48806102'
  s2_url: null
- name: Tianhao Wang
  orcid: null
  s2_author_id: '49980880'
  s2_url: null
- name: M. Backes
  orcid: null
  s2_author_id: '144588806'
  s2_url: null
- name: Mathias Humbert
  orcid: null
  s2_author_id: '144887171'
  s2_url: null
- name: Yang Zhang
  orcid: null
  s2_author_id: '2145954003'
  s2_url: null
published_date: Mar 27, 2021
published_date_iso: '2021-03-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Machine unlearning is a process of removing the impact of some training
  data from the machine learning (ML) models upon receiving removal requests. While
  straightforward and legitimate, retraining the ML model from scratch incurs a high
  computational overhead. To address this issue, a number of approximate algorithms
  have been proposed in the domain of image and text data, among which is the state-of-the-art
  solution. It randomly partitions the training set into multiple shards and trains
  a constituent model for each shard. However, directly applying to the graph data
  can severely damage the graph structural information, and thereby the resulting
  ML model utility. In this paper, we propose, a novel machine unlearning framework
  tailored to graph data. Its contributions include two novel graph partition algorithms
  and a learning-based aggregation method. We conduct extensive experiments on five
  real-world graph datasets to illustrate the unlearning efficiency and model utility
  of. It achieves 2.06$ $ (small dataset) to 35.94$ $ (large dataset) unlearning time
  improvement. On the other hand, achieves up to $62.5\
codebase_url: https://github.com/MinChen00/Graph-Unlearning
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphEraser-BLPA
- GraphEraser-BEKM
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: CiteSeer
  rows:
  - model: SGCONV
    model_key: mixhop
    model_plain: SGCONV
    value: 0.78
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: MixHop is a multi-scale GNN.
    is_global_top: true
    global_rank: 1
    sort_value: 0.78
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGCONV
    model_key: sgconv
    model_plain: SGCONV
    value: 0.763
    std: 0.002
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: SGCONV is a graph convolutional neural network.
    is_global_top: true
    global_rank: 2
    sort_value: 0.763
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGCONV
    model_key: appnp
    model_plain: SGCONV
    value: 0.754
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: APPNP is a graph convolutional neural network.
    is_global_top: true
    global_rank: 3
    sort_value: 0.754
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphEraser-BEKM
    model_key: grapheraser-bekm
    model_plain: GraphEraser-BEKM
    value: 0.746
    std: 0.006
    paper_value: 0.746
    paper_std: 0.006
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.746
    true_std: 0.006
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.006
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.746
    std: 0.006
    paper_value: 0.746
    paper_std: 0.006
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.74
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.746
    true_std: 0.006
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.006
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.493
    std: 0.006
    paper_value: 0.493
    paper_std: 0.006
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.742
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.249
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.742
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.249
    has_value_note: false
    value_note: ''
    sort_value: 0.742
    sort_std: 0.001
    global_rank: 7
    paper_rank: 35
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.739
    std: 0.02
    paper_value: 0.739
    paper_std: 0.02
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: 0.02
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: 0.02
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.716
    std: 0.007
    paper_value: 0.716
    paper_std: 0.007
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.716
    true_std: 0.007
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.716
    sort_std: 0.007
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
  - model: GraphEraser-BLPA
    model_key: grapheraser-blpa
    model_plain: GraphEraser-BLPA
    value: 0.676
    std: 0.004
    paper_value: 0.676
    paper_std: 0.004
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split) as described in experimental setup
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.676
    true_std: 0.004
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.676
    sort_std: 0.004
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Cora
  rows:
  - model: SGCONV
    model_key: acm-gcn
    model_plain: SGCONV
    value: 0.8894
    std: 0.0054
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8894
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGCONV
    model_key: appnp
    model_plain: SGCONV
    value: 0.888
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: APPNP is a standard GNN.
    is_global_top: true
    global_rank: 2
    sort_value: 0.888
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGCONV
    model_key: graphsage
    model_plain: SGCONV
    value: 0.881
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GraphSAGE is a standard GNN that pools node attributes.
    is_global_top: true
    global_rank: 3
    sort_value: 0.881
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.739
    std: 0.003
    paper_value: 0.739
    paper_std: 0.003
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split as described in setup)
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.879
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.14
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.879
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.14
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.001
    global_rank: 6
    paper_rank: 39
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.823
    std: 0.006
    paper_value: 0.823
    paper_std: 0.006
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split as described in setup)
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.867
    at_pub_std: 0.002
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.04400000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.867
    true_std: 0.002
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.04400000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.867
    sort_std: 0.002
    global_rank: 11
    paper_rank: 27
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.801
    std: 0.018
    paper_value: 0.801
    paper_std: 0.018
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split as described in setup)
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-08'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8537
    true_std: 0.0074
    value_gap_source_arxiv: '2402.05894'
    value_gap_source_title: Large Language Model Meets Graph Neural Network in Knowledge
      Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.05269999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8537
    sort_std: 0.0074
    global_rank: 14
    paper_rank: 30
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.824
    std: 0.004
    paper_value: 0.824
    paper_std: 0.004
    metric: F1
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (80/20 split as described in setup)
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8536
    true_std: null
    value_gap_source_arxiv: '2307.00534'
    value_gap_source_title: Shared Growth of Graph Neural Networks via Prompted Free-direction
      Knowledge Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.02960000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8536
    sort_std: null
    global_rank: 15
    paper_rank: 26
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.657
    std: 0.019
    paper_value: 0.657
    paper_std: 0.019
    metric: F1
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: MLP uses only node features
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.657
    true_std: 0.019
    value_gap_source_arxiv: '2103.14991'
    value_gap_source_title: Graph Unlearning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.019
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
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
main_figure: /figures/2103.14991/main_figure.jpegoptim.jpg
---

