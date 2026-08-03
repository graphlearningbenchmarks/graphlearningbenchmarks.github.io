---
title: Simple yet Effective Node Property Prediction on Edge Streams under Distribution
  Shifts
arxiv_id: '2504.00328'
source_url: ''
authors:
- name: Jongha Lee
  orcid: null
  s2_author_id: '2284689477'
  s2_url: null
- name: Taehyung Kwon
  orcid: null
  s2_author_id: '2067591578'
  s2_url: null
- name: Heechan Moon
  orcid: null
  s2_author_id: '2268310784'
  s2_url: null
- name: Kijung Shin
  orcid: null
  s2_author_id: '2287013089'
  s2_url: null
published_date: Apr 1, 2025
published_date_iso: '2025-04-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'The problem of predicting node properties (e.g., node classes) in graphs
  has received significant attention due to its broad range of applications. Graphs
  from real-world datasets often evolve over time, with newly emerging edges and dynamically
  changing node properties, posing a significant challenge for this problem. In response,
  temporal graph neural networks (TGNNs) have been developed to predict dynamic node
  properties from a stream of emerging edges. However, our analysis reveals that most
  TGNN-based methods are (a) far less effective without proper node features and,
  due to their complex model architectures, (b) vulnerable to distribution shifts.
  In this paper, we propose SPLASH, a simple yet powerful method for predicting node
  properties on edge streams under distribution shifts. Our key contributions are
  as follows: (1) we propose feature augmentation methods and an automatic feature
  selection method for edge streams, which improve the effectiveness of TGNNs, (2)
  we propose a lightweight MLP-based TGNN architecture that is highly efficient and
  robust under distribution shifts, and (3) we conduct extensive experiments to evaluate
  the accuracy, efficiency, generalization, and qualitative performance of the proposed
  method and its competitors on dynamic node classification, dynamic anomaly detection,
  and node affinity prediction tasks across seven real-world datasets.'
codebase_url: https://github.com/jhsk777/SPLASH
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SPLASH
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
  - model: SPLASH
    model_key: splash
    model_plain: SPLASH
    value: 0.7358
    std: 0.0028
    paper_value: 0.7358
    paper_std: 0.0028
    metric: AUC
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
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7358
    true_std: 0.0028
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7358
    sort_std: 0.0028
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
  - model: CPDG
    model_key: backbone (tgat)
    model_plain: CPDG
    value: 0.6822
    std: 0.0052
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.10673'
    title: 'Less Can Be More: Unsupervised Graph Pruning for Large-scale Dynamic Graphs'
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    venue: arXiv.org
    codebase_url: https://github.com/EdisonLeeeee/STEP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6822
    sort_std: 0.0052
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPDG
    model_key: pint
    model_plain: CPDG
    value: 0.6731
    std: 0.002
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.15059'
    title: Provably expressive temporal graph networks
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6731
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.61
    std: 0.0088
    paper_value: 0.61
    paper_std: 0.0088
    metric: AUC
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6556
    at_pub_std: 0.007
    at_pub_source_arxiv: '2209.15059'
    at_pub_source_title: Provably expressive temporal graph networks
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.045599999999999974
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6556
    true_std: 0.007
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: false
    value_gap: 0.045599999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.6556
    sort_std: 0.007
    global_rank: 5
    paper_rank: 11
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Provably expressive temporal graph networks
    comparison_source_arxiv: '2209.15059'
    is_best: false
    is_std_outlier: false
  - model: DyGFormer+RF
    model_key: dygformer+rf
    model_plain: DyGFormer+RF
    value: 0.6406
    std: 0.0034
    paper_value: 0.6406
    paper_std: 0.0034
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6406
    true_std: 0.0034
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6406
    sort_std: 0.0034
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
  - model: DyGFormer
    model_key: dygformer
    model_plain: DyGFormer
    value: 0.6371
    std: 0.0067
    paper_value: 0.6371
    paper_std: 0.0067
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yu2023towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6371
    true_std: 0.0067
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6371
    sort_std: 0.0067
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
  - model: GraphMixer
    model_key: graphmixer
    model_plain: GraphMixer
    value: 0.6298
    std: 0.0147
    paper_value: 0.6298
    paper_std: 0.0147
    metric: AUC
    higher_is_better: true
    is_baseline: true
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
    source_ref: cong2022we
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6298
    true_std: 0.0147
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6298
    sort_std: 0.0147
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
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.5522
    std: 0.0103
    paper_value: 0.5522
    paper_std: 0.0103
    metric: AUC
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
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6183
    at_pub_std: 0.027
    at_pub_source_arxiv: '2209.15059'
    at_pub_source_title: Provably expressive temporal graph networks
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.06609999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6183
    true_std: 0.027
    value_gap_source_arxiv: '2209.15059'
    value_gap_source_title: Provably expressive temporal graph networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06609999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6183
    sort_std: 0.027
    global_rank: 11
    paper_rank: 15
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Provably expressive temporal graph networks
    comparison_source_arxiv: '2209.15059'
    is_best: false
    is_std_outlier: false
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.5926
    std: 0.0041
    paper_value: 0.5926
    paper_std: 0.0041
    metric: AUC
    higher_is_better: true
    is_baseline: true
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
    source_ref: tgn_icml_grl2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5552
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2307.02813'
    at_pub_source_title: 'CPDG: A Contrastive Pre-Training Method for Dynamic Graph
      Neural Networks'
    at_pub_source_date_iso: '2023-07-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.03739999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5926
    true_std: 0.0041
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5926
    sort_std: 0.0041
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'CPDG: A Contrastive Pre-Training Method for Dynamic
      Graph Neural Networks'
    comparison_source_arxiv: '2307.02813'
    is_best: false
    is_std_outlier: false
  - model: DySAT
    model_key: dysat
    model_plain: DySAT
    value: 0.569
    std: 0.0234
    paper_value: 0.569
    paper_std: 0.0234
    metric: AUC
    higher_is_better: true
    is_baseline: true
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
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.569
    true_std: 0.0234
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.569
    sort_std: 0.0234
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
  - model: TGAT+RF
    model_key: tgat+rf
    model_plain: TGAT+RF
    value: 0.5613
    std: 0.0407
    paper_value: 0.5613
    paper_std: 0.0407
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5613
    true_std: 0.0407
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5613
    sort_std: 0.0407
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
  - model: TGN+RF
    model_key: tgn+rf
    model_plain: TGN+RF
    value: 0.5385
    std: 0.0212
    paper_value: 0.5385
    paper_std: 0.0212
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5385
    true_std: 0.0212
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5385
    sort_std: 0.0212
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
  - model: DySAT+RF
    model_key: dysat+rf
    model_plain: DySAT+RF
    value: 0.5347
    std: 0.0151
    paper_value: 0.5347
    paper_std: 0.0151
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5347
    true_std: 0.0151
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5347
    sort_std: 0.0151
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
  - model: GraphMixer+RF
    model_key: graphmixer+rf
    model_plain: GraphMixer+RF
    value: 0.5139
    std: 0.0251
    paper_value: 0.5139
    paper_std: 0.0251
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5139
    true_std: 0.0251
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5139
    sort_std: 0.0251
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
  - model: JODIE+RF
    model_key: jodie+rf
    model_plain: JODIE+RF
    value: 0.4872
    std: 0.0056
    paper_value: 0.4872
    paper_std: 0.0056
    metric: AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic Anomaly Detection task on Reddit split 10/10/80
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-01'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4872
    true_std: 0.0056
    value_gap_source_arxiv: '2504.00328'
    value_gap_source_title: Simple yet Effective Node Property Prediction on Edge
      Streams under Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4872
    sort_std: 0.0056
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUC
  metric: AUC
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
single_proposed_model: SPLASH
---

