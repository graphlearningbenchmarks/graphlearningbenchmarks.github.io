---
title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
arxiv_id: '2304.10074'
source_url: ''
authors:
- name: Xiyuan Wang
  orcid: null
  s2_author_id: '2167480960'
  s2_url: null
- name: Pan Li
  orcid: null
  s2_author_id: '1561672016'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '1390814008'
  s2_url: null
published_date: Apr 20, 2023
published_date_iso: '2023-04-20'
published_venue: JMLR 2023
published_conference: JMLR 2023
published_conference_short: JMLR
published_conference_slug: jmlr
abstract: In this paper, we study using graph neural networks (GNNs) for multi-node
  representation learning, where a representation for a set of more than one node
  (such as a link) is to be learned. Existing GNNs are mainly designed to learn single-node
  representations. When used for multi-node representation learning, a common practice
  is to directly aggregate the single-node representations obtained by a GNN. In this
  paper, we show a fundamental limitation of such an approach, namely the inability
  to capture the dependence among multiple nodes in the node set. A straightforward
  solution is to distinguish target nodes from others. Formalizing this idea, we propose,
  which first labels nodes in the graph according to their relationships with the
  target node set before applying a GNN and then aggregates node representations obtained
  in the labeled graph for multi-node representations. Besides node sets in graphs,
  we also extend labeling tricks to posets, subsets and hypergraphs. Experiments verify
  that the labeling trick technique can boost GNNs on various tasks, including undirected
  link prediction, directed link prediction, hyperedge prediction, and subgraph prediction.
  Our work explains the superior performance of previous node-labeling-based methods
  and establishes a theoretical foundation for using GNNs for multi-node representation
  learning.
codebase_url: https://github.com/GraphPKU/LabelingTrick
extraction_model: google/gemma-4-26B-A4B-it
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
  evaluated: 4
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id004
  dataset: ogbl-citation2
  rows:
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
    global_rank: 1
    sort_value: 0.8997
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 2
    sort_value: 0.8987
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LPFormer
    model_key: lpformer
    model_plain: LPFormer
    value: 0.8981
    std: 0.0013
    metric: MRR
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
    sort_value: 0.8981
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on ogbl-citation2 using MRR metric on the
      standard test split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: 0.8767
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
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
    value_gap_source_arxiv: '2310.11009'
    value_gap_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0032
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8705
    std: 0.0004
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
    global_rank: 14
    sort_value: 0.8705
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: 'NO'
    model_key: 'no'
    model_plain: 'NO'
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on ogbl-citation2 using MRR metric on the
      standard test split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8474
    true_std: 0.0021
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8474
    sort_std: 0.0021
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
  - model: ZO-OS
    model_key: zo-os
    model_plain: ZO-OS
    value: 0.8285
    std: 0.0043
    paper_value: 0.8285
    paper_std: 0.0043
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on ogbl-citation2 using MRR metric on the
      standard test split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8285
    true_std: 0.0043
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8285
    sort_std: 0.0043
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
  - model: ZO-S
    model_key: zo-s
    model_plain: ZO-S
    value: 0.8245
    std: 0.0062
    paper_value: 0.8245
    paper_std: 0.0062
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on ogbl-citation2 using MRR metric on the
      standard test split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8245
    true_std: 0.0062
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8245
    sort_std: 0.0062
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
  - model: ZO
    model_key: zo
    model_plain: ZO
    value: 0.785
    std: 0.0108
    paper_value: 0.785
    paper_std: 0.0108
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction task on ogbl-citation2 using MRR metric on the
      standard test split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.785
    true_std: 0.0108
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.785
    sort_std: 0.0108
    global_rank: 46
    paper_rank: 46
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
    global_rank: 72
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
- &id001
  dataset: ogbl-collab
  rows:
  - model: PROXI
    model_key: proxi
    model_plain: PROXI
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
    input_feature_source: raw_features
    feature_source_evidence: combines all relevant proximity information about node
      pairs... structural proximity... and domain proximity
    is_global_top: true
    global_rank: 1
    sort_value: 0.765
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: OGB Leader
    model_key: ogb leader
    model_plain: OGB Leader
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
    input_feature_source: raw_features
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6621
    std: 0.0033
    metric: Hits@50
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
    global_rank: 10
    sort_value: 0.6621
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.5471
    std: 0.0049
    paper_value: 0.5471
    paper_std: 0.0049
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on ogbl-collab undirected link prediction task.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: 0.6474
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.10029999999999994
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
    value_gap: 0.10029999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.0043
    global_rank: 20
    paper_rank: 37
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: ZO-S
    model_key: zo-s
    model_plain: ZO-S
    value: 0.5469
    std: 0.0051
    paper_value: 0.5469
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on ogbl-collab undirected link prediction task.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5469
    true_std: 0.0051
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5469
    sort_std: 0.0051
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
  - model: ZO
    model_key: zo
    model_plain: ZO
    value: 0.5329
    std: 0.0023
    paper_value: 0.5329
    paper_std: 0.0023
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on ogbl-collab undirected link prediction task.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5329
    true_std: 0.0023
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5329
    sort_std: 0.0023
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
  - model: ZO-OS
    model_key: zo-os
    model_plain: ZO-OS
    value: 0.4917
    std: 0.0329
    paper_value: 0.4917
    paper_std: 0.0329
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on ogbl-collab undirected link prediction task.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4917
    true_std: 0.0329
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4917
    sort_std: 0.0329
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
  - model: 'NO'
    model_key: 'no'
    model_plain: 'NO'
    value: 0.4475
    std: 0.0107
    paper_value: 0.4475
    paper_std: 0.0107
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@50 on ogbl-collab undirected link prediction task.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4475
    true_std: 0.0107
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4475
    sort_std: 0.0107
    global_rank: 90
    paper_rank: 90
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
    global_rank: 20
    sort_value: 0.6719
    sort_std: 0.0118
    comparison_type: global_top
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
    feature_source_evidence: The ogbl-ddi graph contains no node features... we give
      up node embeddings in SEAL.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on the ogbl-ddi undirected link prediction task
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
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
    global_rank: 43
    paper_rank: 59
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ZO-OS
    model_key: zo-os
    model_plain: ZO-OS
    value: 0.4124
    std: 0.0149
    paper_value: 0.4124
    paper_std: 0.0149
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
    feature_source_evidence: The ogbl-ddi graph contains no node features, so... the
      GAE methods here use free-parameter node embeddings as the GNN input node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on the ogbl-ddi undirected link prediction task
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4124
    true_std: 0.0149
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4124
    sort_std: 0.0149
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
  - model: 'NO'
    model_key: 'no'
    model_plain: 'NO'
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The ogbl-ddi graph contains no node features, so... the
      GAE methods here use free-parameter node embeddings as the GNN input node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on the ogbl-ddi undirected link prediction task
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3707
    true_std: 0.0507
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3707
    sort_std: 0.0507
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
  - model: ZO-S
    model_key: zo-s
    model_plain: ZO-S
    value: 0.2927
    std: 0.0053
    paper_value: 0.2927
    paper_std: 0.0053
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
    feature_source_evidence: The ogbl-ddi graph contains no node features, so... the
      GAE methods here use free-parameter node embeddings as the GNN input node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on the ogbl-ddi undirected link prediction task
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2927
    true_std: 0.0053
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2927
    sort_std: 0.0053
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ZO
    model_key: zo
    model_plain: ZO
    value: 0.239
    std: 0.0075
    paper_value: 0.239
    paper_std: 0.0075
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
    feature_source_evidence: The ogbl-ddi graph contains no node features, so... the
      GAE methods here use free-parameter node embeddings as the GNN input node features
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@20 on the ogbl-ddi undirected link prediction task
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.239
    true_std: 0.0075
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.239
    sort_std: 0.0075
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
  rank_metric: Hits@20
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: Hits@20
  paper_metrics:
  - Hits@20
  metric: Hits@20
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: ogbl-ppa
  rows:
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
    input_feature_source: raw_features
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
    global_rank: 14
    sort_value: 0.5013
    sort_std: 0.0055
    comparison_type: global_top
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa undirected link prediction task using standard
      split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
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
  - model: ZO-OS
    model_key: zo-os
    model_plain: ZO-OS
    value: 0.4327
    std: 0.0119
    paper_value: 0.4327
    paper_std: 0.0119
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa undirected link prediction task using standard
      split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4327
    true_std: 0.0119
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4327
    sort_std: 0.0119
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
  - model: ZO
    model_key: zo
    model_plain: ZO
    value: 0.3775
    std: 0.0342
    paper_value: 0.3775
    paper_std: 0.0342
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa undirected link prediction task using standard
      split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3775
    true_std: 0.0342
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3775
    sort_std: 0.0342
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
  - model: ZO-S
    model_key: zo-s
    model_plain: ZO-S
    value: 0.3604
    std: 0.045
    paper_value: 0.3604
    paper_std: 0.045
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa undirected link prediction task using standard
      split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3604
    true_std: 0.045
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3604
    sort_std: 0.045
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
  - model: 'NO'
    model_key: 'no'
    model_plain: 'NO'
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Hits@100 on ogbl-ppa undirected link prediction task using standard
      split.
    date: Apr 20, 2023
    date_display: Apr 2023
    date_iso: '2023-04-20'
    published_venue: JMLR 2023
    published_conference: JMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-20'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1867
    true_std: 0.0132
    value_gap_source_arxiv: '2304.10074'
    value_gap_source_title: Improving Graph Neural Networks on Multi-node Tasks with
      the Labeling Trick
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1867
    sort_std: 0.0132
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
    - dataset: ogbl-ddi
      dataset_slug: ogbl-ddi
    - dataset: ogbl-ppa
      dataset_slug: ogbl-ppa
    - dataset: ogbl-citation2
      dataset_slug: ogbl-citation2
main_figure: /figures/2304.10074/main_figure.jpegoptim.jpg
---

