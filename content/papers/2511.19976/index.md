---
title: Rethinking Semi-Supervised Node Classification with Self-Supervised Graph Clustering
arxiv_id: '2511.19976'
source_url: ''
authors:
- name: Songbo Wang
  orcid: null
  s2_author_id: '2117075393'
  s2_url: null
- name: Renchi Yang
  orcid: null
  s2_author_id: '2335817338'
  s2_url: null
- name: Yurui Lai
  orcid: null
  s2_author_id: '2308073125'
  s2_url: null
- name: Xiaoyang Lin
  orcid: null
  s2_author_id: '2302390655'
  s2_url: null
- name: Tsz Nam Chan
  orcid: null
  s2_author_id: '2610571'
  s2_url: null
published_date: Nov 25, 2025
published_date_iso: '2025-11-25'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: The emergence of graph neural networks (GNNs) has offered a powerful tool
  for semi-supervised node classification tasks. Subsequent studies have achieved
  further improvements through refining the message passing schemes in GNN models
  or exploiting various data augmentation techniques to mitigate limited supervision.
  In real graphs, nodes often tend to form tightly-knit communities/clusters, which
  embody abundant signals for compensating label scarcity in semi-supervised node
  classification but are not explored in prior methods. Inspired by this, this paper
  presents NCGC that integrates self-supervised graph clustering and semi-supervised
  classification into a unified framework. Firstly, we theoretically unify the optimization
  objectives of GNNs and spectral graph clustering, and based on that, develop soft
  orthogonal GNNs (SOGNs) that leverage a refined message passing paradigm to generate
  node representations for both classification and clustering. On top of that, NCGC
  includes a self-supervised graph clustering module that enables the training of
  SOGNs for learning representations of unlabeled nodes in a self-supervised manner.
  Particularly, this component comprises two non-trivial clustering objectives and
  a Sinkhorn-Knopp normalization that transforms predicted cluster assignments into
  balanced soft pseudo-labels. Through combining the foregoing clustering module with
  the classification model using a multi-task objective containing the supervised
  classification loss on labeled data and self-supervised clustering loss on unlabeled
  data, NCGC promotes synergy between them and achieves enhanced model capacity. Our
  extensive experiments showcase that the proposed NCGC framework consistently and
  considerably outperforms popular GNN models and recent baselines for semi-supervised
  node classification on seven real graphs, when working with various classic GNN
  backbones.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN*
- NCGC (GCN)
- NCGC (GCNII)
- NCGC (GAT)
mrr: 0.1332
adjusted_mrr: 0.1332
mrr_dataset_count: 6
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 5
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Amazon-Computers
  rows:
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN*
    model_key: gcn
    model_plain: GCN*
    value: 0.8111
    std: 0.016
    paper_value: 0.8111
    paper_std: 0.016
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.916
    at_pub_std: 0.016
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1049
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.1301
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 457
    rank_delta: 455
    rank_delta_abs: 455
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GAT*
    model_key: gat
    model_plain: GAT*
    value: 0.8136
    std: 0.0143
    paper_value: 0.8136
    paper_std: 0.0143
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.924
    at_pub_std: 0.013
    at_pub_source_arxiv: '2410.02622'
    at_pub_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.11040000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.12619999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 451
    rank_delta: 448
    rank_delta_abs: 448
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic
      Transforms'
    comparison_source_arxiv: '2410.02622'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE*
    model_key: graphsage
    model_plain: GraphSAGE*
    value: 0.821
    std: 0.0139
    paper_value: 0.821
    paper_std: 0.0139
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.912
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.09100000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.912
    true_std: 0.0029
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.09100000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.912
    sort_std: 0.0029
    global_rank: 62
    paper_rank: 436
    rank_delta: 374
    rank_delta_abs: 374
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7472
    std: 0.0503
    paper_value: 0.7472
    paper_std: 0.0503
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
    source_ref: chen2020simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9104
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1632
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9104
    true_std: 0.0041
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.1632
    has_value_note: false
    value_note: ''
    sort_value: 0.9104
    sort_std: 0.0041
    global_rank: 73
    paper_rank: 488
    rank_delta: 415
    rank_delta_abs: 415
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.7311
    std: 0.0025
    paper_value: 0.7311
    paper_std: 0.0025
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
    source_ref: gasteiger2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9093
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.17820000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9093
    true_std: 0.0018
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.17820000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9093
    sort_std: 0.0018
    global_rank: 84
    paper_rank: 494
    rank_delta: 410
    rank_delta_abs: 410
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7284
    std: 0.0148
    paper_value: 0.7284
    paper_std: 0.0148
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9022
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.17379999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9022
    true_std: 0.0021
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.17379999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9022
    sort_std: 0.0021
    global_rank: 113
    paper_rank: 496
    rank_delta: 383
    rank_delta_abs: 383
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.6976
    std: 0.0052
    paper_value: 0.6976
    paper_std: 0.0052
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
    source_ref: feng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8937
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2505.20034'
    at_pub_source_title: Graph Wave Networks
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.19610000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8937
    true_std: 0.0041
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.19610000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8937
    sort_std: 0.0041
    global_rank: 176
    paper_rank: 509
    rank_delta: 333
    rank_delta_abs: 333
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Wave Networks
    comparison_source_arxiv: '2505.20034'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.7952
    std: 0.02
    paper_value: 0.7952
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
    source_ref: Chien21adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8763
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2306.07608'
    at_pub_source_title: 'Finding the Missing-half: Graph Complementary Learning for
      Homophily-prone and Heterophily-prone Graphs'
    at_pub_source_date_iso: '2023-06-13'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-13'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.08109999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8763
    true_std: 0.0048
    value_gap_source_arxiv: '2306.07608'
    value_gap_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.08109999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8763
    sort_std: 0.0048
    global_rank: 281
    paper_rank: 470
    rank_delta: 189
    rank_delta_abs: 189
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    comparison_source_arxiv: '2306.07608'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.8045
    std: 0.0053
    paper_value: 0.8045
    paper_std: 0.0053
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.876
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.07150000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.876
    true_std: 0.0
    value_gap_source_arxiv: '2009.09232'
    value_gap_source_title: Learned Low Precision Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07150000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.876
    sort_std: 0.0
    global_rank: 283
    paper_rank: 464
    rank_delta: 181
    rank_delta_abs: 181
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.8081
    std: 0.0093
    paper_value: 0.8081
    paper_std: 0.0093
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
    source_ref: liu2020towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.845
    at_pub_std: 0.012
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-06'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.03689999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.845
    true_std: 0.012
    value_gap_source_arxiv: '2007.09296'
    value_gap_source_title: Towards Deeper Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03689999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.012
    global_rank: 362
    paper_rank: 460
    rank_delta: 98
    rank_delta_abs: 98
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Deeper Graph Neural Networks
    comparison_source_arxiv: '2007.09296'
    is_best: false
    is_std_outlier: false
  - model: NCGC (GAT)
    model_key: ncgc (gat)
    model_plain: NCGC (GAT)
    value: 0.8401
    std: 0.0094
    paper_value: 0.8401
    paper_std: 0.0094
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8401
    true_std: 0.0094
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8401
    sort_std: 0.0094
    global_rank: 386
    paper_rank: 386
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.5477
    std: 0.0234
    paper_value: 0.5477
    paper_std: 0.0234
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
    source_ref: yang2024mixed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8399
    at_pub_std: 0.009
    at_pub_source_arxiv: '2206.02796'
    at_pub_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2922
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8399
    true_std: 0.009
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.2922
    has_value_note: false
    value_note: ''
    sort_value: 0.8399
    sort_std: 0.009
    global_rank: 389
    paper_rank: 523
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    comparison_source_arxiv: '2206.02796'
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.8164
    std: 0.0036
    paper_value: 0.8164
    paper_std: 0.0036
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
    source_ref: stretcu2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8164
    true_std: 0.0036
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8164
    sort_std: 0.0036
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
  - model: PTA
    model_key: pta
    model_plain: PTA
    value: 0.5541
    std: 0.0279
    paper_value: 0.5541
    paper_std: 0.0279
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
    source_ref: dong2021equivalence
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8162
    at_pub_std: 0.0167
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.2621
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.0167
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.2621
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.0167
    global_rank: 448
    paper_rank: 523
    rank_delta: 75
    rank_delta_abs: 75
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    comparison_source_arxiv: '2507.14484'
    is_best: false
    is_std_outlier: false
  - model: M3S
    model_key: m3s
    model_plain: M3S
    value: 0.7592
    std: 0.0107
    paper_value: 0.7592
    paper_std: 0.0107
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
    source_ref: sun2020multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7592
    true_std: 0.0107
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7592
    sort_std: 0.0107
    global_rank: 483
    paper_rank: 483
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.7298
    std: 0.0464
    paper_value: 0.7298
    paper_std: 0.0464
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
    source_ref: zhang2025normalize
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7298
    true_std: 0.0464
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7298
    sort_std: 0.0464
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
    is_std_outlier: true
  - model: Meta-PN
    model_key: meta-pn
    model_plain: Meta-PN
    value: 0.7246
    std: 0.0732
    paper_value: 0.7246
    paper_std: 0.0732
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
    source_ref: ding2022meta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7246
    true_std: 0.0732
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7246
    sort_std: 0.0732
    global_rank: 498
    paper_rank: 498
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.7154
    std: 0.0045
    paper_value: 0.7154
    paper_std: 0.0045
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
    source_ref: verma2021graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7154
    true_std: 0.0045
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7154
    sort_std: 0.0045
    global_rank: 500
    paper_rank: 500
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
- &id003
  dataset: Amazon-Photo
  rows:
  - model: C (orthogonal)
    model_key: msh-gnn
    model_plain: C (orthogonal)
    value: 0.9766
    std: 0.005
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
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: geomancer
    model_plain: C (orthogonal)
    value: 0.9705
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    global_rank: 3
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT*
    model_key: gat
    model_plain: GAT*
    value: 0.9143
    std: 0.0015
    paper_value: 0.9143
    paper_std: 0.0015
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9498
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.035499999999999976
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.05259999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 5
    paper_rank: 365
    rank_delta: 360
    rank_delta_abs: 360
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GCN*
    model_key: gcn
    model_plain: GCN*
    value: 0.9034
    std: 0.0084
    paper_value: 0.9034
    paper_std: 0.0084
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9476
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.04420000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.059799999999999964
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 16
    paper_rank: 422
    rank_delta: 406
    rank_delta_abs: 406
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.8275
    std: 0.0038
    paper_value: 0.8275
    paper_std: 0.0038
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
    source_ref: feng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9579
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2505.20034'
    at_pub_source_title: Graph Wave Networks
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.13039999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9579
    true_std: 0.0059
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.13039999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9579
    sort_std: 0.0059
    global_rank: 25
    paper_rank: 497
    rank_delta: 472
    rank_delta_abs: 472
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Wave Networks
    comparison_source_arxiv: '2505.20034'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8698
    std: 0.002
    paper_value: 0.8698
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: gasteiger2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9573
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08750000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9573
    true_std: 0.0012
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.08750000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9573
    sort_std: 0.0012
    global_rank: 27
    paper_rank: 476
    rank_delta: 449
    rank_delta_abs: 449
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8451
    std: 0.004
    paper_value: 0.8451
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
    table_ref: Table 2
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9511
    at_pub_std: 0.0009
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10599999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9511
    true_std: 0.0009
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.10599999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9511
    sort_std: 0.0009
    global_rank: 66
    paper_rank: 488
    rank_delta: 422
    rank_delta_abs: 422
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE*
    model_key: graphsage
    model_plain: GraphSAGE*
    value: 0.9115
    std: 0.0055
    paper_value: 0.9115
    paper_std: 0.0055
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9508
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0393
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9508
    true_std: 0.0026
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0393
    has_value_note: false
    value_note: ''
    sort_value: 0.9508
    sort_std: 0.0026
    global_rank: 71
    paper_rank: 386
    rank_delta: 315
    rank_delta_abs: 315
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.9081
    std: 0.0018
    paper_value: 0.9081
    paper_std: 0.0018
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
    source_ref: Chien21adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.946
    at_pub_std: 0.003
    at_pub_source_arxiv: '2306.07608'
    at_pub_source_title: 'Finding the Missing-half: Graph Complementary Learning for
      Homophily-prone and Heterophily-prone Graphs'
    at_pub_source_date_iso: '2023-06-13'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-13'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.037899999999999934
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.946
    true_std: 0.003
    value_gap_source_arxiv: '2306.07608'
    value_gap_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.037899999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.946
    sort_std: 0.003
    global_rank: 93
    paper_rank: 393
    rank_delta: 300
    rank_delta_abs: 300
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    comparison_source_arxiv: '2306.07608'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.8778
    std: 0.0148
    paper_value: 0.8778
    paper_std: 0.0148
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
    source_ref: chen2020simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.943
    at_pub_std: 0.002
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.06519999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.943
    true_std: 0.002
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.06519999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.943
    sort_std: 0.002
    global_rank: 110
    paper_rank: 471
    rank_delta: 361
    rank_delta_abs: 361
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: NCGC (GAT)
    model_key: ncgc (gat)
    model_plain: NCGC (GAT)
    value: 0.9274
    std: 0.0038
    paper_value: 0.9274
    paper_std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9274
    true_std: 0.0038
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9274
    sort_std: 0.0038
    global_rank: 256
    paper_rank: 256
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.9078
    std: 0.0022
    paper_value: 0.9078
    paper_std: 0.0022
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
    source_ref: liu2020towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9269
    at_pub_std: null
    at_pub_source_arxiv: '2012.03476'
    at_pub_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    at_pub_source_date_iso: '2020-12-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.019099999999999895
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9269
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.019099999999999895
    has_value_note: false
    value_note: ''
    sort_value: 0.9269
    sort_std: null
    global_rank: 260
    paper_rank: 396
    rank_delta: 136
    rank_delta_abs: 136
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    comparison_source_arxiv: '2012.03476'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.8976
    std: 0.0012
    paper_value: 0.8976
    paper_std: 0.0012
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9268
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2306.07608'
    at_pub_source_title: 'Finding the Missing-half: Graph Complementary Learning for
      Homophily-prone and Heterophily-prone Graphs'
    at_pub_source_date_iso: '2023-06-13'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-13'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.029200000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9268
    true_std: 0.0058
    value_gap_source_arxiv: '2306.07608'
    value_gap_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.029200000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9268
    sort_std: 0.0058
    global_rank: 262
    paper_rank: 438
    rank_delta: 176
    rank_delta_abs: 176
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    comparison_source_arxiv: '2306.07608'
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.9056
    std: 0.0062
    paper_value: 0.9056
    paper_std: 0.0062
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
    source_ref: yang2024mixed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9264
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2206.02796'
    at_pub_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02080000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9264
    true_std: 0.0024
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.02080000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9264
    sort_std: 0.0024
    global_rank: 266
    paper_rank: 408
    rank_delta: 142
    rank_delta_abs: 142
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    comparison_source_arxiv: '2206.02796'
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.9193
    std: 0.0044
    paper_value: 0.9193
    paper_std: 0.0044
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
    source_ref: zhang2025normalize
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9193
    true_std: 0.0044
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9193
    sort_std: 0.0044
    global_rank: 335
    paper_rank: 335
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.9123
    std: 0.0032
    paper_value: 0.9123
    paper_std: 0.0032
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
    source_ref: stretcu2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9123
    true_std: 0.0032
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9123
    sort_std: 0.0032
    global_rank: 382
    paper_rank: 382
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PTA
    model_key: pta
    model_plain: PTA
    value: 0.7417
    std: 0.0157
    paper_value: 0.7417
    paper_std: 0.0157
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
    source_ref: dong2021equivalence
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9011
    at_pub_std: 0.0152
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1594
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9011
    true_std: 0.0152
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.1594
    has_value_note: false
    value_note: ''
    sort_value: 0.9011
    sort_std: 0.0152
    global_rank: 427
    paper_rank: 518
    rank_delta: 91
    rank_delta_abs: 91
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    comparison_source_arxiv: '2507.14484'
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.8845
    std: 0.0076
    paper_value: 0.8845
    paper_std: 0.0076
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
    source_ref: verma2021graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8845
    true_std: 0.0076
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8845
    sort_std: 0.0076
    global_rank: 465
    paper_rank: 465
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M3S
    model_key: m3s
    model_plain: M3S
    value: 0.8709
    std: 0.0052
    paper_value: 0.8709
    paper_std: 0.0052
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
    source_ref: sun2020multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8709
    true_std: 0.0052
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8709
    sort_std: 0.0052
    global_rank: 476
    paper_rank: 476
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Meta-PN
    model_key: meta-pn
    model_plain: Meta-PN
    value: 0.7932
    std: 0.1271
    paper_value: 0.7932
    paper_std: 0.1271
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
    source_ref: ding2022meta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7932
    true_std: 0.1271
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7932
    sort_std: 0.1271
    global_rank: 505
    paper_rank: 505
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
  dataset: Coauthor-Physics
  rows:
  - model: SelfGNN LDP
    model_key: geomancer
    model_plain: SelfGNN LDP
    value: 0.9878
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9878
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: lgd
    model_plain: SelfGNN LDP
    value: 0.9855
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9855
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: msh-gnn
    model_plain: SelfGNN LDP
    value: 0.9837
    std: 0.0008
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
    global_rank: 3
    sort_value: 0.9837
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN*
    model_key: gcn
    model_plain: GCN*
    value: 0.9283
    std: 0.002
    paper_value: 0.9283
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9774
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.04910000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9744
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04610000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0014
    global_rank: 9
    paper_rank: 210
    rank_delta: 201
    rank_delta_abs: 201
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9216
    std: 0.006
    paper_value: 0.9216
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9782
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.056599999999999984
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9732
    true_std: 0.0006
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.05159999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9732
    sort_std: 0.0006
    global_rank: 19
    paper_rank: 226
    rank_delta: 207
    rank_delta_abs: 207
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.9353
    std: 0.0013
    paper_value: 0.9353
    paper_std: 0.0013
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
    source_ref: gasteiger2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9654
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2305.12677'
    at_pub_source_title: Tokenized Graph Transformer with Neighborhood Augmentation
      for Node Classification in Large Graphs
    at_pub_source_date_iso: '2023-05-22'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.030100000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9654
    true_std: 0.0007
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.030100000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.9654
    sort_std: 0.0007
    global_rank: 56
    paper_rank: 185
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tokenized Graph Transformer with Neighborhood Augmentation
      for Node Classification in Large Graphs
    comparison_source_arxiv: '2305.12677'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE*
    model_key: graphsage
    model_plain: GraphSAGE*
    value: 0.927
    std: 0.0046
    paper_value: 0.927
    paper_std: 0.0046
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9649
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.037899999999999934
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9649
    true_std: 0.0006
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.037899999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.9649
    sort_std: 0.0006
    global_rank: 57
    paper_rank: 211
    rank_delta: 154
    rank_delta_abs: 154
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.9264
    std: 0.0012
    paper_value: 0.9264
    paper_std: 0.0012
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
    source_ref: feng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9647
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2305.12677'
    at_pub_source_title: Tokenized Graph Transformer with Neighborhood Augmentation
      for Node Classification in Large Graphs
    at_pub_source_date_iso: '2023-05-22'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0383
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9647
    true_std: 0.0004
    value_gap_source_arxiv: '2505.17660'
    value_gap_source_title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking
      Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0383
    has_value_note: false
    value_note: ''
    sort_value: 0.9647
    sort_std: 0.0004
    global_rank: 59
    paper_rank: 213
    rank_delta: 154
    rank_delta_abs: 154
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tokenized Graph Transformer with Neighborhood Augmentation
      for Node Classification in Large Graphs
    comparison_source_arxiv: '2305.12677'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.9275
    std: 0.0009
    paper_value: 0.9275
    paper_std: 0.0009
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
    source_ref: chen2020simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9597
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.032200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9597
    true_std: 0.0011
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.032200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9597
    sort_std: 0.0011
    global_rank: 81
    paper_rank: 211
    rank_delta: 130
    rank_delta_abs: 130
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.9132
    std: 0.0062
    paper_value: 0.9132
    paper_std: 0.0062
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.958
    at_pub_std: 0.001
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-11-20'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.04479999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.958
    true_std: 0.001
    value_gap_source_arxiv: '2111.10698'
    value_gap_source_title: Towards Graph Self-Supervised Learning with Contrastive
      Adjusted Zooming
    value_gap_source_is_current_paper: false
    value_gap: 0.04479999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.001
    global_rank: 87
    paper_rank: 231
    rank_delta: 144
    rank_delta_abs: 144
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Graph Self-Supervised Learning with Contrastive
      Adjusted Zooming
    comparison_source_arxiv: '2111.10698'
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.9245
    std: 0.0084
    paper_value: 0.9245
    paper_std: 0.0084
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
    source_ref: verma2021graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9449
    at_pub_std: 0.0084
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.020399999999999974
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9449
    true_std: 0.0084
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.020399999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.9449
    sort_std: 0.0084
    global_rank: 159
    paper_rank: 221
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    comparison_source_arxiv: '1909.11715'
    is_best: false
    is_std_outlier: false
  - model: NCGC (GCN)
    model_key: ncgc (gcn)
    model_plain: NCGC (GCN)
    value: 0.9441
    std: 0.0029
    paper_value: 0.9441
    paper_std: 0.0029
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9441
    true_std: 0.0029
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9441
    sort_std: 0.0029
    global_rank: 160
    paper_rank: 160
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.9428
    std: 0.0
    paper_value: 0.9428
    paper_std: 0.0
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
    source_ref: zhang2025normalize
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9428
    true_std: 0.0
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9428
    sort_std: 0.0
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
  - model: PTA
    model_key: pta
    model_plain: PTA
    value: 0.9424
    std: 0.0031
    paper_value: 0.9424
    paper_std: 0.0031
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
    source_ref: dong2021equivalence
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9424
    true_std: 0.0031
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9424
    sort_std: 0.0031
    global_rank: 165
    paper_rank: 165
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.9339
    std: 0.0001
    paper_value: 0.9339
    paper_std: 0.0001
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
    source_ref: liu2020towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9401
    at_pub_std: 0.006
    at_pub_source_arxiv: '2302.08727'
    at_pub_source_title: Building Shortcuts between Distant Nodes with Biaffine Mapping
      for Graph Convolutional Networks
    at_pub_source_date_iso: '2023-02-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006200000000000094
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9401
    true_std: 0.006
    value_gap_source_arxiv: '2302.08727'
    value_gap_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.006200000000000094
    has_value_note: false
    value_note: ''
    sort_value: 0.9401
    sort_std: 0.006
    global_rank: 173
    paper_rank: 190
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Building Shortcuts between Distant Nodes with Biaffine
      Mapping for Graph Convolutional Networks
    comparison_source_arxiv: '2302.08727'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.9357
    std: 0.0011
    paper_value: 0.9357
    paper_std: 0.0011
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
    source_ref: Chien21adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9357
    true_std: 0.0011
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9357
    sort_std: 0.0011
    global_rank: 185
    paper_rank: 185
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.9331
    std: 0.0151
    paper_value: 0.9331
    paper_std: 0.0151
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
    source_ref: stretcu2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9331
    true_std: 0.0151
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: 0.0151
    global_rank: 192
    paper_rank: 192
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.928
    std: 0.0025
    paper_value: 0.928
    paper_std: 0.0025
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9325
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2206.04471'
    at_pub_source_title: 'Towards Understanding Graph Neural Networks: An Algorithm
      Unrolling Perspective'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0044999999999999485
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9325
    true_std: 0.0082
    value_gap_source_arxiv: '2206.04471'
    value_gap_source_title: 'Towards Understanding Graph Neural Networks: An Algorithm
      Unrolling Perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.0044999999999999485
    has_value_note: false
    value_note: ''
    sort_value: 0.9325
    sort_std: 0.0082
    global_rank: 198
    paper_rank: 210
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Meta-PN
    model_key: meta-pn
    model_plain: Meta-PN
    value: 0.9206
    std: 0.0123
    paper_value: 0.9206
    paper_std: 0.0123
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
    source_ref: ding2022meta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9206
    true_std: 0.0123
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9206
    sort_std: 0.0123
    global_rank: 228
    paper_rank: 228
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: M3S
    model_key: m3s
    model_plain: M3S
    value: 0.8945
    std: 0.0095
    paper_value: 0.8945
    paper_std: 0.0095
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
    source_ref: sun2020multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test accuracy reported in Table 2
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8945
    true_std: 0.0095
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8945
    sort_std: 0.0095
    global_rank: 236
    paper_rank: 236
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
  - model: GCN*
    model_key: gcn
    model_plain: GCN*
    value: 0.846
    std: 0.0066
    paper_value: 0.846
    paper_std: 0.0066
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.054400000000000004
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
    value_gap: 0.054400000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 347
    rank_delta: 314
    rank_delta_abs: 314
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8036
    std: 0.0301
    paper_value: 0.8036
    paper_std: 0.0301
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
    source_ref: gasteiger2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8904
    at_pub_std: 0.015
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08679999999999999
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
    value_gap: 0.08679999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 765
    rank_delta: 696
    rank_delta_abs: 696
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: GAT*
    model_key: gat
    model_plain: GAT*
    value: 0.8382
    std: 0.0085
    paper_value: 0.8382
    paper_std: 0.0085
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8897
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.0515000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0515000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 420
    rank_delta: 348
    rank_delta_abs: 348
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7779
    std: 0.0197
    paper_value: 0.7779
    paper_std: 0.0197
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
    source_ref: chen2020simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8893
    at_pub_std: 0.0137
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.11139999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8893
    true_std: 0.0137
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.11139999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8893
    sort_std: 0.0137
    global_rank: 74
    paper_rank: 836
    rank_delta: 762
    rank_delta_abs: 762
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Language is All a Graph Needs
    comparison_source_arxiv: '2308.07134'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE*
    model_key: graphsage
    model_plain: GraphSAGE*
    value: 0.8346
    std: 0.0072
    paper_value: 0.8346
    paper_std: 0.0072
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8777
    at_pub_std: 0.0183
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.04310000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8889
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.054300000000000015
    has_value_note: false
    value_note: ''
    sort_value: 0.8889
    sort_std: null
    global_rank: 79
    paper_rank: 488
    rank_delta: 409
    rank_delta_abs: 409
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    comparison_source_arxiv: '2110.15777'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.8063
    std: 0.0017
    paper_value: 0.8063
    paper_std: 0.0017
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.887
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0807
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
    value_gap: 0.0807
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.0
    global_rank: 88
    paper_rank: 752
    rank_delta: 664
    rank_delta_abs: 664
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8151
    std: 0.0127
    paper_value: 0.8151
    paper_std: 0.0127
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
    source_ref: Chien21adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8854
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-03-12'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.07029999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8854
    true_std: 0.0067
    value_gap_source_arxiv: '2403.07954'
    value_gap_source_title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive
      Krylov Subspace Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.07029999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8854
    sort_std: 0.0067
    global_rank: 100
    paper_rank: 694
    rank_delta: 594
    rank_delta_abs: 594
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.8038
    std: 0.0173
    paper_value: 0.8038
    paper_std: 0.0173
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
    source_ref: liu2020towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.884
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.08020000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.884
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08020000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: null
    global_rank: 108
    paper_rank: 765
    rank_delta: 657
    rank_delta_abs: 657
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.8155
    std: 0.0027
    paper_value: 0.8155
    paper_std: 0.0027
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
    source_ref: feng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8815
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.06599999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8815
    true_std: null
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06599999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8815
    sort_std: null
    global_rank: 127
    paper_rank: 694
    rank_delta: 567
    rank_delta_abs: 567
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Transportation Improves Graph Neural Networks
    comparison_source_arxiv: '2307.16092'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8
    std: 0.0107
    paper_value: 0.8
    paper_std: 0.0107
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.06829999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8797
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0797
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: null
    global_rank: 138
    paper_rank: 775
    rank_delta: 637
    rank_delta_abs: 637
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: NCGC (GCNII)
    model_key: ncgc (gcnii)
    model_plain: NCGC (GCNII)
    value: 0.864
    std: 0.002
    paper_value: 0.864
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.864
    true_std: 0.002
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: 0.002
    global_rank: 241
    paper_rank: 241
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.8607
    std: 0.0
    paper_value: 0.8607
    paper_std: 0.0
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
    source_ref: zhang2025normalize
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8607
    true_std: 0.0
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8607
    sort_std: 0.0
    global_rank: 259
    paper_rank: 259
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DND-Net
    model_key: dnd-net
    model_plain: DND-Net
    value: 0.8498
    std: 0.0056
    paper_value: 0.8498
    paper_std: 0.0056
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
    source_ref: ding2024divide
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8498
    true_std: 0.0056
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8498
    sort_std: 0.0056
    global_rank: 326
    paper_rank: 326
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Violin
    model_key: violin
    model_plain: Violin
    value: 0.8449
    std: 0.0066
    paper_value: 0.8449
    paper_std: 0.0066
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
    source_ref: xie2023violin
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8449
    true_std: 0.0066
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8449
    sort_std: 0.0066
    global_rank: 356
    paper_rank: 356
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.7956
    std: 0.0086
    paper_value: 0.7956
    paper_std: 0.0086
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
    source_ref: verma2021graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8394
    at_pub_std: 0.0057
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.04380000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8394
    true_std: 0.0057
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04380000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8394
    sort_std: 0.0057
    global_rank: 410
    paper_rank: 789
    rank_delta: 379
    rank_delta_abs: 379
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    comparison_source_arxiv: '1909.11715'
    is_best: false
    is_std_outlier: false
  - model: Meta-PN
    model_key: meta-pn
    model_plain: Meta-PN
    value: 0.8233
    std: 0.0079
    paper_value: 0.8233
    paper_std: 0.0079
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
    source_ref: ding2022meta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8233
    true_std: 0.0079
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8233
    sort_std: 0.0079
    global_rank: 601
    paper_rank: 601
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.7566
    std: 0.0015
    paper_value: 0.7566
    paper_std: 0.0015
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
    source_ref: stretcu2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8228
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2009.02027'
    at_pub_source_title: Rethinking Graph Regularization for Graph Neural Networks
    at_pub_source_date_iso: '2020-09-04'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.06619999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8228
    true_std: 0.0048
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06619999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8228
    sort_std: 0.0048
    global_rank: 620
    paper_rank: 874
    rank_delta: 254
    rank_delta_abs: 254
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking Graph Regularization for Graph Neural Networks
    comparison_source_arxiv: '2009.02027'
    is_best: false
    is_std_outlier: false
  - model: PTA
    model_key: pta
    model_plain: PTA
    value: 0.8203
    std: 0.0105
    paper_value: 0.8203
    paper_std: 0.0105
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
    source_ref: dong2021equivalence
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8205
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2507.14484'
    at_pub_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable
      Node Classification with Structured Predictions'
    at_pub_source_date_iso: '2025-07-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8205
    true_std: 0.0028
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.8205
    sort_std: 0.0028
    global_rank: 642
    paper_rank: 643
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.8123
    std: 0.0043
    paper_value: 0.8123
    paper_std: 0.0043
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
    source_ref: yang2024mixed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8089
    at_pub_std: 0.0095
    at_pub_source_arxiv: '2206.02796'
    at_pub_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0034000000000000696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8123
    true_std: 0.0043
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8123
    sort_std: 0.0043
    global_rank: 711
    paper_rank: 711
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M3S
    model_key: m3s
    model_plain: M3S
    value: 0.773
    std: 0.0046
    paper_value: 0.773
    paper_std: 0.0046
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
    source_ref: sun2020multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.773
    true_std: 0.0046
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.773
    sort_std: 0.0046
    global_rank: 850
    paper_rank: 850
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
- &id002
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
    value: 0.7947
    std: 0.0031
    paper_value: 0.7947
    paper_std: 0.0031
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8864
    at_pub_std: 0.003
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.0917
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.15400000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9487
    sort_std: null
    global_rank: 9
    paper_rank: 542
    rank_delta: 533
    rank_delta_abs: 533
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-backtracking Graph Neural Networks
    comparison_source_arxiv: '2310.07430'
    is_best: true
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.7729
    std: 0.0082
    paper_value: 0.7729
    paper_std: 0.0082
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
    source_ref: gasteiger2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9355
    at_pub_std: 0.006
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.16259999999999997
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
    value_gap: 0.16259999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9355
    sort_std: 0.006
    global_rank: 20
    paper_rank: 755
    rank_delta: 735
    rank_delta_abs: 735
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: GCN*
    model_key: gcn
    model_plain: GCN*
    value: 0.8052
    std: 0.0116
    paper_value: 0.8052
    paper_std: 0.0116
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9296
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.12439999999999996
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
    value_gap: 0.12439999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 422
    rank_delta: 401
    rank_delta_abs: 401
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: GAT*
    model_key: gat
    model_plain: GAT*
    value: 0.7906
    std: 0.0208
    paper_value: 0.7906
    paper_std: 0.0208
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
    source_ref: luoclassic
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9233
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.13270000000000004
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
    value_gap: 0.13270000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 608
    rank_delta: 585
    rank_delta_abs: 585
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.7522
    std: 0.0084
    paper_value: 0.7522
    paper_std: 0.0084
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
    source_ref: xu2018representation
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.916
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.16380000000000006
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
    value_gap: 0.16380000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: null
    global_rank: 27
    paper_rank: 822
    rank_delta: 795
    rank_delta_abs: 795
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7618
    std: 0.0178
    paper_value: 0.7618
    paper_std: 0.0178
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
    source_ref: chen2020simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.903
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.1412
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.903
    true_std: null
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1412
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: null
    global_rank: 70
    paper_rank: 795
    rank_delta: 725
    rank_delta_abs: 725
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.7541
    std: 0.0051
    paper_value: 0.7541
    paper_std: 0.0051
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
    source_ref: feng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8902
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.1361
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8902
    true_std: null
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1361
    has_value_note: false
    value_note: ''
    sort_value: 0.8902
    sort_std: null
    global_rank: 130
    paper_rank: 818
    rank_delta: 688
    rank_delta_abs: 688
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Transportation Improves Graph Neural Networks
    comparison_source_arxiv: '2307.16092'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.783
    std: 0.0161
    paper_value: 0.783
    paper_std: 0.0161
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
    source_ref: Chien21adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8846
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-11-30'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10160000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8846
    true_std: 0.0031
    value_gap_source_arxiv: '2311.18177'
    value_gap_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10160000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8846
    sort_std: 0.0031
    global_rank: 152
    paper_rank: 687
    rank_delta: 535
    rank_delta_abs: 535
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7623
    std: 0.0005
    paper_value: 0.7623
    paper_std: 0.0005
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
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8832
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12090000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.0055
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.12090000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.0055
    global_rank: 159
    paper_rank: 794
    rank_delta: 635
    rank_delta_abs: 635
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.775
    std: 0.0131
    paper_value: 0.775
    paper_std: 0.0131
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
    source_ref: liu2020towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.864
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.08899999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.864
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08899999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: null
    global_rank: 247
    paper_rank: 748
    rank_delta: 501
    rank_delta_abs: 501
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: NCGC (GCNII)
    model_key: ncgc (gcnii)
    model_plain: NCGC (GCNII)
    value: 0.8203
    std: 0.0032
    paper_value: 0.8203
    paper_std: 0.0032
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8203
    true_std: 0.0032
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8203
    sort_std: 0.0032
    global_rank: 343
    paper_rank: 343
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Meta-PN
    model_key: meta-pn
    model_plain: Meta-PN
    value: 0.819
    std: 0.0045
    paper_value: 0.819
    paper_std: 0.0045
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
    source_ref: ding2022meta
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.819
    true_std: 0.0045
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.0045
    global_rank: 347
    paper_rank: 347
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NormProp
    model_key: normprop
    model_plain: NormProp
    value: 0.8153
    std: 0.0001
    paper_value: 0.8153
    paper_std: 0.0001
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
    source_ref: zhang2025normalize
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8153
    true_std: 0.0001
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8153
    sort_std: 0.0001
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
  - model: Violin
    model_key: violin
    model_plain: Violin
    value: 0.8123
    std: 0.0042
    paper_value: 0.8123
    paper_std: 0.0042
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
    source_ref: xie2023violin
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8123
    true_std: 0.0042
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8123
    sort_std: 0.0042
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
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.7847
    std: 0.0134
    paper_value: 0.7847
    paper_std: 0.0134
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
    source_ref: verma2021graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.811
    at_pub_std: 0.0078
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.0263000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.811
    true_std: 0.0078
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0263000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.0078
    global_rank: 387
    paper_rank: 680
    rank_delta: 293
    rank_delta_abs: 293
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    comparison_source_arxiv: '1909.11715'
    is_best: false
    is_std_outlier: false
  - model: PTA
    model_key: pta
    model_plain: PTA
    value: 0.8087
    std: 0.0062
    paper_value: 0.8087
    paper_std: 0.0062
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
    source_ref: dong2021equivalence
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7989
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2010.12408'
    at_pub_source_title: On the Equivalence of Decoupled Graph Convolution Network
      and Label Propagation
    at_pub_source_date_iso: '2020-10-23'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00979999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8087
    true_std: 0.0062
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8087
    sort_std: 0.0062
    global_rank: 402
    paper_rank: 402
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: On the Equivalence of Decoupled Graph Convolution Network
      and Label Propagation
    comparison_source_arxiv: '2010.12408'
    is_best: false
    is_std_outlier: false
  - model: GAM
    model_key: gam
    model_plain: GAM
    value: 0.7825
    std: 0.0025
    paper_value: 0.7825
    paper_std: 0.0025
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
    source_ref: stretcu2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.796
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2009.02027'
    at_pub_source_title: Rethinking Graph Regularization for Graph Neural Networks
    at_pub_source_date_iso: '2020-09-04'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-04'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.013500000000000068
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.796
    true_std: 0.0063
    value_gap_source_arxiv: '2009.02027'
    value_gap_source_title: Rethinking Graph Regularization for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.013500000000000068
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.0063
    global_rank: 519
    paper_rank: 694
    rank_delta: 175
    rank_delta_abs: 175
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking Graph Regularization for Graph Neural Networks
    comparison_source_arxiv: '2009.02027'
    is_best: false
    is_std_outlier: false
  - model: M3S
    model_key: m3s
    model_plain: M3S
    value: 0.7558
    std: 0.0115
    paper_value: 0.7558
    paper_std: 0.0115
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
    source_ref: sun2020multi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.795
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2006.10141'
    at_pub_source_title: 'Self-supervised Learning on Graphs: Deep Insights and New
      Directions'
    at_pub_source_date_iso: '2020-06-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-17'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.03920000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.795
    true_std: 0.0076
    value_gap_source_arxiv: '2006.10141'
    value_gap_source_title: 'Self-supervised Learning on Graphs: Deep Insights and
      New Directions'
    value_gap_source_is_current_paper: false
    value_gap: 0.03920000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.795
    sort_std: 0.0076
    global_rank: 534
    paper_rank: 814
    rank_delta: 280
    rank_delta_abs: 280
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Self-supervised Learning on Graphs: Deep Insights and
      New Directions'
    comparison_source_arxiv: '2006.10141'
    is_best: false
    is_std_outlier: false
  - model: DND-Net
    model_key: dnd-net
    model_plain: DND-Net
    value: 0.7824
    std: 0.0098
    paper_value: 0.7824
    paper_std: 0.0098
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
    source_ref: ding2024divide
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7824
    true_std: 0.0098
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7824
    sort_std: 0.0098
    global_rank: 695
    paper_rank: 695
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.7634
    std: 0.0073
    paper_value: 0.7634
    paper_std: 0.0073
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
    source_ref: yang2024mixed
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Planetoid split
    date: Nov 25, 2025
    date_display: Nov 2025
    date_iso: '2025-11-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7634
    true_std: 0.0073
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7634
    sort_std: 0.0073
    global_rank: 792
    paper_rank: 792
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
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
main_figure: /figures/2511.19976/main_figure.jpegoptim.jpg
---

