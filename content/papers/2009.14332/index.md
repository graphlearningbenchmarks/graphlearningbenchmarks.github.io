---
title: Multi-hop Attention Graph Neural Networks
arxiv_id: '2009.14332'
source_url: ''
authors:
- name: Guangtao Wang
  orcid: null
  s2_author_id: '2148300'
  s2_url: null
- name: Rex Ying
  orcid: null
  s2_author_id: '83539859'
  s2_url: null
- name: Jing Huang
  orcid: null
  s2_author_id: '30768523'
  s2_url: null
- name: J. Leskovec
  orcid: null
  s2_author_id: '1702139'
  s2_url: null
published_date: Sep 29, 2020
published_date_iso: '2020-09-29'
published_venue: IJCAI 2020
published_conference: IJCAI 2020
published_conference_short: IJCAI
published_conference_slug: ijcai
abstract: 'Self-attention mechanism in graph neural networks (GNNs) led to state-of-the-art
  performance on many graph representation learning tasks. Currently, at every layer,
  a node computes attention independently for each of its graph neighbors. However,
  such attention mechanism is limited as it does not consider nodes that are not connected
  by an edge but can provide important network context information. Here we propose
  Multi-hop Attention Graph Neural Network (MAGNA), a principled way to incorporate
  multi-hop context information into every layer of GNN attention computation. MAGNA
  diffuses the attention scores across the network, which increases the ``receptive
  field'''' for every layer of the GNN. Unlike previous approaches, MAGNA uses a diffusion
  prior on attention values, to efficiently account for all paths between the pair
  of not-connected nodes. We demonstrate theoretically and experimentally that MAGNA
  captures large-scale structural information in every layer, and has a low-pass effect
  that eliminates noisy high-frequency information from the graph. Experimental results
  on node classification as well as knowledge graph completion benchmarks show that
  MAGNA achieves state-of-the-art results: MAGNA achieves up to $5.7\'
codebase_url: https://github.com/xjtuwgt/GNN-MAGNA
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MAGNA + DistMult
- MAGNA
mrr: 0.0032
adjusted_mrr: 0.0032
mrr_dataset_count: 3
benchmark_categories:
- Classic
- Knowledge Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 2
  total: 3
task_categories:
- link_prediction
- node_classification
experiment_scopes:
- edge-level
- node-level
results:
- &id002
  dataset: CiteSeer
  rows:
  - model: SGC+TSC
    model_key: cna
    model_plain: SGC+TSC
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: is-gib
    model_plain: SGC+TSC
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: eerm
    model_plain: SGC+TSC
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.703
    std: null
    paper_value: 0.703
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.768
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.06500000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.17390000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 666
    rank_delta: 645
    rank_delta_abs: 645
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.711
    std: 0.004
    paper_value: 0.711
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.805
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.09400000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8142
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10320000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 610
    rank_delta: 581
    rank_delta_abs: 581
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
    value: 0.725
    std: 0.007
    paper_value: 0.725
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: velivckovic2017graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.786
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.061000000000000054
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08300000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 439
    rank_delta: 393
    rank_delta_abs: 393
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.698
    std: null
    paper_value: 0.698
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.792
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.09400000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.792
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09400000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: null
    global_rank: 77
    paper_rank: 691
    rank_delta: 614
    rank_delta_abs: 614
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: MAGNA
    model_key: magna
    model_plain: MAGNA
    value: 0.737
    std: 0.005
    paper_value: 0.737
    paper_std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.737
    true_std: 0.005
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: 0.005
    global_rank: 295
    paper_rank: 295
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diff-GCN
    model_key: diff-gcn
    model_plain: Diff-GCN
    value: 0.734
    std: 0.003
    paper_value: 0.734
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2019diffusion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.003
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.003
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
  - model: Diffusion-GCN (PPR)
    model_key: diffusion-gcn (ppr)
    model_plain: Diffusion-GCN (PPR)
    value: 0.734
    std: 0.003
    paper_value: 0.734
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: klicpera2019diffusion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.003
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.003
    global_rank: 332
    paper_rank: 332
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: g-U-Nets
    model_key: g-u-nets
    model_plain: g-U-Nets
    value: 0.732
    std: 0.005
    paper_value: 0.732
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gao2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.732
    at_pub_std: 0.005
    at_pub_source_arxiv: '1905.05178'
    at_pub_source_title: Graph U-Nets
    at_pub_source_date_iso: '2019-05-11'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.732
    true_std: 0.005
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.732
    sort_std: 0.005
    global_rank: 354
    paper_rank: 354
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGCN
    model_key: lgcn
    model_plain: LGCN
    value: 0.73
    std: 0.006
    paper_value: 0.73
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gao2018large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.73
    at_pub_std: 0.006
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2019-09-07'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.73
    true_std: 0.006
    value_gap_source_arxiv: '1909.03184'
    value_gap_source_title: 'Auto-GNN: Neural Architecture Search of Graph Neural
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: 0.006
    global_rank: 379
    paper_rank: 379
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DualGCN
    model_key: dualgcn
    model_plain: DualGCN
    value: 0.726
    std: null
    paper_value: 0.726
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
    source_ref: zhuang2018dual
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: null
    global_rank: 429
    paper_rank: 429
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: diffusion-gcn (ppr) + layernorm + ff
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.723
    std: 0.004
    paper_value: 0.723
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.723
    true_std: 0.004
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.004
    global_rank: 489
    paper_rank: 489
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cheby
    model_key: cheby
    model_plain: Cheby
    value: 0.698
    std: null
    paper_value: 0.698
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
    source_ref: defferrard2016convolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed split)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.702
    at_pub_std: 0.01
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-03-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.702
    true_std: 0.01
    value_gap_source_arxiv: '1903.02428'
    value_gap_source_title: Fast Graph Representation Learning with PyTorch Geometric
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.702
    sort_std: 0.01
    global_rank: 674
    paper_rank: 691
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.815
    std: null
    paper_value: 0.815
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.8717
    at_pub_std: 0.0058
    at_pub_source_arxiv: '1711.08920'
    at_pub_source_title: 'SplineCNN: Fast Geometric Deep Learning with Continuous
      B-Spline Kernels'
    at_pub_source_date_iso: '2017-11-24'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.056700000000000084
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08540000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 695
    rank_delta: 662
    rank_delta_abs: 662
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SplineCNN: Fast Geometric Deep Learning with Continuous
      B-Spline Kernels'
    comparison_source_arxiv: '1711.08920'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.843
    std: 0.002
    paper_value: 0.843
    paper_std: 0.002
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
    source_ref: klicpera2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.877
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03400000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8904
    true_std: 0.015
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0474
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 370
    rank_delta: 301
    rank_delta_abs: 301
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.811
    std: null
    paper_value: 0.811
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.887
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.07599999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.887
    true_std: 0.0
    value_gap_source_arxiv: '2009.09232'
    value_gap_source_title: Learned Low Precision Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07599999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.0
    global_rank: 88
    paper_rank: 725
    rank_delta: 637
    rank_delta_abs: 637
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: MAGNA
    model_key: magna
    model_plain: MAGNA
    value: 0.854
    std: 0.006
    paper_value: 0.854
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.854
    true_std: 0.006
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: 0.006
    global_rank: 294
    paper_rank: 294
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: g-U-Nets
    model_key: g-u-nets
    model_plain: g-U-Nets
    value: 0.844
    std: 0.006
    paper_value: 0.844
    paper_std: 0.006
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gao2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.844
    at_pub_std: 0.006
    at_pub_source_arxiv: '1905.05178'
    at_pub_source_title: Graph U-Nets
    at_pub_source_date_iso: '2019-05-11'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.844
    true_std: 0.006
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.844
    sort_std: 0.006
    global_rank: 360
    paper_rank: 360
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diff-GCN
    model_key: diff-gcn
    model_plain: Diff-GCN
    value: 0.836
    std: 0.002
    paper_value: 0.836
    paper_std: 0.002
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
    source_ref: klicpera2019diffusion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.002
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.002
    global_rank: 459
    paper_rank: 459
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diffusion-GCN (PPR)
    model_key: diffusion-gcn (ppr)
    model_plain: Diffusion-GCN (PPR)
    value: 0.836
    std: 0.002
    paper_value: 0.836
    paper_std: 0.002
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
    table_ref: Table 2
    source_ref: klicpera2019diffusion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.002
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.002
    global_rank: 469
    paper_rank: 469
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DualGCN
    model_key: dualgcn
    model_plain: DualGCN
    value: 0.835
    std: null
    paper_value: 0.835
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
    source_ref: zhuang2018dual
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.835
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: null
    global_rank: 477
    paper_rank: 477
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: diffusion-gcn (ppr) + layernorm + ff
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.834
    std: 0.004
    paper_value: 0.834
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.834
    true_std: 0.004
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.834
    sort_std: 0.004
    global_rank: 496
    paper_rank: 496
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGCN
    model_key: lgcn
    model_plain: LGCN
    value: 0.833
    std: 0.005
    paper_value: 0.833
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gao2018large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.833
    at_pub_std: 0.005
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2022-04-13'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.833
    true_std: 0.005
    value_gap_source_arxiv: '2204.06127'
    value_gap_source_title: 'Reinforcement learning on graphs: A survey'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.833
    sort_std: 0.005
    global_rank: 502
    paper_rank: 502
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT (hidden dimension = 512)
    model_key: gat (hidden dimension = 512)
    model_plain: GAT (hidden dimension = 512)
    value: 0.831
    std: 0.005
    paper_value: 0.831
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.831
    true_std: 0.005
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.005
    global_rank: 535
    paper_rank: 535
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cheby
    model_key: cheby
    model_plain: Cheby
    value: 0.812
    std: null
    paper_value: 0.812
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
    source_ref: defferrard2016convolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.812
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.812
    sort_std: null
    global_rank: 717
    paper_rank: 717
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
  dataset: FB15k-237
  rows:
  - model: CompGCN
    model_key: llms
    model_plain: CompGCN
    value: 0.815
    std: 0.023
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted by ICLR'26, 41 pages
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.815
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: gcope
    model_plain: CompGCN
    value: 0.793
    std: 0.022
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted by ICLR'26, 41 pages
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.793
    sort_std: 0.022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    value: 0.791
    std: 0.016
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted by ICLR'26, 41 pages
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.791
    sort_std: 0.016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAGNA + DistMult
    model_key: magna + distmult
    model_plain: MAGNA + DistMult
    value: 0.369
    std: null
    paper_value: 0.369
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.369
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: QuatE
    model_key: quate
    model_plain: QuatE
    value: 0.366
    std: null
    paper_value: 0.366
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhang2019quaternion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.366
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.366
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
  - model: CoKE
    model_key: coke
    model_plain: CoKE
    value: 0.361
    std: null
    paper_value: 0.361
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wang2019CoKE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.364
    true_std: null
    value_gap_source_arxiv: '2205.14209'
    value_gap_source_title: 'StarGraph: Knowledge Representation Learning based on
      Incomplete Two-hop Subgraph'
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.364
    sort_std: null
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OTE
    model_key: ote
    model_plain: OTE
    value: 0.361
    std: null
    paper_value: 0.361
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tang2019orthogonal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.361
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.361
    sort_std: null
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSF
    model_key: autosf
    model_plain: AutoSF
    value: 0.36
    std: null
    paper_value: 0.36
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhang2020autosf
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.36
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.36
    sort_std: null
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TuckER
    model_key: tucker
    model_plain: TuckER
    value: 0.358
    std: null
    paper_value: 0.358
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: balazevic2019tucker
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.358
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.358
    sort_std: null
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SACN
    model_key: sacn
    model_plain: SACN
    value: 0.35
    std: null
    paper_value: 0.35
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: shang2019end
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.35
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.35
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.35
    sort_std: null
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.247
    std: null
    paper_value: 0.247
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: trouillon2016complex
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.247
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.346
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: 0.09899999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.346
    sort_std: null
    global_rank: 42
    paper_rank: 74
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ROTH
    model_key: roth
    model_plain: ROTH
    value: 0.344
    std: null
    paper_value: 0.344
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chami2020low
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.344
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.344
    sort_std: null
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RotatE
    model_key: rotate
    model_plain: RotatE
    value: 0.338
    std: null
    paper_value: 0.338
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: sun2019rotate
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.338
    at_pub_std: null
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.338
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.338
    sort_std: null
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConvE
    model_key: conve
    model_plain: ConvE
    value: 0.325
    std: null
    paper_value: 0.325
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: dettmers2018convolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.325
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.325
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.325
    sort_std: null
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A2N
    model_key: a2n
    model_plain: A2N
    value: 0.317
    std: null
    paper_value: 0.317
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bansal2019a2n
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.317
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.317
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.294
    std: null
    paper_value: 0.294
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bordes2013translating
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.294
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.294
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.294
    sort_std: null
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
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.249
    std: null
    paper_value: 0.249
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schlichtkrull2018modeling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.248
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.249
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.249
    sort_std: null
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Knowledge Graphs
    comparison_source_arxiv: '1707.01476'
    is_best: false
    is_std_outlier: false
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.241
    std: null
    paper_value: 0.241
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2014embedding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on FB15k-237 using Toutanova & Chen 2015 split.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.241
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.241
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.241
    sort_std: null
    global_rank: 76
    paper_rank: 76
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
- &id003
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.797
    std: 0.003
    paper_value: 0.797
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.905
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10799999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9355
    true_std: 0.006
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.13849999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9355
    sort_std: 0.006
    global_rank: 20
    paper_rank: 504
    rank_delta: 484
    rank_delta_abs: 484
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.79
    std: null
    paper_value: 0.79
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10699999999999998
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
    value_gap: 0.13959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 611
    rank_delta: 590
    rank_delta_abs: 590
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
    value: 0.79
    std: 0.003
    paper_value: 0.79
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: velivckovic2017graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10699999999999998
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
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 611
    rank_delta: 588
    rank_delta_abs: 588
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.781
    std: null
    paper_value: 0.781
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.916
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.135
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.916
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.135
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: null
    global_rank: 27
    paper_rank: 702
    rank_delta: 675
    rank_delta_abs: 675
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: MAGNA
    model_key: magna
    model_plain: MAGNA
    value: 0.814
    std: 0.002
    paper_value: 0.814
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.002
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.002
    global_rank: 368
    paper_rank: 368
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DualGCN
    model_key: dualgcn
    model_plain: DualGCN
    value: 0.8
    std: null
    paper_value: 0.8
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
    source_ref: zhuang2018dual
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: null
    global_rank: 474
    paper_rank: 474
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diff-GCN
    model_key: diff-gcn
    model_plain: Diff-GCN
    value: 0.796
    std: 0.004
    paper_value: 0.796
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2019diffusion
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.796
    true_std: 0.004
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.004
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
  - model: g-U-Nets
    model_key: g-u-nets
    model_plain: g-U-Nets
    value: 0.796
    std: 0.002
    paper_value: 0.796
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: gao2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.796
    at_pub_std: 0.002
    at_pub_source_arxiv: '1905.05178'
    at_pub_source_title: Graph U-Nets
    at_pub_source_date_iso: '2019-05-11'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.796
    true_std: 0.002
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.002
    global_rank: 516
    paper_rank: 516
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGCN
    model_key: lgcn
    model_plain: LGCN
    value: 0.795
    std: 0.002
    paper_value: 0.795
    paper_std: 0.002
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
    source_ref: gao2018large
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.795
    at_pub_std: 0.002
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2019-09-07'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.795
    true_std: 0.002
    value_gap_source_arxiv: '1909.03184'
    value_gap_source_title: 'Auto-GNN: Neural Architecture Search of Graph Neural
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.795
    sort_std: 0.002
    global_rank: 528
    paper_rank: 528
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cheby
    model_key: cheby
    model_plain: Cheby
    value: 0.744
    std: null
    paper_value: 0.744
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
    source_ref: defferrard2016convolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.784
    at_pub_std: 0.004
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-03-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.040000000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.784
    true_std: 0.004
    value_gap_source_arxiv: '1903.02428'
    value_gap_source_title: Fast Graph Representation Learning with PyTorch Geometric
    value_gap_source_is_current_paper: false
    value_gap: 0.040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.004
    global_rank: 685
    paper_rank: 835
    rank_delta: 150
    rank_delta_abs: 150
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: diffusion-gcn (ppr) + layernorm + ff
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
    value: 0.781
    std: 0.005
    paper_value: 0.781
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016)
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.781
    true_std: 0.005
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.781
    sort_std: 0.005
    global_rank: 706
    paper_rank: 706
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
  dataset: WN18RR
  rows:
  - model: CompGCN
    model_key: gft
    model_plain: CompGCN
    value: 0.9191
    std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_display: Nov 2024
    date_iso: '2024-11-09'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Zehong-Wang/GFT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9191
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CompGCN
    model_key: unigraph2
    model_plain: CompGCN
    value: 0.8786
    std: 0.0006
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.00806'
    title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
    date: Feb 2, 2025
    date_display: Feb 2025
    date_iso: '2025-02-02'
    venue: The Web Conference
    codebase_url: https://github.com/yf-he/UniGraph2
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8786
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CompGCN
    model_key: gat
    model_plain: CompGCN
    value: 0.8552
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
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: Accepted by NeurIPS 2025
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8552
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNA + DistMult
    model_key: magna + distmult
    model_plain: MAGNA + DistMult
    value: 0.502
    std: null
    paper_value: 0.502
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: MAGNA uses its own embeddings... achieves drastic improvements
      over using the corresponding DistMult embeddings.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.502
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.502
    sort_std: null
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ROTH
    model_key: roth
    model_plain: ROTH
    value: 0.496
    std: null
    paper_value: 0.496
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Chami 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.496
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.496
    sort_std: null
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
  - model: OTE
    model_key: ote
    model_plain: OTE
    value: 0.491
    std: null
    paper_value: 0.491
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Tang 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.491
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.491
    sort_std: null
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoSF
    model_key: autosf
    model_plain: AutoSF
    value: 0.49
    std: null
    paper_value: 0.49
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Zhang 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.49
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.49
    sort_std: null
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: QuatE
    model_key: quate
    model_plain: QuatE
    value: 0.488
    std: null
    paper_value: 0.488
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Zhang 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.488
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: null
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RotatE
    model_key: rotate
    model_plain: RotatE
    value: 0.476
    std: null
    paper_value: 0.476
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Sun 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.477
    at_pub_std: 0.001
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2018-09-27'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.477
    true_std: 0.001
    value_gap_source_arxiv: '1902.10197'
    value_gap_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.477
    sort_std: 0.001
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    comparison_source_arxiv: '1902.10197'
    is_best: false
    is_std_outlier: false
  - model: CoKE
    model_key: coke
    model_plain: CoKE
    value: 0.475
    std: null
    paper_value: 0.475
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Wang 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.475
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.475
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TuckER
    model_key: tucker
    model_plain: TuckER
    value: 0.47
    std: null
    paper_value: 0.47
    paper_std: null
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Balazevic 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.47
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: null
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SACN
    model_key: sacn
    model_plain: SACN
    value: 0.47
    std: null
    paper_value: 0.47
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Shang 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.47
    at_pub_std: null
    at_pub_source_arxiv: '1911.03082'
    at_pub_source_title: Composition-based Multi-Relational Graph Convolutional Networks
    at_pub_source_date_iso: '2019-11-08'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.47
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.47
    sort_std: null
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ConvE
    model_key: conve
    model_plain: ConvE
    value: 0.43
    std: null
    paper_value: 0.43
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Dettmers 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.43
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2023-02-25'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.462
    true_std: null
    value_gap_source_arxiv: '2302.13083'
    value_gap_source_title: Knowledge Graph Completion with Counterfactual Augmentation
    value_gap_source_is_current_paper: false
    value_gap: 0.03200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.462
    sort_std: null
    global_rank: 58
    paper_rank: 69
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A2N
    model_key: a2n
    model_plain: A2N
    value: 0.45
    std: null
    paper_value: 0.45
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Bansal 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-29'
    value_gap_source_date_label: IJCAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.45
    true_std: null
    value_gap_source_arxiv: '2009.14332'
    value_gap_source_title: Multi-hop Attention Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.45
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ComplEx
    model_key: complex
    model_plain: ComplEx
    value: 0.44
    std: null
    paper_value: 0.44
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Trouillon 2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.44
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.44
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.44
    sort_std: null
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DistMult
    model_key: distmult
    model_plain: DistMult
    value: 0.43
    std: null
    paper_value: 0.43
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Yang 2014
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.43
    at_pub_std: null
    at_pub_source_arxiv: '1707.01476'
    at_pub_source_title: Knowledge Graphs
    at_pub_source_date_iso: '2017-07-05'
    at_pub_source_date_label: AAAI 2017
    value_gap_source_date_iso: '2019-11-08'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.43
    true_std: null
    value_gap_source_arxiv: '1911.03082'
    value_gap_source_title: Composition-based Multi-Relational Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.43
    sort_std: null
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
  - model: TransE
    model_key: transe
    model_plain: TransE
    value: 0.226
    std: null
    paper_value: 0.226
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Bordes 2013
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on WN18RR test split using MRR metric.
    date: Sep 29, 2020
    date_display: Sep 2020
    date_iso: '2020-09-29'
    published_venue: IJCAI 2020
    published_conference: IJCAI 2020
    at_pub_value: 0.226
    at_pub_std: null
    at_pub_source_arxiv: '1902.10197'
    at_pub_source_title: 'RotatE: Knowledge Graph Embedding by Relational Rotation
      in Complex Space'
    at_pub_source_date_iso: '2018-09-27'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2022-12-12'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.231
    true_std: null
    value_gap_source_arxiv: '2212.05767'
    value_gap_source_title: 'A Survey of Knowledge Graph Reasoning on Graph Types:
      Static, Dynamic, and Multi-Modal'
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.231
    sort_std: null
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: Knowledge Graphs
  datasets:
  - *id004
  - *id005
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
    - dataset: PubMed
      dataset_slug: pubmed
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
    - dataset: FB15k-237
      dataset_slug: fb15k-237
main_figure: /figures/2009.14332/main_figure.jpegoptim.jpg
---

