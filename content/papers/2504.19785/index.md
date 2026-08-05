---
title: Heterophily-informed Message Passing
arxiv_id: '2504.19785'
source_url: ''
authors:
- name: Haishan Wang
  orcid: null
  s2_author_id: '2354065858'
  s2_url: null
- name: Arno Solin
  orcid: null
  s2_author_id: '2303464125'
  s2_url: null
- name: Vikas Garg
  orcid: null
  s2_author_id: '2362314100'
  s2_url: null
published_date: Apr 28, 2025
published_date_iso: '2025-04-28'
published_venue: TMLR 2025
published_conference: TMLR 2025
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Graph neural networks (GNNs) are known to be vulnerable to oversmoothing
  due to their implicit homophily assumption. We mitigate this problem with a novel
  scheme that regulates the aggregation of messages, modulating the type and extent
  of message passing locally thereby preserving both the low and high-frequency components
  of information. Our approach relies solely on learnt embeddings, obviating the need
  for auxiliary labels, thus extending the benefits of heterophily-aware embeddings
  to broader applications,, generative modelling. Our experiments, conducted across
  various data sets and GNN architectures, demonstrate performance enhancements and
  reveal heterophily patterns across standard classification benchmarks. Furthermore,
  application to molecular generation showcases notable performance improvements on
  chemoinformatics benchmarks.
codebase_url: https://github.com/AaltoML/heterophily-imp
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Heterophilic Graphs
- Heterophily Benchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 5
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: Amazon-Computers
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.916
    std: 0.005
    paper_value: 0.916
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.916
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: 0.005
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
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.915
    std: 0.005
    paper_value: 0.915
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.915
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.005
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
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.912
    std: 0.006
    paper_value: 0.912
    paper_std: 0.006
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.006
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.912
    std: 0.003
    paper_value: 0.912
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.912
    true_std: 0.003
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.003
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.911
    std: 0.003
    paper_value: 0.911
    paper_std: 0.003
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.911
    true_std: 0.003
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: 0.003
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.909
    std: 0.003
    paper_value: 0.909
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.909
    true_std: 0.003
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.909
    sort_std: 0.003
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.909
    std: 0.003
    paper_value: 0.909
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.909
    true_std: 0.003
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.909
    sort_std: 0.003
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.906
    std: 0.004
    paper_value: 0.906
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.906
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.906
    sort_std: 0.004
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
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.903
    std: 0.005
    paper_value: 0.903
    paper_std: 0.005
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.005
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
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.894
    std: 0.006
    paper_value: 0.894
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.894
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.894
    sort_std: 0.006
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
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.84
    std: 0.02
    paper_value: 0.84
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.84
    true_std: 0.02
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: 0.02
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
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.783
    std: 0.014
    paper_value: 0.783
    paper_std: 0.014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.783
    true_std: 0.014
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.783
    sort_std: 0.014
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
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.573
    std: 0.147
    paper_value: 0.573
    paper_std: 0.147
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.573
    true_std: 0.147
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.573
    sort_std: 0.147
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
    is_std_outlier: true
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.431
    std: 0.093
    paper_value: 0.431
    paper_std: 0.093
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.431
    true_std: 0.093
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.431
    sort_std: 0.093
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
    is_std_outlier: true
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.428
    std: 0.038
    paper_value: 0.428
    paper_std: 0.038
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.428
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.428
    sort_std: 0.038
    global_rank: 15
    paper_rank: 15
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
    value: 0.412
    std: 0.031
    paper_value: 0.412
    paper_std: 0.031
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.412
    true_std: 0.031
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.412
    sort_std: 0.031
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
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: Amazon-Photo
  rows:
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.955
    std: 0.004
    paper_value: 0.955
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.955
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.955
    sort_std: 0.004
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
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.955
    std: 0.004
    paper_value: 0.955
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.955
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.955
    sort_std: 0.004
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
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.952
    std: 0.005
    paper_value: 0.952
    paper_std: 0.005
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.952
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.005
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.95
    std: 0.006
    paper_value: 0.95
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.95
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: 0.006
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.946
    std: 0.006
    paper_value: 0.946
    paper_std: 0.006
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.946
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.946
    sort_std: 0.006
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.944
    std: 0.005
    paper_value: 0.944
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.944
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.944
    sort_std: 0.005
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
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.944
    std: 0.004
    paper_value: 0.944
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.944
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.944
    sort_std: 0.004
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.941
    std: 0.005
    paper_value: 0.941
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.941
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.941
    sort_std: 0.005
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
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.941
    std: 0.003
    paper_value: 0.941
    paper_std: 0.003
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.941
    true_std: 0.003
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.941
    sort_std: 0.003
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
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.936
    std: 0.006
    paper_value: 0.936
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.936
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.936
    sort_std: 0.006
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
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.873
    std: 0.013
    paper_value: 0.873
    paper_std: 0.013
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.873
    true_std: 0.013
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.013
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
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.854
    std: 0.016
    paper_value: 0.854
    paper_std: 0.016
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.016
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.016
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
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.782
    std: 0.136
    paper_value: 0.782
    paper_std: 0.136
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.136
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.136
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
    is_std_outlier: true
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.384
    std: 0.157
    paper_value: 0.384
    paper_std: 0.157
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.384
    true_std: 0.157
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.384
    sort_std: 0.157
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
    is_std_outlier: true
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.377
    std: 0.08
    paper_value: 0.377
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.377
    true_std: 0.08
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.377
    sort_std: 0.08
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.353
    std: 0.071
    paper_value: 0.353
    paper_std: 0.071
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.353
    true_std: 0.071
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.353
    sort_std: 0.071
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
    is_std_outlier: true
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id008
  dataset: Amazon-ratings
  rows:
  - model: H2GCN
    model_key: h2gcn + unigap
    model_plain: H2GCN
    value: 0.6375
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6375
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: graphsage + unigap
    model_plain: H2GCN
    value: 0.6283
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6283
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: gcn + unigap
    model_plain: H2GCN
    value: 0.5976
    std: 0.008
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5976
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.488
    std: 0.005
    paper_value: 0.488
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.4909
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0029000000000000137
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5559
    true_std: 0.0027
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.06789999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.5559
    sort_std: 0.0027
    global_rank: 16
    paper_rank: 116
    rank_delta: 100
    rank_delta_abs: 100
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.527
    std: 0.006
    paper_value: 0.527
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.554
    at_pub_std: 0.002
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.027000000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.554
    true_std: 0.002
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.027000000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.554
    sort_std: 0.002
    global_rank: 17
    paper_rank: 55
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.491
    std: 0.006
    paper_value: 0.491
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.538
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.04700000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5411
    true_std: 0.0034
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.05010000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5411
    sort_std: 0.0034
    global_rank: 26
    paper_rank: 113
    rank_delta: 87
    rank_delta_abs: 87
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.535
    std: 0.007
    paper_value: 0.535
    paper_std: 0.007
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
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.535
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.535
    sort_std: 0.007
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.522
    std: 0.006
    paper_value: 0.522
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.522
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.522
    sort_std: 0.006
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.516
    std: 0.005
    paper_value: 0.516
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.516
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.516
    sort_std: 0.005
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.502
    std: 0.005
    paper_value: 0.502
    paper_std: 0.005
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
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
    sort_std: 0.005
    global_rank: 96
    paper_rank: 96
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
    value: 0.502
    std: 0.007
    paper_value: 0.502
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.441
    at_pub_std: 0.008
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.061
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
    sort_std: 0.007
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.497
    std: 0.008
    paper_value: 0.497
    paper_std: 0.008
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
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.497
    true_std: 0.008
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.497
    sort_std: 0.008
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.492
    std: 0.007
    paper_value: 0.492
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.492
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.492
    sort_std: 0.007
    global_rank: 113
    paper_rank: 113
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.482
    std: 0.012
    paper_value: 0.482
    paper_std: 0.012
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.482
    true_std: 0.012
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.482
    sort_std: 0.012
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.482
    std: 0.015
    paper_value: 0.482
    paper_std: 0.015
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
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.482
    true_std: 0.015
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.482
    sort_std: 0.015
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.472
    std: 0.007
    paper_value: 0.472
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.472
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.472
    sort_std: 0.007
    global_rank: 130
    paper_rank: 130
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.471
    std: 0.005
    paper_value: 0.471
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.471
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.471
    sort_std: 0.005
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.464
    std: 0.006
    paper_value: 0.464
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.464
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.464
    sort_std: 0.006
    global_rank: 135
    paper_rank: 135
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.441
    std: 0.006
    paper_value: 0.441
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy reported as ROC-AUC for binary datasets;
      standard split implied by context.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.441
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.441
    sort_std: 0.006
    global_rank: 158
    paper_rank: 158
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
- &id005
  dataset: Cornell
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.948
    std: 0.038
    paper_value: 0.948
    paper_std: 0.038
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
    source_ref: acm_luan2022revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8571
    at_pub_std: null
    at_pub_source_arxiv: '2504.13426'
    at_pub_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    at_pub_source_date_iso: '2025-04-18'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.09089999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.948
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.038
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    comparison_source_arxiv: '2504.13426'
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: rf-gcn
    model_plain: R-SoftGraphAIN
    value: 0.9429
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.914
    std: 0.007
    paper_value: 0.914
    paper_std: 0.007
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
    source_ref: chien2021adaptive_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9157
    at_pub_std: 0.0196
    at_pub_source_arxiv: '2403.03676'
    at_pub_source_title: Simplified PCNet with Robustness
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0016999999999999238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9157
    true_std: 0.0196
    value_gap_source_arxiv: '2403.03676'
    value_gap_source_title: Simplified PCNet with Robustness
    value_gap_source_is_current_paper: false
    value_gap: 0.0016999999999999238
    has_value_note: false
    value_note: ''
    sort_value: 0.9157
    sort_std: 0.0196
    global_rank: 22
    paper_rank: 23
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.862
    std: 0.047
    paper_value: 0.862
    paper_std: 0.047
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
    source_ref: zhu2021graph_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.851
    at_pub_std: 0.061
    at_pub_source_arxiv: '2401.14580'
    at_pub_source_title: 'Design your own universe: a physics-informed agnostic method
      for enhancing graph neural networks'
    at_pub_source_date_iso: '2024-01-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0471
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0471
    global_rank: 82
    paper_rank: 87
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMP
    model_key: acmp
    model_plain: ACMP
    value: 0.854
    std: 0.07
    paper_value: 0.854
    paper_std: 0.07
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
    source_ref: wang2023acmp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.854
    at_pub_std: 0.07
    at_pub_source_arxiv: '2310.16401'
    at_pub_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-20'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.07
    value_gap_source_arxiv: '2605.21247'
    value_gap_source_title: Graph Navier–Stokes Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.07
    global_rank: 100
    paper_rank: 100
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
    value: 0.457
    std: 0.063
    paper_value: 0.457
    paper_std: 0.063
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.819
    at_pub_std: 0.054
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.36199999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: 0.054
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.36199999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.054
    global_rank: 171
    paper_rank: 532
    rank_delta: 361
    rank_delta_abs: 361
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.427
    std: 0.049
    paper_value: 0.427
    paper_std: 0.049
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8015
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2405.16185'
    at_pub_source_title: Differentiable Cluster Graph Neural Network
    at_pub_source_date_iso: '2024-05-25'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3745
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8015
    true_std: 0.0037
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.3745
    has_value_note: false
    value_note: ''
    sort_value: 0.8015
    sort_std: 0.0037
    global_rank: 190
    paper_rank: 551
    rank_delta: 361
    rank_delta_abs: 361
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Differentiable Cluster Graph Neural Network
    comparison_source_arxiv: '2405.16185'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.714
    std: 0.012
    paper_value: 0.714
    paper_std: 0.012
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8196
    at_pub_std: 0.0739
    at_pub_source_arxiv: '2302.03228'
    at_pub_source_title: Heterophily-Aware Graph Attention Network
    at_pub_source_date_iso: '2023-02-07'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10560000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8008
    true_std: 0.0296
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: 0.08679999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8008
    sort_std: 0.0296
    global_rank: 192
    paper_rank: 292
    rank_delta: 100
    rank_delta_abs: 100
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterophily-Aware Graph Attention Network
    comparison_source_arxiv: '2302.03228'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.468
    std: 0.071
    paper_value: 0.468
    paper_std: 0.071
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.78
    at_pub_std: 0.019
    at_pub_source_arxiv: '2309.02769'
    at_pub_source_title: 'Unifying over-smoothing and over-squashing in graph neural
      networks: A physics informed approach and beyond'
    at_pub_source_date_iso: '2023-09-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.312
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.78
    true_std: 0.019
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.312
    has_value_note: false
    value_note: ''
    sort_value: 0.78
    sort_std: 0.019
    global_rank: 222
    paper_rank: 526
    rank_delta: 304
    rank_delta_abs: 304
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unifying over-smoothing and over-squashing in graph
      neural networks: A physics informed approach and beyond'
    comparison_source_arxiv: '2309.02769'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.751
    std: 0.04
    paper_value: 0.751
    paper_std: 0.04
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.751
    true_std: 0.04
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: 0.04
    global_rank: 260
    paper_rank: 260
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.722
    std: 0.076
    paper_value: 0.722
    paper_std: 0.076
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.722
    true_std: 0.076
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.722
    sort_std: 0.076
    global_rank: 287
    paper_rank: 287
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.673
    std: 0.041
    paper_value: 0.673
    paper_std: 0.041
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.673
    true_std: 0.041
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.673
    sort_std: 0.041
    global_rank: 328
    paper_rank: 328
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.608
    std: null
    paper_value: 0.608
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
    source_ref: pei2019geom_node_homophily
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.6412
    at_pub_std: null
    at_pub_source_arxiv: '2303.01265'
    at_pub_source_title: Steering Graph Neural Networks with Pinning Control
    at_pub_source_date_iso: '2023-03-02'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03320000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6412
    true_std: null
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: 0.03320000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.6412
    sort_std: null
    global_rank: 359
    paper_rank: 387
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Steering Graph Neural Networks with Pinning Control
    comparison_source_arxiv: '2303.01265'
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.589
    std: 0.094
    paper_value: 0.589
    paper_std: 0.094
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.589
    true_std: 0.094
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.589
    sort_std: 0.094
    global_rank: 410
    paper_rank: 410
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.505
    std: 0.075
    paper_value: 0.505
    paper_std: 0.075
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.505
    true_std: 0.075
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.505
    sort_std: 0.075
    global_rank: 508
    paper_rank: 508
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.503
    std: 0.107
    paper_value: 0.503
    paper_std: 0.107
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.503
    true_std: 0.107
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.503
    sort_std: 0.107
    global_rank: 510
    paper_rank: 510
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.5
    std: 0.082
    paper_value: 0.5
    paper_std: 0.082
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5
    true_std: 0.082
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5
    sort_std: 0.082
    global_rank: 513
    paper_rank: 513
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.495
    std: 0.067
    paper_value: 0.495
    paper_std: 0.067
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.495
    true_std: 0.067
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.495
    sort_std: 0.067
    global_rank: 515
    paper_rank: 515
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.489
    std: 0.062
    paper_value: 0.489
    paper_std: 0.062
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.489
    true_std: 0.062
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.489
    sort_std: 0.062
    global_rank: 518
    paper_rank: 518
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.47
    std: 0.075
    paper_value: 0.47
    paper_std: 0.075
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.47
    true_std: 0.075
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: 0.075
    global_rank: 526
    paper_rank: 526
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.468
    std: 0.066
    paper_value: 0.468
    paper_std: 0.066
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.468
    true_std: 0.066
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.468
    sort_std: 0.066
    global_rank: 527
    paper_rank: 527
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.414
    std: 0.054
    paper_value: 0.414
    paper_std: 0.054
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.414
    true_std: 0.054
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.414
    sort_std: 0.054
    global_rank: 560
    paper_rank: 560
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
- &id011
  dataset: Minesweeper
  rows:
  - model: Tango_GPS
    model_key: bunn
    model_plain: Tango_GPS
    value: 0.9899
    std: 0.0016
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.15540'
    title: Bundle Neural Networks for message diffusion on graphs
    date: May 24, 2024
    date_display: May 2024
    date_iso: '2024-05-24'
    venue: arXiv.org
    codebase_url: https://github.com/jacobbamberger/BuNN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9899
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: dc-gnn
    model_plain: Tango_GPS
    value: 0.985
    std: 0.0021
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
    sort_value: 0.985
    sort_std: 0.0021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.9839
    std: 0.0054
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9839
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.544
    std: 0.016
    paper_value: 0.544
    paper_std: 0.016
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.921
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.377
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9391
    true_std: 0.0035
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.3951
    has_value_note: false
    value_note: ''
    sort_value: 0.9391
    sort_std: 0.0035
    global_rank: 30
    paper_rank: 139
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.732
    std: 0.017
    paper_value: 0.732
    paper_std: 0.017
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9353
    at_pub_std: 0.005
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.20330000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9358
    true_std: 0.0005
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.20379999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9358
    sort_std: 0.0005
    global_rank: 36
    paper_rank: 119
    rank_delta: 83
    rank_delta_abs: 83
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.523
    std: 0.006
    paper_value: 0.523
    paper_std: 0.006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8975
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.37449999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.915
    true_std: 0.0006
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.392
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.0006
    global_rank: 59
    paper_rank: 140
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.551
    std: 0.032
    paper_value: 0.551
    paper_std: 0.032
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8782
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2406.06642'
    at_pub_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    at_pub_source_date_iso: '2024-06-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32719999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8782
    true_std: 0.0034
    value_gap_source_arxiv: '2406.06642'
    value_gap_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.32719999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8782
    sort_std: 0.0034
    global_rank: 94
    paper_rank: 139
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TopoBench: A Framework for Benchmarking Topological
      Deep Learning'
    comparison_source_arxiv: '2406.06642'
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.751
    std: 0.024
    paper_value: 0.751
    paper_std: 0.024
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.751
    true_std: 0.024
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: 0.024
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
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.745
    std: 0.023
    paper_value: 0.745
    paper_std: 0.023
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.745
    true_std: 0.023
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.023
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
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.731
    std: 0.019
    paper_value: 0.731
    paper_std: 0.019
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.731
    true_std: 0.019
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.731
    sort_std: 0.019
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
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.715
    std: 0.018
    paper_value: 0.715
    paper_std: 0.018
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.018
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.018
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.71
    std: 0.019
    paper_value: 0.71
    paper_std: 0.019
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.71
    true_std: 0.019
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: 0.019
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.684
    std: 0.014
    paper_value: 0.684
    paper_std: 0.014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.684
    true_std: 0.014
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.684
    sort_std: 0.014
    global_rank: 128
    paper_rank: 128
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.657
    std: 0.098
    paper_value: 0.657
    paper_std: 0.098
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.657
    true_std: 0.098
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.098
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
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.605
    std: 0.07
    paper_value: 0.605
    paper_std: 0.07
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.605
    true_std: 0.07
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.605
    sort_std: 0.07
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.582
    std: 0.046
    paper_value: 0.582
    paper_std: 0.046
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.582
    true_std: 0.046
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.582
    sort_std: 0.046
    global_rank: 137
    paper_rank: 137
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.573
    std: 0.01
    paper_value: 0.573
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.573
    true_std: 0.01
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.573
    sort_std: 0.01
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.555
    std: 0.032
    paper_value: 0.555
    paper_std: 0.032
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.555
    true_std: 0.032
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.555
    sort_std: 0.032
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.527
    std: 0.038
    paper_value: 0.527
    paper_std: 0.038
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.527
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.527
    sort_std: 0.038
    global_rank: 140
    paper_rank: 140
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
- &id001
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.881
    std: 0.005
    paper_value: 0.881
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8864
    at_pub_std: 0.003
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.00539999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9487
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06769999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9487
    sort_std: null
    global_rank: 9
    paper_rank: 175
    rank_delta: 166
    rank_delta_abs: 166
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.878
    std: 0.003
    paper_value: 0.878
    paper_std: 0.003
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
    source_ref: zhu2021graph_GNNhom2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8959
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2307.16026'
    at_pub_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.017900000000000027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9361
    true_std: 0.0013
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.05810000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: 0.0013
    global_rank: 19
    paper_rank: 187
    rank_delta: 168
    rank_delta_abs: 168
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MUSE: Multi-View Contrastive Learning for Heterophilic
      Graphs'
    comparison_source_arxiv: '2307.16026'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.885
    std: 0.005
    paper_value: 0.885
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.01200000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04459999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 149
    rank_delta: 128
    rank_delta_abs: 128
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.871
    std: 0.005
    paper_value: 0.871
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.026000000000000023
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05230000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 222
    rank_delta: 199
    rank_delta_abs: 199
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.907
    std: 0.005
    paper_value: 0.907
    paper_std: 0.005
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
    source_ref: acm_luan2022revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9096
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0025999999999999357
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9096
    true_std: 0.0062
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.0025999999999999357
    has_value_note: false
    value_note: ''
    sort_value: 0.9096
    sort_std: 0.0062
    global_rank: 45
    paper_rank: 53
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.9
    std: null
    paper_value: 0.9
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
    source_ref: pei2019geom_node_homophily
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9005
    at_pub_std: null
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9005
    true_std: null
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0004999999999999449
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: null
    global_rank: 84
    paper_rank: 87
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.851
    std: 0.001
    paper_value: 0.851
    paper_std: 0.001
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
    source_ref: chien2021adaptive_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8782
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.027200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8934
    true_std: 0.0025
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04239999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8934
    sort_std: 0.0025
    global_rank: 112
    paper_rank: 272
    rank_delta: 160
    rank_delta_abs: 160
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.893
    std: 0.004
    paper_value: 0.893
    paper_std: 0.004
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.004
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.889
    std: 0.004
    paper_value: 0.889
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.889
    true_std: 0.004
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.889
    sort_std: 0.004
    global_rank: 135
    paper_rank: 135
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.887
    std: 0.005
    paper_value: 0.887
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.887
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.005
    global_rank: 142
    paper_rank: 142
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.886
    std: 0.005
    paper_value: 0.886
    paper_std: 0.005
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
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.886
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.886
    sort_std: 0.005
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.882
    std: 0.005
    paper_value: 0.882
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.882
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.882
    sort_std: 0.005
    global_rank: 173
    paper_rank: 173
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
    value: 0.861
    std: 0.008
    paper_value: 0.861
    paper_std: 0.008
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.881
    at_pub_std: null
    at_pub_source_arxiv: '2308.10737'
    at_pub_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    at_pub_source_date_iso: '2023-08-21'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-21'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.020000000000000018
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: null
    value_gap_source_arxiv: '2308.10737'
    value_gap_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: null
    global_rank: 176
    paper_rank: 248
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UGSL: A Unified Framework for Benchmarking Graph Structure
      Learning'
    comparison_source_arxiv: '2308.10737'
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.878
    std: 0.007
    paper_value: 0.878
    paper_std: 0.007
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
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.878
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.878
    sort_std: 0.007
    global_rank: 189
    paper_rank: 189
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.877
    std: 0.005
    paper_value: 0.877
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.877
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.877
    sort_std: 0.005
    global_rank: 197
    paper_rank: 197
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.874
    std: 0.008
    paper_value: 0.874
    paper_std: 0.008
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.874
    true_std: 0.008
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.874
    sort_std: 0.008
    global_rank: 214
    paper_rank: 214
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.866
    std: 0.009
    paper_value: 0.866
    paper_std: 0.009
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
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.866
    true_std: 0.009
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.866
    sort_std: 0.009
    global_rank: 243
    paper_rank: 243
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.839
    std: 0.005
    paper_value: 0.839
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.005
    global_rank: 296
    paper_rank: 296
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.811
    std: 0.149
    paper_value: 0.811
    paper_std: 0.149
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.149
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.149
    global_rank: 388
    paper_rank: 388
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.796
    std: 0.009
    paper_value: 0.796
    paper_std: 0.009
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.796
    true_std: 0.009
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.009
    global_rank: 518
    paper_rank: 518
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMP
    model_key: acmp
    model_plain: ACMP
    value: 0.789
    std: 0.01
    paper_value: 0.789
    paper_std: 0.01
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
    source_ref: wang2023acmp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on Planetoid split
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.78
    at_pub_std: 0.003
    at_pub_source_arxiv: '2401.14580'
    at_pub_source_title: 'Design your own universe: a physics-informed agnostic method
      for enhancing graph neural networks'
    at_pub_source_date_iso: '2024-01-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.789
    true_std: 0.01
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.01
    global_rank: 635
    paper_rank: 635
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- &id009
  dataset: Questions
  rows:
  - model: Tango GPS
    model_key: graphsage + unigap
    model_plain: Tango GPS
    value: 0.8421
    std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
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
  - model: Tango GPS
    model_key: h2gcn + unigap
    model_plain: Tango GPS
    value: 0.8359
    std: 0.007
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8359
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango GPS
    model_key: gcn + unigap
    model_plain: Tango GPS
    value: 0.8273
    std: 0.009
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8273
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.532
    std: 0.004
    paper_value: 0.532
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7902
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2582
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
    value_gap: 0.2582
    has_value_note: false
    value_note: ''
    sort_value: 0.7902
    sort_std: 0.006
    global_rank: 17
    paper_rank: 161
    rank_delta: 144
    rank_delta_abs: 144
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
    value: 0.524
    std: 0.004
    paper_value: 0.524
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7743
    at_pub_std: 0.012
    at_pub_source_arxiv: '2403.12529'
    at_pub_source_title: Contextualized Messages Boost Graph Representations
    at_pub_source_date_iso: '2024-03-19'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.25029999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7743
    true_std: 0.012
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.25029999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7743
    sort_std: 0.012
    global_rank: 40
    paper_rank: 164
    rank_delta: 124
    rank_delta_abs: 124
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
    value: 0.56
    std: 0.008
    paper_value: 0.56
    paper_std: 0.008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7721
    at_pub_std: 0.013
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.21209999999999996
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
    value_gap: 0.21209999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: 0.013
    global_rank: 48
    paper_rank: 152
    rank_delta: 104
    rank_delta_abs: 104
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.518
    std: 0.03
    paper_value: 0.518
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.6776
    at_pub_std: null
    at_pub_source_arxiv: '2312.17679'
    at_pub_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    at_pub_source_date_iso: '2023-12-29'
    at_pub_source_date_label: LoG 2023
    value_gap_source_date_iso: '2023-12-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: 0.15959999999999996
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
    value_gap: 0.15959999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6776
    sort_std: null
    global_rank: 123
    paper_rank: 166
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Data Augmentation for Supervised Graph Outlier Detection
      via Latent Diffusion Models
    comparison_source_arxiv: '2312.17679'
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.593
    std: 0.039
    paper_value: 0.593
    paper_std: 0.039
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.593
    true_std: 0.039
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.593
    sort_std: 0.039
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.572
    std: 0.012
    paper_value: 0.572
    paper_std: 0.012
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.572
    true_std: 0.012
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.572
    sort_std: 0.012
    global_rank: 149
    paper_rank: 149
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.561
    std: 0.007
    paper_value: 0.561
    paper_std: 0.007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.561
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.561
    sort_std: 0.007
    global_rank: 152
    paper_rank: 152
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.557
    std: 0.007
    paper_value: 0.557
    paper_std: 0.007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.557
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.557
    sort_std: 0.007
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.557
    std: 0.046
    paper_value: 0.557
    paper_std: 0.046
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.557
    true_std: 0.046
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.557
    sort_std: 0.046
    global_rank: 156
    paper_rank: 156
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.548
    std: 0.009
    paper_value: 0.548
    paper_std: 0.009
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.548
    true_std: 0.009
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.548
    sort_std: 0.009
    global_rank: 158
    paper_rank: 158
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.531
    std: 0.006
    paper_value: 0.531
    paper_std: 0.006
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.531
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.531
    sort_std: 0.006
    global_rank: 162
    paper_rank: 162
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.53
    std: 0.007
    paper_value: 0.53
    paper_std: 0.007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.53
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.53
    sort_std: 0.007
    global_rank: 163
    paper_rank: 163
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.528
    std: 0.002
    paper_value: 0.528
    paper_std: 0.002
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.528
    true_std: 0.002
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.528
    sort_std: 0.002
    global_rank: 164
    paper_rank: 164
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.521
    std: 0.009
    paper_value: 0.521
    paper_std: 0.009
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
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
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.521
    sort_std: 0.009
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
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.513
    std: 0.008
    paper_value: 0.513
    paper_std: 0.008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.513
    true_std: 0.008
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.513
    sort_std: 0.008
    global_rank: 167
    paper_rank: 167
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.508
    std: 0.026
    paper_value: 0.508
    paper_std: 0.026
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.508
    true_std: 0.026
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.508
    sort_std: 0.026
    global_rank: 169
    paper_rank: 169
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
- &id007
  dataset: Roman-empire
  rows:
  - model: GPS + Mamba
    model_key: dir-nt
    model_plain: GPS + Mamba
    value: 0.9477
    std: 0.0031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9477
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: dir-poly
    model_plain: GPS + Mamba
    value: 0.9451
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9451
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: largescalenet
    model_plain: GPS + Mamba
    value: 0.9358
    std: 0.0024
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
    global_rank: 3
    sort_value: 0.9358
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.789
    std: 0.004
    paper_value: 0.789
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.858
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.06899999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9106
    true_std: 0.0027
    value_gap_source_arxiv: '2505.17939'
    value_gap_source_title: Directed Semi-Simplicial Learning with Applications to
      Brain Activity Decoding
    value_gap_source_is_current_paper: false
    value_gap: 0.12159999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9106
    sort_std: 0.0027
    global_rank: 27
    paper_rank: 98
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.471
    std: 0.006
    paper_value: 0.471
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8102
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.33920000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8875
    true_std: 0.0041
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.4165
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0041
    global_rank: 43
    paper_rank: 181
    rank_delta: 138
    rank_delta_abs: 138
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.478
    std: 0.008
    paper_value: 0.478
    paper_std: 0.008
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8272
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.34920000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7882
    true_std: 0.0009
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.31020000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7882
    sort_std: 0.0009
    global_rank: 99
    paper_rank: 181
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HyperAggregation: Aggregating over Graph Edges with
      Hypernetworks'
    comparison_source_arxiv: '2407.11596'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.787
    std: 0.007
    paper_value: 0.787
    paper_std: 0.007
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
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.787
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.787
    sort_std: 0.007
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.786
    std: 0.006
    paper_value: 0.786
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.786
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.786
    sort_std: 0.006
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.781
    std: 0.007
    paper_value: 0.781
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.781
    true_std: 0.007
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.781
    sort_std: 0.007
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.715
    std: 0.005
    paper_value: 0.715
    paper_std: 0.005
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
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.005
    global_rank: 127
    paper_rank: 127
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.689
    std: 0.009
    paper_value: 0.689
    paper_std: 0.009
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
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.689
    true_std: 0.009
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.009
    global_rank: 135
    paper_rank: 135
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.659
    std: 0.008
    paper_value: 0.659
    paper_std: 0.008
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.659
    true_std: 0.008
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.659
    sort_std: 0.008
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.64
    std: 0.01
    paper_value: 0.64
    paper_std: 0.01
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
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64
    true_std: 0.01
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: 0.01
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.602
    std: 0.005
    paper_value: 0.602
    paper_std: 0.005
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.602
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.602
    sort_std: 0.005
    global_rank: 163
    paper_rank: 163
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.586
    std: 0.011
    paper_value: 0.586
    paper_std: 0.011
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.586
    true_std: 0.011
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.586
    sort_std: 0.011
    global_rank: 168
    paper_rank: 168
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.576
    std: 0.01
    paper_value: 0.576
    paper_std: 0.01
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.576
    true_std: 0.01
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.576
    sort_std: 0.01
    global_rank: 171
    paper_rank: 171
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.566
    std: 0.006
    paper_value: 0.566
    paper_std: 0.006
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.566
    true_std: 0.006
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.566
    sort_std: 0.006
    global_rank: 174
    paper_rank: 174
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
    value: 0.482
    std: 0.012
    paper_value: 0.482
    paper_std: 0.012
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.568
    at_pub_std: 0.01
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.08599999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.482
    true_std: 0.012
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.482
    sort_std: 0.012
    global_rank: 180
    paper_rank: 180
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.48
    std: 0.013
    paper_value: 0.48
    paper_std: 0.013
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy (reported as ROC-AUC for binary labels)
      on standard split.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.48
    true_std: 0.013
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.48
    sort_std: 0.013
    global_rank: 181
    paper_rank: 181
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
- &id004
  dataset: Texas
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: gpf-plus
    model_plain: R-SoftGraphAIN
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.949
    std: 0.029
    paper_value: 0.949
    paper_std: 0.029
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
    source_ref: acm_luan2022revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.951
    at_pub_std: 0.032
    at_pub_source_arxiv: '2503.12563'
    at_pub_source_title: 'Diffusion on Graph: Augmentation of Graph Structure for
      Node Classification'
    at_pub_source_date_iso: '2025-03-16'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9557
    true_std: 0.036
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.006700000000000039
    has_value_note: false
    value_note: ''
    sort_value: 0.9557
    sort_std: 0.036
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.929
    std: 0.006
    paper_value: 0.929
    paper_std: 0.006
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
    source_ref: chien2021adaptive_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9295
    at_pub_std: 0.0131
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9292
    true_std: 0.0061
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.9292
    sort_std: 0.0061
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.79
    std: 0.012
    paper_value: 0.79
    paper_std: 0.012
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9001
    at_pub_std: 0.023
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.11009999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9001
    true_std: 0.023
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.11009999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9001
    sort_std: 0.023
    global_rank: 67
    paper_rank: 302
    rank_delta: 235
    rank_delta_abs: 235
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.859
    std: 0.035
    paper_value: 0.859
    paper_std: 0.035
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
    source_ref: zhu2021graph_GNNhom2
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.9189
    at_pub_std: 0.0393
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.059900000000000064
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8765
    true_std: null
    value_gap_source_arxiv: '2406.10863'
    value_gap_source_title: Global-Local Graph Neural Networks for Node-Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.01749999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8765
    sort_std: null
    global_rank: 101
    paper_rank: 143
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMP
    model_key: acmp
    model_plain: ACMP
    value: 0.862
    std: 0.03
    paper_value: 0.862
    paper_std: 0.03
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
    source_ref: wang2023acmp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.862
    at_pub_std: 0.03
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.862
    true_std: 0.03
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.862
    sort_std: 0.03
    global_rank: 128
    paper_rank: 128
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
    value: 0.578
    std: 0.046
    paper_value: 0.578
    paper_std: 0.046
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8082
    at_pub_std: 0.0213
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.23020000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.0645
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.23820000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.0645
    global_rank: 245
    paper_rank: 574
    rank_delta: 329
    rank_delta_abs: 329
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.797
    std: 0.059
    paper_value: 0.797
    paper_std: 0.059
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.797
    true_std: 0.059
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.059
    global_rank: 292
    paper_rank: 292
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
    value: 0.584
    std: 0.046
    paper_value: 0.584
    paper_std: 0.046
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7933
    at_pub_std: 0.0447
    at_pub_source_arxiv: '2505.20034'
    at_pub_source_title: Graph Wave Networks
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.20930000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7933
    true_std: 0.0447
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.20930000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0447
    global_rank: 299
    paper_rank: 561
    rank_delta: 262
    rank_delta_abs: 262
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Wave Networks
    comparison_source_arxiv: '2505.20034'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.759
    std: 0.068
    paper_value: 0.759
    paper_std: 0.068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.759
    true_std: 0.068
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.759
    sort_std: 0.068
    global_rank: 340
    paper_rank: 340
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
    value: 0.57
    std: 0.069
    paper_value: 0.57
    paper_std: 0.069
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.746
    at_pub_std: 0.008
    at_pub_source_arxiv: '2309.02769'
    at_pub_source_title: 'Unifying over-smoothing and over-squashing in graph neural
      networks: A physics informed approach and beyond'
    at_pub_source_date_iso: '2023-09-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.17600000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.746
    true_std: 0.008
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.17600000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.746
    sort_std: 0.008
    global_rank: 361
    paper_rank: 581
    rank_delta: 220
    rank_delta_abs: 220
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unifying over-smoothing and over-squashing in graph
      neural networks: A physics informed approach and beyond'
    comparison_source_arxiv: '2309.02769'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.705
    std: 0.055
    paper_value: 0.705
    paper_std: 0.055
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.705
    true_std: 0.055
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.705
    sort_std: 0.055
    global_rank: 412
    paper_rank: 412
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.676
    std: null
    paper_value: 0.676
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
    source_ref: pei2019geom_node_homophily
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.676
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.676
    true_std: null
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.676
    sort_std: null
    global_rank: 443
    paper_rank: 443
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.6
    std: 0.077
    paper_value: 0.6
    paper_std: 0.077
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6
    true_std: 0.077
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: 0.077
    global_rank: 531
    paper_rank: 531
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.597
    std: 0.055
    paper_value: 0.597
    paper_std: 0.055
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.597
    true_std: 0.055
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.597
    sort_std: 0.055
    global_rank: 536
    paper_rank: 536
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.595
    std: 0.049
    paper_value: 0.595
    paper_std: 0.049
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.595
    true_std: 0.049
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.595
    sort_std: 0.049
    global_rank: 538
    paper_rank: 538
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.595
    std: 0.08
    paper_value: 0.595
    paper_std: 0.08
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.595
    true_std: 0.08
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.595
    sort_std: 0.08
    global_rank: 539
    paper_rank: 539
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.592
    std: 0.047
    paper_value: 0.592
    paper_std: 0.047
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.047
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.047
    global_rank: 551
    paper_rank: 551
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.586
    std: 0.051
    paper_value: 0.586
    paper_std: 0.051
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.586
    true_std: 0.051
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.586
    sort_std: 0.051
    global_rank: 560
    paper_rank: 560
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.584
    std: 0.068
    paper_value: 0.584
    paper_std: 0.068
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.584
    true_std: 0.068
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.584
    sort_std: 0.068
    global_rank: 562
    paper_rank: 562
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.581
    std: 0.068
    paper_value: 0.581
    paper_std: 0.068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.581
    true_std: 0.068
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.581
    sort_std: 0.068
    global_rank: 568
    paper_rank: 568
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.568
    std: 0.053
    paper_value: 0.568
    paper_std: 0.053
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.568
    true_std: 0.053
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.568
    sort_std: 0.053
    global_rank: 584
    paper_rank: 584
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
- &id010
  dataset: Tolokers
  rows:
  - model: Schrödinger
    model_key: polynormer-r
    model_plain: Schrödinger
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
  - model: Schrödinger
    model_key: dc-gnn
    model_plain: Schrödinger
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
  - model: Schrödinger
    model_key: polynormer + wideformer
    model_plain: Schrödinger
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
    value: 0.57
    std: 0.027
    paper_value: 0.57
    paper_std: 0.027
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8443
    at_pub_std: 0.01
    at_pub_source_arxiv: '2406.06642'
    at_pub_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    at_pub_source_date_iso: '2024-06-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2743000000000001
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
    value_gap: 0.2743000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8443
    sort_std: 0.01
    global_rank: 17
    paper_rank: 137
    rank_delta: 120
    rank_delta_abs: 120
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
    value: 0.58
    std: 0.029
    paper_value: 0.58
    paper_std: 0.029
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8364
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.2564000000000001
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
    value_gap: 0.2564000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8364
    sort_std: 0.0067
    global_rank: 37
    paper_rank: 135
    rank_delta: 98
    rank_delta_abs: 98
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.605
    std: 0.016
    paper_value: 0.605
    paper_std: 0.016
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8243
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.21930000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8243
    true_std: 0.0044
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.21930000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8243
    sort_std: 0.0044
    global_rank: 65
    paper_rank: 130
    rank_delta: 65
    rank_delta_abs: 65
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.533
    std: 0.069
    paper_value: 0.533
    paper_std: 0.069
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8072
    at_pub_std: 0.0119
    at_pub_source_arxiv: '2406.06642'
    at_pub_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    at_pub_source_date_iso: '2024-06-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2742
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8072
    true_std: 0.0119
    value_gap_source_arxiv: '2406.06642'
    value_gap_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.2742
    has_value_note: false
    value_note: ''
    sort_value: 0.8072
    sort_std: 0.0119
    global_rank: 77
    paper_rank: 142
    rank_delta: 65
    rank_delta_abs: 65
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'TopoBench: A Framework for Benchmarking Topological
      Deep Learning'
    comparison_source_arxiv: '2406.06642'
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.624
    std: 0.027
    paper_value: 0.624
    paper_std: 0.027
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.624
    true_std: 0.027
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.624
    sort_std: 0.027
    global_rank: 129
    paper_rank: 129
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.597
    std: 0.015
    paper_value: 0.597
    paper_std: 0.015
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.597
    true_std: 0.015
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.597
    sort_std: 0.015
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
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.592
    std: 0.02
    paper_value: 0.592
    paper_std: 0.02
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.02
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.02
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.587
    std: 0.016
    paper_value: 0.587
    paper_std: 0.016
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.587
    true_std: 0.016
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.587
    sort_std: 0.016
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
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.577
    std: 0.032
    paper_value: 0.577
    paper_std: 0.032
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.577
    true_std: 0.032
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.577
    sort_std: 0.032
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.577
    std: 0.014
    paper_value: 0.577
    paper_std: 0.014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.577
    true_std: 0.014
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.577
    sort_std: 0.014
    global_rank: 137
    paper_rank: 137
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.563
    std: 0.07
    paper_value: 0.563
    paper_std: 0.07
    metric: ROC-AUC
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
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.563
    true_std: 0.07
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.563
    sort_std: 0.07
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.557
    std: 0.032
    paper_value: 0.557
    paper_std: 0.032
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.557
    true_std: 0.032
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.557
    sort_std: 0.032
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.551
    std: 0.011
    paper_value: 0.551
    paper_std: 0.011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.551
    true_std: 0.011
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.551
    sort_std: 0.011
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.537
    std: 0.058
    paper_value: 0.537
    paper_std: 0.058
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.537
    true_std: 0.058
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.537
    sort_std: 0.058
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
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.53
    std: 0.064
    paper_value: 0.53
    paper_std: 0.064
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.53
    true_std: 0.064
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.53
    sort_std: 0.064
    global_rank: 143
    paper_rank: 143
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.505
    std: 0.005
    paper_value: 0.505
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Binary classification task reported as ROC-AUC per caption.
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.505
    true_std: 0.005
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.505
    sort_std: 0.005
    global_rank: 145
    paper_rank: 145
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
- &id006
  dataset: Wisconsin
  rows:
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.958
    std: 0.02
    paper_value: 0.958
    paper_std: 0.02
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
    source_ref: acm_luan2022revisiting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8843
    at_pub_std: 0.0322
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.07369999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.02
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.02
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    comparison_source_arxiv: '2211.11761'
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.938
    std: 0.024
    paper_value: 0.938
    paper_std: 0.024
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
    source_ref: chien2021adaptive_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.899
    at_pub_std: 0.03
    at_pub_source_arxiv: '2410.05593'
    at_pub_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    at_pub_source_date_iso: '2024-10-08'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.038999999999999924
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.938
    true_std: 0.024
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.938
    sort_std: 0.024
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: dmd++
    model_plain: R-SoftGraphAIN
    value: 0.919
    std: 0.026
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.919
    sort_std: 0.026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.875
    std: 0.018
    paper_value: 0.875
    paper_std: 0.018
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
    source_ref: zhu2021graph_GNNhom3
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.879
    at_pub_std: 0.042
    at_pub_source_arxiv: '2410.05593'
    at_pub_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    at_pub_source_date_iso: '2024-10-08'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.879
    true_std: 0.042
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.042
    global_rank: 24
    paper_rank: 26
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMP
    model_key: acmp
    model_plain: ACMP
    value: 0.861
    std: 0.04
    paper_value: 0.861
    paper_std: 0.04
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
    source_ref: wang2023acmp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.861
    at_pub_std: 0.04
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.861
    true_std: 0.04
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.861
    sort_std: 0.04
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
  - model: GraphSAGE+mix.
    model_key: graphsage+mix.
    model_plain: GraphSAGE+mix.
    value: 0.845
    std: 0.011
    paper_value: 0.845
    paper_std: 0.011
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.011
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.011
    global_rank: 57
    paper_rank: 57
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
    value: 0.508
    std: 0.087
    paper_value: 0.508
    paper_std: 0.087
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.843
    at_pub_std: 0.037
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.33499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.843
    true_std: 0.037
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.33499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.843
    sort_std: 0.037
    global_rank: 62
    paper_rank: 225
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.524
    std: 0.06
    paper_value: 0.524
    paper_std: 0.06
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.831
    at_pub_std: 0.032
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.30699999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.032
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.30699999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.032
    global_rank: 74
    paper_rank: 216
    rank_delta: 142
    rank_delta_abs: 142
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.771
    std: 0.065
    paper_value: 0.771
    paper_std: 0.065
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.8118
    at_pub_std: 0.0556
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-02-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.04079999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8118
    true_std: 0.0556
    value_gap_source_arxiv: '2602.15634'
    value_gap_source_title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological
      Priors'
    value_gap_source_is_current_paper: false
    value_gap: 0.04079999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8118
    sort_std: 0.0556
    global_rank: 85
    paper_rank: 108
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+hom.
    model_key: graphsage+hom.
    model_plain: GraphSAGE+hom.
    value: 0.802
    std: 0.052
    paper_value: 0.802
    paper_std: 0.052
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.802
    true_std: 0.052
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.802
    sort_std: 0.052
    global_rank: 92
    paper_rank: 92
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE+het.
    model_key: graphsage+het.
    model_plain: GraphSAGE+het.
    value: 0.8
    std: 0.043
    paper_value: 0.8
    paper_std: 0.043
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: 0.043
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.043
    global_rank: 93
    paper_rank: 93
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
    value: 0.449
    std: 0.068
    paper_value: 0.449
    paper_std: 0.068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.7328
    at_pub_std: 0.0206
    at_pub_source_arxiv: '2405.18581'
    at_pub_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    at_pub_source_date_iso: '2024-05-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.2838
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.79
    true_std: 0.006
    value_gap_source_arxiv: '2505.11346'
    value_gap_source_title: What Can We Learn From MIMO Graph Convolutions?
    value_gap_source_is_current_paper: false
    value_gap: 0.341
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: 0.006
    global_rank: 100
    paper_rank: 234
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unleashing the Potential of Text-attributed Graphs:
      Automatic Relation Decomposition via Large Language Models'
    comparison_source_arxiv: '2405.18581'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.641
    std: null
    paper_value: 0.641
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
    source_ref: pei2019geom_node_homophily
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Comparison with other heterophily-aware GNNs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: 0.6757
    at_pub_std: null
    at_pub_source_arxiv: '2406.10863'
    at_pub_source_title: Global-Local Graph Neural Networks for Node-Classification
    at_pub_source_date_iso: '2024-06-01'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03469999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6757
    true_std: null
    value_gap_source_arxiv: '2406.10863'
    value_gap_source_title: Global-Local Graph Neural Networks for Node-Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.03469999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.6757
    sort_std: null
    global_rank: 152
    paper_rank: 164
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Global-Local Graph Neural Networks for Node-Classification
    comparison_source_arxiv: '2406.10863'
    is_best: false
    is_std_outlier: false
  - model: GAT+mix.
    model_key: gat+mix.
    model_plain: GAT+mix.
    value: 0.553
    std: 0.063
    paper_value: 0.553
    paper_std: 0.063
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.553
    true_std: 0.063
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.553
    sort_std: 0.063
    global_rank: 204
    paper_rank: 204
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+hom.
    model_key: gat+hom.
    model_plain: GAT+hom.
    value: 0.549
    std: 0.058
    paper_value: 0.549
    paper_std: 0.058
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.549
    true_std: 0.058
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.549
    sort_std: 0.058
    global_rank: 205
    paper_rank: 205
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+hom.
    model_key: gcn+hom.
    model_plain: GCN+hom.
    value: 0.545
    std: 0.033
    paper_value: 0.545
    paper_std: 0.033
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.545
    true_std: 0.033
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.545
    sort_std: 0.033
    global_rank: 207
    paper_rank: 207
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+het.
    model_key: gcn+het.
    model_plain: GCN+het.
    value: 0.539
    std: 0.038
    paper_value: 0.539
    paper_std: 0.038
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.539
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.539
    sort_std: 0.038
    global_rank: 209
    paper_rank: 209
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT+het.
    model_key: gat+het.
    model_plain: GAT+het.
    value: 0.533
    std: 0.068
    paper_value: 0.533
    paper_std: 0.068
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.533
    true_std: 0.068
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.533
    sort_std: 0.068
    global_rank: 212
    paper_rank: 212
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN+mix.
    model_key: gcn+mix.
    model_plain: GCN+mix.
    value: 0.52
    std: 0.061
    paper_value: 0.52
    paper_std: 0.061
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.52
    true_std: 0.061
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.52
    sort_std: 0.061
    global_rank: 220
    paper_rank: 220
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+het.
    model_key: gin+het.
    model_plain: GIN+het.
    value: 0.52
    std: 0.038
    paper_value: 0.52
    paper_std: 0.038
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.52
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.52
    sort_std: 0.038
    global_rank: 221
    paper_rank: 221
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+mix.
    model_key: gin+mix.
    model_plain: GIN+mix.
    value: 0.506
    std: 0.078
    paper_value: 0.506
    paper_std: 0.078
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
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.506
    true_std: 0.078
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.506
    sort_std: 0.078
    global_rank: 227
    paper_rank: 227
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN+hom.
    model_key: gin+hom.
    model_plain: GIN+hom.
    value: 0.49
    std: 0.063
    paper_value: 0.49
    paper_std: 0.063
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average of 10 random runs
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.49
    true_std: 0.063
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.49
    sort_std: 0.063
    global_rank: 232
    paper_rank: 232
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
  - *id002
  - *id003
- benchmark: Heterophilic Graphs
  datasets:
  - *id004
  - *id005
  - *id006
- benchmark: Heterophily Benchmark
  datasets:
  - *id007
  - *id008
  - *id009
  - *id010
  - *id011
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Wisconsin
      dataset_slug: wisconsin
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
    - dataset: Questions
      dataset_slug: questions
    - dataset: Tolokers
      dataset_slug: tolokers
    - dataset: Minesweeper
      dataset_slug: minesweeper
main_figure: /figures/2504.19785/main_figure.jpegoptim.jpg
---

