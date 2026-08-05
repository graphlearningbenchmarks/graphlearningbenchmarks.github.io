---
title: Simplifying Subgraph Representation Learning for Scalable Link Prediction
arxiv_id: '2301.12562'
source_url: ''
authors:
- name: Paul Louis
  orcid: null
  s2_author_id: '2173449532'
  s2_url: null
- name: Shweta Ann Jacob
  orcid: null
  s2_author_id: '2173258768'
  s2_url: null
- name: Amirali Salehi-Abari
  orcid: null
  s2_author_id: '1403711294'
  s2_url: null
published_date: Jan 29, 2023
published_date_iso: '2023-01-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Link prediction on graphs is a fundamental problem, addressing the task
  of predicting potential connections between entities in a network, enabling the
  identification of missing or future relationships. Its applications span various
  domains, including social networks, recommendation systems, and biological networks,
  where predicting links can enhance our understanding of network structure and facilitate
  more effective information dissemination or resource allocation. Subgraph representation
  learning approaches (SGRLs), by transforming link prediction to graph classification
  on the subgraphs around the links, have achieved state-of-the-art performance in
  link prediction. However, SGRLs are computationally expensive and not scalable to
  large-scale graphs due to expensive subgraph-level operations. To unlock the scalability
  of SGRLs, we propose a new class of SGRLs, that we call Scalable Simplified SGRL
  (S3GRL). Aimed at faster training and inference, S3GRL simplifies the message passing
  and aggregation operations in each link's subgraph. S3GRL, as a scalability framework,
  accommodates various subgraph sampling strategies and diffusion operators to emulate
  computationally expensive SGRLs. We propose multiple instances of S3GRL and empirically
  study them on small to large-scale graphs. Our extensive experiments demonstrate
  that the proposed S3GRL models scale up SGRLs without significant performance compromise
  (even with considerable gains in some cases), while offering substantially lower
  computational footprints (e.g., multi-fold inference and training speedup).
codebase_url: https://github.com/venomouscyanide/S3GRL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 3
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id002
  dataset: ogbl-citation2
  rows:
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.9072
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
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/GraphPKU/Refined-GAE
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
  - model: CFG
    model_key: cfg
    model_plain: CFG
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
  - model: SIEG
    model_key: sieg
    model_plain: SIEG
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
  - model: PoS+
    model_key: pos+
    model_plain: PoS+
    value: 0.8814
    std: 0.0008
    paper_value: 0.8814
    paper_std: 0.0008
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-01-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8814
    true_std: 0.0008
    value_gap_source_arxiv: '2301.12562'
    value_gap_source_title: Simplifying Subgraph Representation Learning for Scalable
      Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8814
    sort_std: 0.0008
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
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8767
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-11-06'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2411.03845'
    value_gap_source_title: Reconsidering the Performance of GAE in Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0032
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8756
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-11-06'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2411.03845'
    value_gap_source_title: Reconsidering the Performance of GAE in Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8756
    sort_std: 0.0011
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
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
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
    global_rank: 17
    paper_rank: 26
    rank_delta: 9
    rank_delta_abs: 9
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
    value: 0.8367
    std: 0.0007
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.17475'
    title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
      Networks
    date: Sep 26, 2024
    date_display: Sep 2024
    date_iso: '2024-09-26'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/tensor-gales/HeteLinkPred
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.8367
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8264
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8264
    true_std: 0.0001
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000006697
    has_value_note: false
    value_note: ''
    sort_value: 0.8264
    sort_std: 0.0001
    global_rank: 38
    paper_rank: 38
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
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
    global_rank: 59
    paper_rank: 68
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
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
    global_rank: 61
    paper_rank: 70
    rank_delta: 9
    rank_delta_abs: 9
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
    value: 0.3917
    std: 0.0044
    metric: MRR
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
    global_rank: 78
    sort_value: 0.3917
    sort_std: 0.0044
    comparison_type: global_top
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
  dataset: ogbl-ddi
  rows:
  - model: ELGNN
    model_key: elgnn
    model_plain: ELGNN
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
  - model: GIDN
    model_key: gidn
    model_plain: GIDN
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
  - model: AGDN
    model_key: agdn
    model_plain: AGDN
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
    source_ref: chamberlain2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7851
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7851
    sort_std: 0.0136
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.6719
    std: 0.0118
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.16687'
    title: Link Prediction with Untrained Message Passing Layers
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 22
    sort_value: 0.6719
    sort_std: 0.0118
    comparison_type: global_top
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.446
    at_pub_std: 0.0887
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07530000000000003
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6476
    true_std: 0.0145
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.2769
    has_value_note: false
    value_note: ''
    sort_value: 0.6476
    sort_std: 0.0145
    global_rank: 26
    paper_rank: 56
    rank_delta: 30
    rank_delta_abs: 30
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.539
    at_pub_std: 0.0474
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-22'
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
    value_gap_source_arxiv: '2310.14166'
    value_gap_source_title: Ensemble Learning for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.539
    sort_std: 0.0474
    global_rank: 40
    paper_rank: 40
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3056
    at_pub_std: 0.0386
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4974
    true_std: 0.0239
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.19180000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4974
    sort_std: 0.0239
    global_rank: 46
    paper_rank: 62
    rank_delta: 16
    rank_delta_abs: 16
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1861
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3975
    true_std: null
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.21140000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3975
    sort_std: null
    global_rank: 53
    paper_rank: 78
    rank_delta: 25
    rank_delta_abs: 25
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1773
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3869
    true_std: null
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.2096
    has_value_note: false
    value_note: ''
    sort_value: 0.3869
    sort_std: null
    global_rank: 54
    paper_rank: 81
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PoS+
    model_key: pos+
    model_plain: PoS+
    value: 0.2224
    std: 0.0336
    paper_value: 0.2224
    paper_std: 0.0336
    metric: Hits@20
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-01-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2224
    true_std: 0.0336
    value_gap_source_arxiv: '2301.12562'
    value_gap_source_title: Simplifying Subgraph Representation Learning for Scalable
      Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2224
    sort_std: 0.0336
    global_rank: 74
    paper_rank: 74
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
- &id001
  dataset: ogbl-ppa
  rows:
  - model: Optimized GAE
    model_key: optimized gae
    model_plain: Optimized GAE
    value: 0.7841
    std: 0.0083
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/GraphPKU/Refined-GAE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7841
    sort_std: 0.0083
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPLP
    model_key: mplp
    model_plain: MPLP
    value: 0.6524
    std: 0.015
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_display: Nov 2024
    date_iso: '2024-11-06'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/GraphPKU/Refined-GAE
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
  - model: OGB Leader
    model_key: ogb leader
    model_plain: OGB Leader
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
    global_rank: 3
    sort_value: 0.6524
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.5013
    std: 0.0055
    metric: Hits@100
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_display: Mar 2023
    date_iso: '2023-03-01'
    venue: ACM Transactions on Knowledge Discovery from Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 16
    sort_value: 0.5013
    sort_std: 0.0055
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4985
    at_pub_std: 0.002
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4985
    sort_std: 0.002
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
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.488
    at_pub_std: 0.0316
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.488
    sort_std: 0.0316
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
    global_rank: 26
    sort_value: 0.46
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PoS+
    model_key: pos+
    model_plain: PoS+
    value: 0.4242
    std: 0.018
    paper_value: 0.4242
    paper_std: 0.018
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-01-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4242
    true_std: 0.018
    value_gap_source_arxiv: '2301.12562'
    value_gap_source_title: Simplifying Subgraph Representation Learning for Scalable
      Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4242
    sort_std: 0.018
    global_rank: 35
    paper_rank: 35
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3245
    at_pub_std: 0.0
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3245
    sort_std: 0.0
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
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.187
    at_pub_std: 0.013
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-06-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0002999999999999947
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3084
    true_std: 0.0178
    value_gap_source_arxiv: '2406.16687'
    value_gap_source_title: Link Prediction with Untrained Message Passing Layers
    value_gap_source_is_current_paper: false
    value_gap: 0.1217
    has_value_note: false
    value_note: ''
    sort_value: 0.3084
    sort_std: 0.0178
    global_rank: 49
    paper_rank: 63
    rank_delta: 14
    rank_delta_abs: 14
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2765
    at_pub_std: 0.0
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2765
    sort_std: 0.0
    global_rank: 53
    paper_rank: 53
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Official OGB split
    date: Jan 29, 2023
    date_display: Jan 2023
    date_iso: '2023-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1655
    at_pub_std: 0.024
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-01-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1655
    true_std: 0.024
    value_gap_source_arxiv: '2301.12562'
    value_gap_source_title: Simplifying Subgraph Representation Learning for Scalable
      Link Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1655
    sort_std: 0.024
    global_rank: 68
    paper_rank: 68
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
    - dataset: ogbl-ddi
      dataset_slug: ogbl-ddi
main_figure: /figures/2301.12562/main_figure.jpegoptim.jpg
---

