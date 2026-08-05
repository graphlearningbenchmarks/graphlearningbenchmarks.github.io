---
title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based Graph Representation
  Learning'
arxiv_id: '2303.03379'
source_url: ''
authors:
- name: Haoteng Yin
  orcid: null
  s2_author_id: '26379330'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '1390814008'
  s2_url: null
- name: Jianguo Wang
  orcid: null
  s2_author_id: '2118443226'
  s2_url: null
- name: Pan Li
  orcid: null
  s2_author_id: '1561672016'
  s2_url: null
published_date: Mar 6, 2023
published_date_iso: '2023-03-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Subgraph-based graph representation learning (SGRL) has recently emerged
  as a powerful tool in many prediction tasks on graphs due to its advantages in model
  expressiveness and generalization ability. Most previous SGRL models face computational
  challenges associated with the high cost of subgraph extraction for each training
  or test query. Recently, SUREL was proposed to accelerate SGRL, which samples random
  walks offline and joins these walks online as a proxy of subgraph for representation
  learning. Thanks to the reusability of sampled walks across different queries, SUREL
  achieves state-of-the-art performance in terms of scalability and prediction accuracy.
  However, SUREL still suffers from high computational overhead caused by node duplication
  in sampled walks. In this work, we propose a novel framework SUREL+ that upgrades
  SUREL by using node sets instead of walks to represent subgraphs. This set-based
  representation eliminates repeated nodes by definition but can also be irregular
  in size. To address this issue, we design a customized sparse data structure to
  efficiently store and access node sets and provide a specialized operator to join
  them in parallel batches. SUREL+ is modularized to support multiple types of set
  samplers, structural features, and neural encoders to complement the structural
  information loss after the reduction from walks to sets. Extensive experiments have
  been performed to validate SUREL+ in the prediction tasks of links, relation types,
  and higher-order patterns. SUREL+ achieves 3-11$ $ speedups of SUREL while maintaining
  comparable or even better prediction performance; compared to other SGRL baselines,
  SUREL+ achieves $ $20$ $ speedups and significantly improves the prediction accuracy.
codebase_url: 'https://github.com/Graph-COM/SUREL_Plus{https:'
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SUREL
mrr: 0.1964
adjusted_mrr: 0.131
mrr_dataset_count: 2
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: ogbl-citation2
  rows:
  - model: Classification
    model_key: mplp
    model_plain: Classification
    value: 0.9072
    std: 0.0012
    metric: MRR
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_display: Sep 2023
    date_iso: '2023-09-02'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
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
  - model: Classification
    model_key: cfg
    model_plain: Classification
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
  - model: Classification
    model_key: sieg
    model_plain: Classification
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
  - model: SUREL
    model_key: surel
    model_plain: SUREL
    value: 0.8974
    std: 0.0018
    paper_value: 0.8974
    paper_std: 0.0018
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-citation2
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8974
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2202.13538'
    at_pub_source_title: Algorithm and System Co-design for Efficient Subgraph-based
      Graph Representation Learning
    at_pub_source_date_iso: '2022-02-28'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8974
    true_std: 0.0018
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8974
    sort_std: 0.0018
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
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.8767
    std: 0.0032
    paper_value: 0.8767
    paper_std: 0.0032
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-citation2
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8767
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8767
    true_std: 0.0032
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0032
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8474
    std: 0.0021
    paper_value: 0.8474
    paper_std: 0.0021
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-citation2
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8479
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8705
    true_std: 0.0004
    value_gap_source_arxiv: '2409.17475'
    value_gap_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.02310000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8705
    sort_std: 0.0004
    global_rank: 14
    paper_rank: 23
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGNN
    model_key: gdgnn
    model_plain: GDGNN
    value: 0.8696
    std: 0.0028
    paper_value: 0.8696
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-citation2
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8696
    true_std: 0.0028
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8696
    sort_std: 0.0028
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
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.7985
    std: 0.004
    paper_value: 0.7985
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-citation2
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7985
    at_pub_std: 0.004
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7985
    true_std: 0.004
    value_gap_source_arxiv: '2303.03379'
    value_gap_source_title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based
      Graph Representation Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7985
    sort_std: 0.004
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
  rank_metric: MRR
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - MRR
  metric: MRR
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ogbl-ppa
  rows:
  - model: Classification
    model_key: mplp
    model_plain: Classification
    value: 0.6524
    std: 0.015
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_display: Sep 2023
    date_iso: '2023-09-02'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6524
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Classification
    model_key: ogb leader
    model_plain: Classification
    value: 0.6524
    std: 0.015
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/workrep20232/PROXI
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6524
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Classification
    model_key: prb
    model_plain: Classification
    value: 0.6347
    std: 0.0175
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.01410'
    title: PageRank Bandits for Link Prediction
    date: Nov 3, 2024
    date_display: Nov 2024
    date_iso: '2024-11-03'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/jiaruzouu/PRB
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6347
    sort_std: 0.0175
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SUREL
    model_key: surel
    model_plain: SUREL
    value: 0.5432
    std: 0.0044
    paper_value: 0.5432
    paper_std: 0.0044
    metric: Hits@100
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-ppa
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5323
    at_pub_std: 0.0103
    at_pub_source_arxiv: '2202.13538'
    at_pub_source_title: Algorithm and System Co-design for Efficient Subgraph-based
      Graph Representation Learning
    at_pub_source_date_iso: '2022-02-28'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-03-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.01090000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5432
    true_std: 0.0044
    value_gap_source_arxiv: '2303.03379'
    value_gap_source_title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based
      Graph Representation Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5432
    sort_std: 0.0044
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.488
    std: 0.0316
    paper_value: 0.488
    paper_std: 0.0316
    metric: Hits@100
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-ppa
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.488
    at_pub_std: 0.0316
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.488
    true_std: 0.0316
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: 0.0316
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDGNN
    model_key: gdgnn
    model_plain: GDGNN
    value: 0.4592
    std: 0.0214
    paper_value: 0.4592
    paper_std: 0.0214
    metric: Hits@100
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-ppa
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4592
    true_std: 0.0214
    value_gap_source_arxiv: '2303.03379'
    value_gap_source_title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based
      Graph Representation Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4592
    sort_std: 0.0214
    global_rank: 24
    paper_rank: 24
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
    value: 0.1867
    std: 0.0132
    paper_value: 0.1867
    paper_std: 0.0132
    metric: Hits@100
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-ppa
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.187
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.0002999999999999947
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2957
    true_std: 0.029
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.10900000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2957
    sort_std: 0.029
    global_rank: 41
    paper_rank: 55
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.0383
    std: 0.0133
    paper_value: 0.0383
    paper_std: 0.0133
    metric: Hits@100
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Standard link prediction task on ogbl-ppa
    date: Mar 6, 2023
    date_display: Mar 2023
    date_iso: '2023-03-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0383
    at_pub_std: 0.0133
    at_pub_source_arxiv: '2202.13538'
    at_pub_source_title: Algorithm and System Co-design for Efficient Subgraph-based
      Graph Representation Learning
    at_pub_source_date_iso: '2022-02-28'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-03-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0383
    true_std: 0.0133
    value_gap_source_arxiv: '2303.03379'
    value_gap_source_title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based
      Graph Representation Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0383
    sort_std: 0.0133
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Hits@100
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@100
  paper_metrics:
  - Hits@100
  metric: Hits@100
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-ppa
      dataset_slug: ogbl-ppa
    - dataset: ogbl-citation2
      dataset_slug: ogbl-citation2
single_proposed_model: SUREL
main_figure: /figures/2303.03379/main_figure.jpegoptim.jpg
---

