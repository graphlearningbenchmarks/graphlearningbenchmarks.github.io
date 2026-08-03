---
title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
arxiv_id: '2412.16435'
source_url: ''
authors:
- name: Yuchen Yan
  orcid: null
  s2_author_id: '2274018166'
  s2_url: null
- name: Yuzhong Chen
  orcid: null
  s2_author_id: '2215477428'
  s2_url: null
- name: Huiyuan Chen
  orcid: null
  s2_author_id: '2284864789'
  s2_url: null
- name: Xiaoting Li
  orcid: null
  s2_author_id: '2336880050'
  s2_url: null
- name: Zhe Xu
  orcid: null
  s2_author_id: '2319221713'
  s2_url: null
- name: Zhichen Zeng
  orcid: null
  s2_author_id: '2215437587'
  s2_url: null
- name: Zhining Liu
  orcid: null
  s2_author_id: '2257083296'
  s2_url: null
- name: Hanghang Tong
  orcid: null
  s2_author_id: '2278450099'
  s2_url: null
published_date: Dec 21, 2024
published_date_iso: '2024-12-21'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks (GNNs) have exhibited remarkable efficacy in diverse
  graph learning tasks, particularly on static homophilic graphs. Recent attention
  has pivoted towards more intricate structures, encompassing (1) static heterophilic
  graphs encountering the edge heterophily issue in the spatial domain and (2) event-based
  continuous graphs in the temporal domain. State-of-the-art (SOTA) has been concurrently
  addressing these two lines of work but tends to overlook the presence of heterophily
  in the temporal domain, constituting the temporal heterophily issue. Furthermore,
  we highlight that the edge heterophily issue and the temporal heterophily issue
  often co-exist in event-based continuous graphs, giving rise to the temporal edge
  heterophily challenge. To tackle this challenge, this paper first introduces the
  temporal edge heterophily measurement. Subsequently, we propose the emporal terophilic
  raph onvolutional etwork (THeGCN), an innovative model that incorporates the low/high-pass
  graph signal filtering technique to accurately capture both edge (spatial) heterophily
  and temporal heterophily. Specifically, the THeGCN\ model consists of two key components:
  a sampler and an aggregator. The sampler selects events relevant to a node at a
  given moment. Then, the aggregator executes message-passing, encoding temporal information,
  node attributes, and edge attributes into node embeddings. Extensive experiments
  conducted on 5 real-world datasets validate the efficacy of THeGCN.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- THeGCN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Reddit
  rows:
  - model: GCNII
    model_key: ne-asgcn
    model_plain: GCNII
    value: 0.9758
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.16097'
    title: Neighbor Enhanced Graph Convolutional Networks for Node Classification
      and Recommendation
    date: Mar 1, 2022
    date_display: Mar 2022
    date_iso: '2022-03-01'
    venue: Knowledge-Based Systems
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9758
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCNII
    model_key: gcmae
    model_plain: GCNII
    value: 0.9713
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.15523'
    title: Generative and Contrastive Paradigms Are Complementary for Graph Self-Supervised
      Learning
    date: Oct 24, 2023
    date_display: Oct 2023
    date_iso: '2023-10-24'
    venue: IEEE International Conference on Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9713
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gat+norm.adj.
    model_plain: GCNII
    value: 0.9706
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
    arxiv_id: '2103.13355'
    title: Bag of Tricks for Node Classification with Graph Neural Networks
    date: Mar 24, 2021
    date_display: Mar 2021
    date_iso: '2021-03-24'
    venue: null
    codebase_url: https://github.com/espylapiza/Bag-of-Tricks-for-Node-Classification-with-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9706
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.3027
    std: 0.0162
    paper_value: 0.3027
    paper_std: 0.0162
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
    source_ref: velivckovic2017graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.965
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2406.12059'
    at_pub_source_title: A Scalable and Effective Alternative to Graph Transformers
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.6622999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.965
    true_std: 0.0011
    value_gap_source_arxiv: '2406.12059'
    value_gap_source_title: A Scalable and Effective Alternative to Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.6622999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.965
    sort_std: 0.0011
    global_rank: 17
    paper_rank: 144
    rank_delta: 127
    rank_delta_abs: 127
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Scalable and Effective Alternative to Graph Transformers
    comparison_source_arxiv: '2406.12059'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2973
    std: 0.0308
    paper_value: 0.2973
    paper_std: 0.0308
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
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9648
    at_pub_std: null
    at_pub_source_arxiv: '1907.10903'
    at_pub_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on Node
      Classification'
    at_pub_source_date_iso: '2019-07-25'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-07-25'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.6675
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9648
    true_std: null
    value_gap_source_arxiv: '1907.10903'
    value_gap_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on
      Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.6675
    has_value_note: false
    value_note: ''
    sort_value: 0.9648
    sort_std: null
    global_rank: 21
    paper_rank: 145
    rank_delta: 124
    rank_delta_abs: 124
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks
      on Node Classification'
    comparison_source_arxiv: '1907.10903'
    is_best: true
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.3044
    std: 0.0178
    paper_value: 0.3044
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
    table_ref: Table 1
    source_ref: klicpera2018predict
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.95
    at_pub_std: null
    at_pub_source_arxiv: '2102.10739'
    at_pub_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.6456
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '2102.10739'
    value_gap_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.6456
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 58
    paper_rank: 144
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    comparison_source_arxiv: '2102.10739'
    is_best: false
    is_std_outlier: false
  - model: THeGCN
    model_key: thegcn
    model_plain: THeGCN
    value: 0.3319
    std: 0.0409
    paper_value: 0.3319
    paper_std: 0.0409
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3319
    true_std: 0.0409
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3319
    sort_std: 0.0409
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
  - model: APAN
    model_key: apan
    model_plain: APAN
    value: 0.3195
    std: 0.0218
    paper_value: 0.3195
    paper_std: 0.0218
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
    source_ref: wang2021apan
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3195
    true_std: 0.0218
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3195
    sort_std: 0.0218
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
  - model: DySAT
    model_key: dysat
    model_plain: DySAT
    value: 0.3177
    std: 0.0196
    paper_value: 0.3177
    paper_std: 0.0196
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
    source_ref: sankar2020dysat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3177
    true_std: 0.0196
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3177
    sort_std: 0.0196
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3124
    std: 0.0187
    paper_value: 0.3124
    paper_std: 0.0187
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
    source_ref: chien2020adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3124
    true_std: 0.0187
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3124
    sort_std: 0.0187
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
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.308
    std: 0.0199
    paper_value: 0.308
    paper_std: 0.0199
    metric: Accuracy
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
    source_ref: kumar2019predicting
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.308
    true_std: 0.0199
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.308
    sort_std: 0.0199
    global_rank: 144
    paper_rank: 144
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.3018
    std: 0.0235
    paper_value: 0.3018
    paper_std: 0.0235
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
    source_ref: bo2021beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3018
    true_std: 0.0235
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3018
    sort_std: 0.0235
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
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.2929
    std: 0.0472
    paper_value: 0.2929
    paper_std: 0.0472
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
    source_ref: xu2020inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2929
    true_std: 0.0472
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2929
    sort_std: 0.0472
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.1578
    std: 0.0105
    paper_value: 0.1578
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
    table_ref: Table 1
    source_ref: rossi2020temporal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 60/20/20% split for training, validation, and testing.
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1578
    true_std: 0.0105
    value_gap_source_arxiv: '2412.16435'
    value_gap_source_title: 'THeGCN: Temporal Heterophilic Graph Convolutional Network'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1578
    sort_std: 0.0105
    global_rank: 148
    paper_rank: 148
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
  dataset_primary_metric: F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
single_proposed_model: THeGCN
---

