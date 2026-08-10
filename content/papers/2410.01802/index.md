---
title: 'PROXI: Challenging the GNNs for Link Prediction'
arxiv_id: '2410.01802'
source_url: ''
authors:
- name: Astrit Tola
  orcid: null
  s2_author_id: '104327236'
  s2_url: null
- name: Jack Myrick
  orcid: null
  s2_author_id: '2323788342'
  s2_url: null
- name: B. Coskunuzer
  orcid: null
  s2_author_id: '101047611'
  s2_url: null
published_date: Oct 2, 2024
published_date_iso: '2024-10-02'
published_venue: TMLR 2024
published_conference: TMLR 2024
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: Over the past decade, Graph Neural Networks (GNNs) have transformed graph
  representation learning. In the widely adopted message-passing GNN framework, nodes
  refine their representations by aggregating information from neighboring nodes iteratively.
  While GNNs excel in various domains, recent theoretical studies have raised concerns
  about their capabilities. GNNs aim to address various graph-related tasks by utilizing
  such node representations, however, this one-size-fits-all approach proves suboptimal
  for diverse tasks. Motivated by these observations, we conduct empirical tests to
  compare the performance of current GNN models with more conventional and direct
  methods in link prediction tasks. Introducing our model, PROXI, which leverages
  proximity information of node pairs in both graph and attribute spaces, we find
  that standard machine learning (ML) models perform competitively, even outperforming
  cutting-edge GNN models when applied to these proximity metrics derived from node
  neighborhoods and attributes. This holds true across both homophilic and heterophilic
  networks, as well as small and large benchmark datasets, including those from the
  Open Graph Benchmark (OGB). Moreover, we show that augmenting traditional GNNs with
  PROXI significantly boosts their link prediction performance. Our empirical findings
  corroborate the previously mentioned theoretical observations and imply that there
  exists ample room for enhancement in current GNN models to reach their potential.
codebase_url: https://github.com/workrep20232/PROXI
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- PROXI
mrr: 0.55
adjusted_mrr: 0.3667
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
- &id001
  dataset: ogbl-collab
  rows:
  - model: PROXI
    model_key: proxi
    model_plain: PROXI
    value: 0.765
    std: 0.0027
    paper_value: 0.765
    paper_std: 0.0027
    metric: Hits@50
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: combines all relevant proximity information about node
      pairs... structural proximity... and domain proximity
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.765
    true_std: 0.0027
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.765
    sort_std: 0.0027
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
  - model: OGB Leader
    model_key: ogb leader
    model_plain: OGB Leader
    value: 0.7129
    std: 0.0018
    paper_value: 0.7129
    paper_std: 0.0018
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: OGB Leaderboard
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7129
    true_std: 0.0018
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7129
    sort_std: 0.0018
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIDN
    model_key: gidn
    model_plain: GIDN
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
  - model: NCNC
    model_key: ncnc
    model_plain: NCNC
    value: 0.6597
    std: 0.0103
    paper_value: 0.6597
    paper_std: 0.0103
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wang2023neural
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6661
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2310.11009'
    at_pub_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.006400000000000072
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6661
    true_std: 0.0071
    value_gap_source_arxiv: '2310.11009'
    value_gap_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.006400000000000072
    has_value_note: false
    value_note: ''
    sort_value: 0.6661
    sort_std: 0.0071
    global_rank: 9
    paper_rank: 13
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5496
    std: 0.0318
    paper_value: 0.5496
    paper_std: 0.0318
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6621
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2409.17475'
    at_pub_source_title: On the Impact of Feature Heterophily on Link Prediction with
      Graph Neural Networks
    at_pub_source_date_iso: '2024-09-26'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.11250000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.11250000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0033
    global_rank: 10
    paper_rank: 33
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    comparison_source_arxiv: '2409.17475'
    is_best: false
    is_std_outlier: false
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.6613
    std: 0.0061
    paper_value: 0.6613
    paper_std: 0.0061
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yun2021neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.5752
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.08609999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6613
    true_std: 0.0061
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6613
    sort_std: 0.0061
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    comparison_source_arxiv: '2206.04216'
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.6459
    std: 0.0046
    paper_value: 0.6459
    paper_std: 0.0046
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chamberlain2022graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6594
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2310.09516'
    at_pub_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    at_pub_source_date_iso: '2023-10-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.013499999999999956
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6594
    true_std: 0.0058
    value_gap_source_arxiv: '2310.11009'
    value_gap_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.013499999999999956
    has_value_note: false
    value_note: ''
    sort_value: 0.6594
    sort_std: 0.0058
    global_rank: 14
    paper_rank: 20
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    comparison_source_arxiv: '2310.09516'
    is_best: false
    is_std_outlier: false
  - model: NCN
    model_key: ncn
    model_plain: NCN
    value: 0.6386
    std: 0.0051
    paper_value: 0.6386
    paper_std: 0.0051
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: wang2023neural
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6476
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2310.11009'
    at_pub_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6476
    true_std: 0.0087
    value_gap_source_arxiv: '2310.11009'
    value_gap_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.6476
    sort_std: 0.0087
    global_rank: 19
    paper_rank: 25
    rank_delta: 6
    rank_delta_abs: 6
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
    value: 0.6337
    std: 0.0069
    paper_value: 0.6337
    paper_std: 0.0069
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhang2018link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6474
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.013699999999999934
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6474
    true_std: 0.0043
    value_gap_source_arxiv: '2310.11009'
    value_gap_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.013699999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.0043
    global_rank: 20
    paper_rank: 25
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.5944
    std: 0.0137
    paper_value: 0.5944
    paper_std: 0.0137
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.5463
    at_pub_std: 0.0112
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.04810000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5944
    true_std: 0.0137
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5944
    sort_std: 0.0137
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Pairwise Learning for Neural Link Prediction
    comparison_source_arxiv: '2112.02936'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.55
    std: 0.0328
    paper_value: 0.55
    paper_std: 0.0328
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: velivckovic2017graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.5643
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2303.00170'
    at_pub_source_title: Asymmetric Learning for Graph Neural Network based Link Prediction
    at_pub_source_date_iso: '2023-03-01'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.01429999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5643
    true_std: 0.0086
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.01429999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.5643
    sort_std: 0.0086
    global_rank: 32
    paper_rank: 33
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.5463
    std: 0.0112
    metric: Hits@50
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.12488'
    title: 'Bring Your Own View: Graph Neural Networks for Link Prediction with Personalized
      Subgraph Selection'
    date: Dec 23, 2022
    date_display: Dec 2022
    date_iso: '2022-12-23'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/qiaoyu-tan/PS2
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 39
    sort_value: 0.5463
    sort_std: 0.0112
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: N2Vec
    model_key: n2vec
    model_plain: N2Vec
    value: 0.4906
    std: 0.0104
    paper_value: 0.4906
    paper_std: 0.0104
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: grover2016node2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4906
    true_std: 0.0104
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4906
    sort_std: 0.0104
    global_rank: 72
    paper_rank: 72
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
    value: 0.4438
    std: 0.0347
    metric: Hits@50
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
    global_rank: 91
    sort_value: 0.4438
    sort_std: 0.0347
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.4181
    std: 0.0167
    paper_value: 0.4181
    paper_std: 0.0167
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: menon2011link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on the standard ogbl-collab link prediction task and split.
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.389
    at_pub_std: 0.003
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.029100000000000015
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4181
    true_std: 0.0167
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4181
    sort_std: 0.0167
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
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
- &id002
  dataset: ogbl-ppa
  rows:
  - model: OGB Leader
    model_key: ogb leader
    model_plain: OGB Leader
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
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: li2023evaluating
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6524
    true_std: 0.015
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
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
    is_best: true
    is_std_outlier: false
  - model: PRB
    model_key: prb
    model_plain: PRB
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
    global_rank: 2
    sort_value: 0.6347
    sort_std: 0.0175
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LPFormer
    model_key: lpformer
    model_plain: LPFormer
    value: 0.6332
    std: 0.0063
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11009'
    title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/HarryShomer/LPFormer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6332
    sort_std: 0.0063
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NCNC
    model_key: ncnc
    model_plain: NCNC
    value: 0.6261
    std: 0.0076
    paper_value: 0.6261
    paper_std: 0.0076
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
    table_ref: Table 1
    source_ref: wang2023neural
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6264
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2310.00793'
    at_pub_source_title: 'Revisiting Link Prediction: a data perspective'
    at_pub_source_date_iso: '2023-10-01'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6264
    true_std: 0.0079
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.6264
    sort_std: 0.0079
    global_rank: 4
    paper_rank: 5
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCN
    model_key: ncn
    model_plain: NCN
    value: 0.6263
    std: 0.0115
    paper_value: 0.6263
    paper_std: 0.0115
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
    table_ref: Table 1
    source_ref: wang2023neural
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.6119
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2310.11009'
    at_pub_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.014399999999999968
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6263
    true_std: 0.0115
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6263
    sort_std: 0.0115
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
  - model: PROXI
    model_key: proxi
    model_plain: PROXI
    value: 0.5036
    std: 0.0076
    paper_value: 0.5036
    paper_std: 0.0076
    metric: Hits@100
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: combines all relevant proximity information about node
      pairs... structural proximity... and domain proximity
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5036
    true_std: 0.0076
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5036
    sort_std: 0.0076
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
    value: 0.4102
    std: 0.0194
    paper_value: 0.4102
    paper_std: 0.0194
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
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.5013
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2303.00170'
    at_pub_source_title: Asymmetric Learning for Graph Neural Network based Link Prediction
    at_pub_source_date_iso: '2023-03-01'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.09109999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.09109999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.0055
    global_rank: 14
    paper_rank: 32
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    comparison_source_arxiv: '2303.00170'
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.4733
    std: 0.0196
    paper_value: 0.4733
    paper_std: 0.0196
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
    table_ref: Table 1
    source_ref: chamberlain2022graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.4985
    at_pub_std: 0.002
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0252
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4985
    true_std: 0.002
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: 0.0252
    has_value_note: false
    value_note: ''
    sort_value: 0.4985
    sort_std: 0.002
    global_rank: 15
    paper_rank: 21
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    comparison_source_arxiv: '2209.15486'
    is_best: false
    is_std_outlier: false
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.4845
    std: 0.0101
    paper_value: 0.4845
    paper_std: 0.0101
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
    table_ref: Table 1
    source_ref: yun2021neo
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.4913
    at_pub_std: 0.006
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.006800000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4913
    true_std: 0.006
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: 0.006800000000000028
    has_value_note: false
    value_note: ''
    sort_value: 0.4913
    sort_std: 0.006
    global_rank: 18
    paper_rank: 19
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.484
    std: 0.0561
    paper_value: 0.484
    paper_std: 0.0561
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
    table_ref: Table 1
    source_ref: zhang2018link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.488
    at_pub_std: 0.0316
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.488
    true_std: 0.0316
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: 0.0316
    global_rank: 19
    paper_rank: 20
    rank_delta: 1
    rank_delta_abs: 1
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
    value: 0.46
    std: 0.0
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_display: Oct 2023
    date_iso: '2023-10-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 23
    sort_value: 0.46
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.284
    std: 0.0462
    paper_value: 0.284
    paper_std: 0.0462
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
    table_ref: Table 1
    source_ref: menon2011link
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.323
    at_pub_std: 0.009
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.039000000000000035
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
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.323
    sort_std: 0.009
    global_rank: 42
    paper_rank: 48
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2957
    std: 0.029
    paper_value: 0.2957
    paper_std: 0.029
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.3084
    at_pub_std: 0.0178
    at_pub_source_arxiv: '2406.16687'
    at_pub_source_title: Link Prediction with Untrained Message Passing Layers
    at_pub_source_date_iso: '2024-06-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.012699999999999989
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3084
    true_std: 0.0178
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.012699999999999989
    has_value_note: false
    value_note: ''
    sort_value: 0.3084
    sort_std: 0.0178
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: N2Vec
    model_key: n2vec
    model_plain: N2Vec
    value: 0.2624
    std: 0.0096
    paper_value: 0.2624
    paper_std: 0.0096
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
    table_ref: Table 1
    source_ref: grover2016node2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa test split
    date: Oct 2, 2024
    date_display: Oct 2024
    date_iso: '2024-10-02'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
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
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2624
    true_std: 0.0096
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2624
    sort_std: 0.0096
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.1655
    std: 0.024
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.12562'
    title: Simplifying Subgraph Representation Learning for Scalable Link Prediction
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    venue: arXiv.org
    codebase_url: https://github.com/venomouscyanide/S3GRL
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 63
    sort_value: 0.1655
    sort_std: 0.024
    comparison_type: global_top
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
    - dataset: ogbl-collab
      dataset_slug: ogbl-collab
    - dataset: ogbl-ppa
      dataset_slug: ogbl-ppa
single_proposed_model: PROXI
main_figure: /figures/2410.01802/main_figure.jpegoptim.jpg
---

