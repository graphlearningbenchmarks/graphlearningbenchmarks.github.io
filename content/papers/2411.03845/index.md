---
title: Reconsidering the Performance of GAE in Link Prediction
arxiv_id: '2411.03845'
source_url: ''
authors:
- name: Weishuo Ma
  orcid: null
  s2_author_id: '2329881981'
  s2_url: null
- name: Yanbo Wang
  orcid: null
  s2_author_id: '2298929357'
  s2_url: null
- name: Xiyuan Wang
  orcid: null
  s2_author_id: '2167480960'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '2264103931'
  s2_url: null
published_date: Nov 6, 2024
published_date_iso: '2024-11-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Recent advancements in graph neural networks (GNNs) for link prediction
  have introduced sophisticated training techniques and model architectures. However,
  reliance on outdated baselines may exaggerate the benefits of these new approaches.
  To tackle this issue, we systematically explore Graph Autoencoders (GAEs) by applying
  model-agnostic tricks in recent methods and tuning hyperparameters. We find that
  a well-tuned GAE can match the performance of recent sophisticated models while
  offering superior computational efficiency on widely used link prediction benchmarks.
  Our approach delivers substantial performance gains on datasets where structural
  information dominates and feature data is limited. Specifically, our GAE achieves
  a state-of-the-art (SOTA) Hits@100 score of 78.41\
codebase_url: https://github.com/GraphPKU/Refined-GAE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MPNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 4
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id003
  dataset: ogbl-citation2
  rows:
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.9072
    std: 0.0012
    paper_value: 0.9072
    paper_std: 0.0012
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
    source_ref: mplp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9072
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2309.00976'
    at_pub_source_title: Pure Message Passing Can Estimate Common Neighbor for Link
      Prediction
    at_pub_source_date_iso: '2023-09-02'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-09-02'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9072
    true_std: 0.0012
    value_gap_source_arxiv: '2309.00976'
    value_gap_source_title: Pure Message Passing Can Estimate Common Neighbor for
      Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9072
    sort_std: 0.0012
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
  - model: Optimized GAE
    model_key: optimized gae
    model_plain: Optimized GAE
    value: 0.8874
    std: 0.0006
    paper_value: 0.8874
    paper_std: 0.0006
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8874
    sort_std: 0.0006
    global_rank: 7
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
    source_ref: seal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
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
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.8756
    std: 0.0011
    paper_value: 0.8756
    paper_std: 0.0011
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
    source_ref: buddy
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8756
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
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
    true_value: 0.8756
    true_std: 0.0011
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8756
    sort_std: 0.0011
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
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.8726
    std: 0.0084
    paper_value: 0.8726
    paper_std: 0.0084
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
    source_ref: neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8726
    at_pub_std: 0.0084
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8726
    true_std: 0.0084
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8726
    sort_std: 0.0084
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
    is_std_outlier: false
  - model: GAE(GCN)
    model_key: gae(gcn)
    model_plain: GAE(GCN)
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
    source_ref: ogb
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8474
    sort_std: 0.0021
    global_rank: 25
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.5198
    std: 0.0
    paper_value: 0.5198
    paper_std: 0.0
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
    source_ref: ra
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5198
    at_pub_std: 0.0
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7604
    true_std: 0.0
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.24059999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7604
    sort_std: 0.0
    global_rank: 52
    paper_rank: 62
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.5189
    std: 0.0
    paper_value: 0.5189
    paper_std: 0.0
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
    source_ref: aa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5189
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7596
    true_std: 0.0
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.24070000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.0
    global_rank: 53
    paper_rank: 62
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.5147
    std: 0.0
    paper_value: 0.5147
    paper_std: 0.0
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
    source_ref: cn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5147
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.743
    true_std: 0.0
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.22829999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.0
    global_rank: 55
    paper_rank: 63
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
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
- &id001
  dataset: ogbl-collab
  rows:
  - model: SIGN
    model_key: proxi
    model_plain: SIGN
    value: 0.765
    std: 0.0027
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 1
    sort_value: 0.765
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SIGN
    model_key: ogb leader
    model_plain: SIGN
    value: 0.7129
    std: 0.0018
    metric: Hits@50
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
    sort_value: 0.7129
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: gidn
    model_plain: SIGN
    value: 0.7096
    std: 0.0055
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.01301'
    title: 'GIDN: A Lightweight Graph Inception Diffusion Network for High-efficient
      Link Prediction'
    date: Oct 4, 2022
    date_display: Oct 2022
    date_iso: '2022-10-04'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7096
    sort_std: 0.0055
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.6699
    std: 0.004
    paper_value: 0.6699
    paper_std: 0.004
    metric: Hits@50
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
    source_ref: mplp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6699
    sort_std: 0.004
    global_rank: 6
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.5752
    std: 0.0037
    paper_value: 0.5752
    paper_std: 0.0037
    metric: Hits@50
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
    source_ref: neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6613
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2410.01802'
    at_pub_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    at_pub_source_date_iso: '2024-10-02'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.08609999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6613
    true_std: 0.0061
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.08609999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.6613
    sort_std: 0.0061
    global_rank: 8
    paper_rank: 26
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    comparison_source_arxiv: '2410.01802'
    is_best: false
    is_std_outlier: false
  - model: Optimized GAE
    model_key: optimized gae
    model_plain: Optimized GAE
    value: 0.6611
    std: 0.0035
    paper_value: 0.6611
    paper_std: 0.0035
    metric: Hits@50
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6611
    sort_std: 0.0035
    global_rank: 9
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.6594
    std: 0.0058
    paper_value: 0.6594
    paper_std: 0.0058
    metric: Hits@50
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
    source_ref: buddy
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6594
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2310.09516'
    at_pub_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    at_pub_source_date_iso: '2023-10-14'
    at_pub_source_date_label: '2023'
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
    true_value: 0.6594
    true_std: 0.0058
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6594
    sort_std: 0.0058
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
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.6474
    std: 0.0043
    paper_value: 0.6474
    paper_std: 0.0043
    metric: Hits@50
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
    source_ref: seal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6474
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
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
    true_value: 0.6474
    true_std: 0.0043
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.0043
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
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.6435
    std: 0.0
    paper_value: 0.6435
    paper_std: 0.0
    metric: Hits@50
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
    source_ref: aa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6435
    at_pub_std: 0.0
    at_pub_source_arxiv: '2310.09516'
    at_pub_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    at_pub_source_date_iso: '2023-10-14'
    at_pub_source_date_label: '2023'
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
    true_value: 0.6435
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6435
    sort_std: 0.0
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
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.64
    std: 0.0
    paper_value: 0.64
    paper_std: 0.0
    metric: Hits@50
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
    source_ref: ra
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.64
    at_pub_std: 0.0
    at_pub_source_arxiv: '2310.09516'
    at_pub_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    at_pub_source_date_iso: '2023-10-14'
    at_pub_source_date_label: '2023'
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
    true_value: 0.64
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: 0.0
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
  - model: NCN
    model_key: ncn
    model_plain: NCN
    value: 0.6476
    std: 0.0087
    paper_value: 0.6476
    paper_std: 0.0087
    metric: Hits@50
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
    source_ref: ncn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6476
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2310.11009'
    at_pub_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6386
    true_std: 0.0051
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.6386
    sort_std: 0.0051
    global_rank: 21
    paper_rank: 15
    rank_delta: -6
    rank_delta_abs: 6
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.5644
    std: 0.0
    paper_value: 0.5644
    paper_std: 0.0
    metric: Hits@50
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
    source_ref: cn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6137
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.04930000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6137
    true_std: 0.0
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.04930000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.6137
    sort_std: 0.0
    global_rank: 22
    paper_rank: 26
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: GAE(SAGE)
    model_key: gae(sage)
    model_plain: GAE(SAGE)
    value: 0.5463
    std: 0.0112
    paper_value: 0.5463
    paper_std: 0.0112
    metric: Hits@50
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
    source_ref: ogb
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5463
    sort_std: 0.0112
    global_rank: 32
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Hits@50
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@50
  paper_metrics:
  - Hits@50
  metric: Hits@50
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: ogbl-ddi
  rows:
  - model: MPNNs
    model_key: elgnn
    model_plain: MPNNs
    value: 0.9777
    std: 0.0037
    metric: Hits@20
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_display: Oct 2023
    date_iso: '2023-10-22'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: construct an ensemble of graph neural networks by utilizing
      both input features and graph structures
    is_global_top: true
    global_rank: 1
    sort_value: 0.9777
    sort_std: 0.0037
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPNNs
    model_key: gidn
    model_plain: MPNNs
    value: 0.9542
    std: 0.0
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_display: Oct 2023
    date_iso: '2023-10-22'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9542
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNNs
    model_key: agdn
    model_plain: MPNNs
    value: 0.9538
    std: 0.0094
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_display: Oct 2023
    date_iso: '2023-10-22'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9538
    sort_std: 0.0094
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.9443
    std: 0.0057
    paper_value: 0.9443
    paper_std: 0.0057
    metric: Hits@20
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.9443
    sort_std: 0.0057
    global_rank: 5
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.7851
    std: 0.0136
    paper_value: 0.7851
    paper_std: 0.0136
    metric: Hits@20
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
    source_ref: buddy
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7851
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
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
    true_value: 0.7851
    true_std: 0.0136
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7851
    sort_std: 0.0136
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
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.6357
    std: 0.0352
    paper_value: 0.6357
    paper_std: 0.0352
    metric: Hits@20
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
    source_ref: neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6357
    at_pub_std: 0.0352
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6357
    true_std: 0.0352
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6357
    sort_std: 0.0352
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
  - model: GAE(SAGE)
    model_key: gae(sage)
    model_plain: GAE(SAGE)
    value: 0.539
    std: 0.0474
    paper_value: 0.539
    paper_std: 0.0474
    metric: Hits@20
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
    source_ref: ogb
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.539
    sort_std: 0.0474
    global_rank: 27
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.3056
    std: 0.0386
    paper_value: 0.3056
    paper_std: 0.0386
    metric: Hits@20
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
    source_ref: seal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4974
    at_pub_std: 0.0239
    at_pub_source_arxiv: '2406.16687'
    at_pub_source_title: Link Prediction with Untrained Message Passing Layers
    at_pub_source_date_iso: '2024-06-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.19180000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3056
    true_std: 0.0386
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3056
    sort_std: 0.0386
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Link Prediction with Untrained Message Passing Layers
    comparison_source_arxiv: '2406.16687'
    is_best: false
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.276
    std: 0.0
    paper_value: 0.276
    paper_std: 0.0
    metric: Hits@20
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
    source_ref: ra
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4401
    at_pub_std: null
    at_pub_source_arxiv: '2406.16687'
    at_pub_source_title: Link Prediction with Untrained Message Passing Layers
    at_pub_source_date_iso: '2024-06-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.16409999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.276
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.276
    sort_std: 0.0
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Link Prediction with Untrained Message Passing Layers
    comparison_source_arxiv: '2406.16687'
    is_best: false
    is_std_outlier: false
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.1861
    std: 0.0
    paper_value: 0.1861
    paper_std: 0.0
    metric: Hits@20
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
    source_ref: aa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3975
    at_pub_std: null
    at_pub_source_arxiv: '2406.16687'
    at_pub_source_title: Link Prediction with Untrained Message Passing Layers
    at_pub_source_date_iso: '2024-06-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.21140000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1861
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1861
    sort_std: 0.0
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Link Prediction with Untrained Message Passing Layers
    comparison_source_arxiv: '2406.16687'
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.1773
    std: 0.0
    paper_value: 0.1773
    paper_std: 0.0
    metric: Hits@20
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
    source_ref: cn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3869
    at_pub_std: null
    at_pub_source_arxiv: '2406.16687'
    at_pub_source_title: Link Prediction with Untrained Message Passing Layers
    at_pub_source_date_iso: '2024-06-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2096
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1773
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1773
    sort_std: 0.0
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Link Prediction with Untrained Message Passing Layers
    comparison_source_arxiv: '2406.16687'
    is_best: false
    is_std_outlier: false
  - model: NBFnet
    model_key: nbfnet
    model_plain: NBFnet
    value: 0.04
    std: 0.0058
    paper_value: 0.04
    paper_std: 0.0058
    metric: Hits@20
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
    source_ref: kg
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.04
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
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
    true_value: 0.04
    true_std: 0.0058
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.04
    sort_std: 0.0058
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
  rank_metric: Hits@20
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@20
  paper_metrics:
  - Hits@20
  metric: Hits@20
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: ogbl-ppa
  rows:
  - model: Optimized GAE
    model_key: optimized gae
    model_plain: Optimized GAE
    value: 0.7841
    std: 0.0083
    paper_value: 0.7841
    paper_std: 0.0083
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7841
    sort_std: 0.0083
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.6524
    std: 0.015
    paper_value: 0.6524
    paper_std: 0.015
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
    source_ref: mplp
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6524
    at_pub_std: 0.015
    at_pub_source_arxiv: '2309.00976'
    at_pub_source_title: Pure Message Passing Can Estimate Common Neighbor for Link
      Prediction
    at_pub_source_date_iso: '2023-09-02'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-09-02'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6524
    true_std: 0.015
    value_gap_source_arxiv: '2309.00976'
    value_gap_source_title: Pure Message Passing Can Estimate Common Neighbor for
      Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6524
    sort_std: 0.015
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
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
    is_best: false
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
    is_best: false
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.4933
    std: 0.0
    paper_value: 0.4933
    paper_std: 0.0
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
    source_ref: ra
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5324
    at_pub_std: 0.0
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.03909999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5324
    true_std: 0.0
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.03909999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5324
    sort_std: 0.0
    global_rank: 8
    paper_rank: 16
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pairwise Learning for Neural Link Prediction
    comparison_source_arxiv: '2112.02936'
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.4985
    std: 0.002
    paper_value: 0.4985
    paper_std: 0.002
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
    source_ref: buddy
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4985
    at_pub_std: 0.002
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4985
    true_std: 0.002
    value_gap_source_arxiv: '2209.15486'
    value_gap_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4985
    sort_std: 0.002
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
    is_std_outlier: false
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.4913
    std: 0.006
    paper_value: 0.4913
    paper_std: 0.006
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
    source_ref: neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4913
    at_pub_std: 0.006
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4913
    true_std: 0.006
    value_gap_source_arxiv: '2209.15486'
    value_gap_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4913
    sort_std: 0.006
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
    source_ref: seal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
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
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.3245
    std: 0.0
    paper_value: 0.3245
    paper_std: 0.0
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
    source_ref: aa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3245
    at_pub_std: 0.0
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
    true_value: 0.3245
    true_std: 0.0
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3245
    sort_std: 0.0
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
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.2765
    std: 0.0
    paper_value: 0.2765
    paper_std: 0.0
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
    source_ref: cn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2765
    at_pub_std: 0.0
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2765
    true_std: 0.0
    value_gap_source_arxiv: '2209.15486'
    value_gap_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2765
    sort_std: 0.0
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE(GCN)
    model_key: gae(gcn)
    model_plain: GAE(GCN)
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
    source_ref: ogb
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.1867
    sort_std: 0.0132
    global_rank: 58
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
  - *id003
  - *id004
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-collab
      dataset_slug: ogbl-collab
    - dataset: ogbl-ppa
      dataset_slug: ogbl-ppa
    - dataset: ogbl-citation2
      dataset_slug: ogbl-citation2
    - dataset: ogbl-ddi
      dataset_slug: ogbl-ddi
single_proposed_model: MPNN
main_figure: /figures/2411.03845/main_figure.jpegoptim.jpg
---

