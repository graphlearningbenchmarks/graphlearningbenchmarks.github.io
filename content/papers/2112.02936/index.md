---
title: Pairwise Learning for Neural Link Prediction
arxiv_id: '2112.02936'
source_url: ''
authors:
- name: Zhitao Wang
  orcid: null
  s2_author_id: '2278354826'
  s2_url: null
- name: Yong Zhou
  orcid: null
  s2_author_id: '2145494047'
  s2_url: null
- name: L. Hong
  orcid: null
  s2_author_id: '150187969'
  s2_url: null
- name: Yuanhang Zou
  orcid: null
  s2_author_id: '3103561'
  s2_url: null
- name: Hanjing Su
  orcid: null
  s2_author_id: '2658433'
  s2_url: null
- name: Shouzhi Chen
  orcid: null
  s2_author_id: '1940391397'
  s2_url: null
published_date: Dec 6, 2021
published_date_iso: '2021-12-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: In this paper, we aim at providing an effective Pairwise Learning for Neural
  Link Prediction (PLNLP) framework. The framework treats link prediction as a pairwise
  learning to rank problem and consists of four main components, i.e., neighborhood
  encoder, link predictor, negative sampler and objective function. The framework
  is flexible that any generic graph neural convolutions or link prediction specific
  neural architectures could be employed as neighborhood encoder. For link predictor,
  we design different scoring functions, which could be selected based on different
  types of graphs. In negative sampler, we provide several sampling strategies, which
  are problem specific. As for objective function, we propose to use an effective
  ranking loss, which approximately maximizes the standard ranking metric AUC. We
  evaluate the proposed PLNLP framework on 4 link property prediction datasets of
  Open Graph Benchmark (OGB), including ogbl-ddi, ogbl-collab, ogbl-ppa and ogbl-ciation2.
  PLNLP achieves top 1 performance on ogbl-ddi and ogbl-collab, and top 2 performance
  on ogbl-ciation2 only with basic neural architecture. The experimental results demonstrate
  the effectiveness of PLNLP.
codebase_url: https://github.com/zhitao-wang/PLNLP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PLNLP
mrr: 0.1221
adjusted_mrr: 0.1221
mrr_dataset_count: 4
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
    input_feature_source: raw_features
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    std: 0.0031
    paper_value: 0.8474
    paper_std: 0.0031
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
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8474
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
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
  - model: PLNLP
    model_key: plnlp
    model_plain: PLNLP
    value: 0.8492
    std: 0.0029
    paper_value: 0.8492
    paper_std: 0.0029
    metric: MRR
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
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8492
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2012.15024'
    at_pub_source_title: Adaptive Graph Diffusion Networks
    at_pub_source_date_iso: '2020-12-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8492
    true_std: 0.0029
    value_gap_source_arxiv: '2012.15024'
    value_gap_source_title: Adaptive Graph Diffusion Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8492
    sort_std: 0.0029
    global_rank: 22
    paper_rank: 22
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
    model_key: classification
    model_plain: Classification
    value: 0.8464
    std: null
    paper_value: 0.8464
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
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8464
    true_std: null
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8464
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.826
    std: 0.0036
    paper_value: 0.826
    paper_std: 0.0036
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
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8367
    true_std: 0.0007
    value_gap_source_arxiv: '2409.17475'
    value_gap_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.010700000000000043
    has_value_note: false
    value_note: ''
    sort_value: 0.8367
    sort_std: 0.0007
    global_rank: 29
    paper_rank: 34
    rank_delta: 5
    rank_delta_abs: 5
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
    input_feature_source: raw_features
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    input_feature_source: raw_features
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.5186
    std: 0.0443
    paper_value: 0.5186
    paper_std: 0.0443
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
    feature_source_evidence: Each node is a paper with 128-dimensional word2vec features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Test set MRR on ogbl-citation2
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5186
    at_pub_std: 0.0443
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
    true_value: 0.5186
    true_std: 0.0443
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5186
    sort_std: 0.0443
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
  - model: PLNLP
    model_key: plnlp
    model_plain: PLNLP
    value: 0.7059
    std: 0.0029
    paper_value: 0.7059
    paper_std: 0.0029
    metric: Hits@50
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
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-04'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7059
    true_std: 0.0029
    value_gap_source_arxiv: '2210.01301'
    value_gap_source_title: 'GIDN: A Lightweight Graph Inception Diffusion Network
      for High-efficient Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7059
    sort_std: 0.0029
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
  - model: HOP-Rec
    model_key: hop-rec
    model_plain: HOP-Rec
    value: 0.7012
    std: 0.0016
    paper_value: 0.7012
    paper_std: 0.0016
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7012
    true_std: 0.0016
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7012
    sort_std: 0.0016
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4714
    std: 0.0145
    paper_value: 0.4714
    paper_std: 0.0145
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4714
    at_pub_std: 0.0145
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6621
    true_std: 0.0033
    value_gap_source_arxiv: '2409.17475'
    value_gap_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.19070000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0033
    global_rank: 7
    paper_rank: 69
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AA+Proposal Set
    model_key: aa+proposal set
    model_plain: AA+Proposal Set
    value: 0.6548
    std: 0.0
    paper_value: 0.6548
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6548
    true_std: 0.0
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6548
    sort_std: 0.0
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
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.6474
    std: 0.0033
    paper_value: 0.6474
    paper_std: 0.0033
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    value: 0.6417
    std: 0.0
    paper_value: 0.6417
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6417
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6435
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.0017999999999999128
    has_value_note: false
    value_note: ''
    sort_value: 0.6435
    sort_std: 0.0
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.6137
    std: 0.0
    paper_value: 0.6137
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6137
    true_std: 0.0
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6137
    sort_std: 0.0
    global_rank: 22
    paper_rank: 22
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5944
    true_std: 0.0137
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.04810000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5944
    sort_std: 0.0137
    global_rank: 23
    paper_rank: 30
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.5037
    std: 0.0034
    paper_value: 0.5037
    paper_std: 0.0034
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.504
    at_pub_std: 0.003
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.504
    true_std: 0.003
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.504
    sort_std: 0.003
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.4888
    std: 0.0054
    paper_value: 0.4888
    paper_std: 0.0054
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.489
    at_pub_std: 0.005
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4929
    true_std: 0.0064
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.0040999999999999925
    has_value_note: false
    value_note: ''
    sort_value: 0.4929
    sort_std: 0.0064
    global_rank: 55
    paper_rank: 61
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.3886
    std: 0.0029
    paper_value: 0.3886
    paper_std: 0.0029
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
    input_feature_source: raw_features
    feature_source_evidence: All nodes come with 128-dimensional features.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the official ogbl-collab test split.
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.389
    at_pub_std: 0.003
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.00040000000000001146
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4181
    true_std: 0.0167
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.029500000000000026
    has_value_note: false
    value_note: ''
    sort_value: 0.4181
    sort_std: 0.0167
    global_rank: 82
    paper_rank: 84
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
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
  - model: PLNLP
    model_key: plnlp
    model_plain: PLNLP
    value: 0.9088
    std: 0.0313
    paper_value: 0.9088
    paper_std: 0.0313
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9088
    at_pub_std: 0.0313
    at_pub_source_arxiv: '2012.15024'
    at_pub_source_title: Adaptive Graph Diffusion Networks
    at_pub_source_date_iso: '2020-12-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9088
    true_std: 0.0313
    value_gap_source_arxiv: '2012.15024'
    value_gap_source_title: Adaptive Graph Diffusion Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9088
    sort_std: 0.0313
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
  - model: SAGE+Edge Attr
    model_key: sage+edge attr
    model_plain: SAGE+Edge Attr
    value: 0.8781
    std: 0.0447
    paper_value: 0.8781
    paper_std: 0.0447
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8781
    true_std: 0.0447
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8781
    sort_std: 0.0447
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
  - model: CFLP (w/ JKNet)
    model_key: cflp (w/ jknet)
    model_plain: CFLP (w/ JKNet)
    value: 0.8608
    std: 0.0198
    paper_value: 0.8608
    paper_std: 0.0198
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8608
    true_std: 0.0198
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8608
    sort_std: 0.0198
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
  - model: SAGE+Proposal Set
    model_key: sage+proposal set
    model_plain: SAGE+Proposal Set
    value: 0.7495
    std: 0.0317
    paper_value: 0.7495
    paper_std: 0.0317
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7495
    true_std: 0.0317
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7495
    sort_std: 0.0317
    global_rank: 17
    paper_rank: 17
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    true_value: 0.539
    true_std: 0.0474
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.539
    sort_std: 0.0474
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3707
    std: 0.0507
    paper_value: 0.3707
    paper_std: 0.0507
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3707
    at_pub_std: 0.0507
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.499
    true_std: 0.0723
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.12830000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.499
    sort_std: 0.0723
    global_rank: 28
    paper_rank: 32
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3056
    at_pub_std: 0.0386
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
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.2246
    std: 0.029
    paper_value: 0.2246
    paper_std: 0.029
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.264
    at_pub_std: 0.061
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.03940000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.264
    true_std: 0.061
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.03940000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.264
    sort_std: 0.061
    global_rank: 44
    paper_rank: 48
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.2326
    std: 0.0209
    paper_value: 0.2326
    paper_std: 0.0209
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.233
    at_pub_std: 0.021
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00040000000000001146
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.233
    true_std: 0.021
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000001146
    has_value_note: false
    value_note: ''
    sort_value: 0.233
    sort_std: 0.021
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1861
    at_pub_std: 0.0
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
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1773
    at_pub_std: 0.0
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
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.1368
    std: 0.0475
    paper_value: 0.1368
    paper_std: 0.0475
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on ogbl-ddi test set
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.137
    at_pub_std: 0.047
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00020000000000000573
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.137
    true_std: 0.047
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00020000000000000573
    has_value_note: false
    value_note: ''
    sort_value: 0.137
    sort_std: 0.047
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.5324
    std: 0.0
    paper_value: 0.5324
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5324
    true_std: 0.0
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5324
    sort_std: 0.0
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.1655
    std: 0.024
    paper_value: 0.1655
    paper_std: 0.024
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5013
    true_std: 0.0055
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.3358
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.0055
    global_rank: 13
    paper_rank: 58
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
  - model: PLNLP
    model_key: plnlp
    model_plain: PLNLP
    value: 0.3238
    std: 0.0258
    paper_value: 0.3238
    paper_std: 0.0258
    metric: Hits@100
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3238
    at_pub_std: 0.0258
    at_pub_source_arxiv: '2012.15024'
    at_pub_source_title: Adaptive Graph Diffusion Networks
    at_pub_source_date_iso: '2020-12-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3238
    true_std: 0.0258
    value_gap_source_arxiv: '2012.15024'
    value_gap_source_title: Adaptive Graph Diffusion Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3238
    sort_std: 0.0258
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.3229
    std: 0.0094
    paper_value: 0.3229
    paper_std: 0.0094
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.323
    at_pub_std: 0.009
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.323
    true_std: 0.009
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.323
    sort_std: 0.009
    global_rank: 39
    paper_rank: 39
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.2302
    std: 0.0163
    paper_value: 0.2302
    paper_std: 0.0163
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.289
    at_pub_std: 0.015
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.05879999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.289
    true_std: 0.015
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.05879999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.289
    sort_std: 0.015
    global_rank: 42
    paper_rank: 51
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.276
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.0005000000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
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
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.2226
    std: 0.0083
    paper_value: 0.2226
    paper_std: 0.0083
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.223
    at_pub_std: 0.008
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00040000000000001146
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.223
    true_std: 0.008
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000001146
    has_value_note: false
    value_note: ''
    sort_value: 0.223
    sort_std: 0.008
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Classification
    model_key: classification
    model_plain: Classification
    value: 0.1655
    std: null
    paper_value: 0.1655
    paper_std: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on the official ogbl-ppa test split
    date: Dec 6, 2021
    date_display: Dec 2021
    date_iso: '2021-12-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-12-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1655
    true_std: null
    value_gap_source_arxiv: '2112.02936'
    value_gap_source_title: Pairwise Learning for Neural Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1655
    sort_std: null
    global_rank: 60
    paper_rank: 60
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
single_proposed_model: PLNLP
main_figure: /figures/2112.02936/main_figure.jpegoptim.jpg
---

