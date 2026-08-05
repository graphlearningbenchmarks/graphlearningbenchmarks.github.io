---
title: Link Prediction with Untrained Message Passing Layers
arxiv_id: '2406.16687'
source_url: ''
authors:
- name: Lisi Qarkaxhija
  orcid: null
  s2_author_id: '2185413546'
  s2_url: null
- name: Anatol E. Wegner
  orcid: null
  s2_author_id: '3216421'
  s2_url: null
- name: Ingo Scholtes
  orcid: null
  s2_author_id: '50790523'
  s2_url: null
published_date: Jun 24, 2024
published_date_iso: '2024-06-24'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: In this work, we explore the use of untrained message passing layers in
  graph neural networks for link prediction. The untrained message passing layers
  we consider are derived from widely used graph neural network architectures by removing
  trainable parameters and nonlinearities in their respective message passing layers.
  Experimentally, we find that untrained message passing layers can lead to competitive
  and even superior link prediction performance compared to fully trained message
  passing layers while being more efficient, especially in the presence of high-dimensional
  features. We also provide a theoretical analysis of untrained message passing layers
  in the context of link prediction and show that the inner product of features produced
  by untrained message passing layers relate to common neighbour and path-based topological
  measures which are widely used for link prediction. As such, untrained message passing
  layers offer a more efficient alternative to trained message passing layers in link
  prediction tasks, with clearer theoretical links to classical path-based heuristics.
codebase_url: ''
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
  - model: NCNC
    model_key: ncnc
    model_plain: NCNC
    value: 0.1961
    std: 0.0054
    paper_value: 0.1961
    paper_std: 0.0054
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8912
    at_pub_std: 0.004
    at_pub_source_arxiv: '2309.00976'
    at_pub_source_title: Pure Message Passing Can Estimate Common Neighbor for Link
      Prediction
    at_pub_source_date_iso: '2023-09-02'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-09-02'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.6951
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8912
    true_std: 0.004
    value_gap_source_arxiv: '2309.00976'
    value_gap_source_title: Pure Message Passing Can Estimate Common Neighbor for
      Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.6951
    has_value_note: false
    value_note: ''
    sort_value: 0.8912
    sort_std: 0.004
    global_rank: 5
    paper_rank: 73
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pure Message Passing Can Estimate Common Neighbor for
      Link Prediction
    comparison_source_arxiv: '2309.00976'
    is_best: false
    is_std_outlier: false
  - model: SEAL
    model_key: seal
    model_plain: SEAL
    value: 0.206
    std: 0.0128
    paper_value: 0.206
    paper_std: 0.0128
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.6707000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8767
    true_std: 0.0032
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.6707000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0032
    global_rank: 9
    paper_rank: 73
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.1917
    std: 0.002
    paper_value: 0.1917
    paper_std: 0.002
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.6839000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8756
    true_std: 0.0011
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.6839000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8756
    sort_std: 0.0011
    global_rank: 10
    paper_rank: 73
    rank_delta: 63
    rank_delta_abs: 63
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
    value: 0.1612
    std: 0.0025
    paper_value: 0.1612
    paper_std: 0.0025
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.7114
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8726
    true_std: 0.0084
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.7114
    has_value_note: false
    value_note: ''
    sort_value: 0.8726
    sort_std: 0.0084
    global_rank: 13
    paper_rank: 73
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    comparison_source_arxiv: '2206.04216'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.1998
    std: 0.0035
    paper_value: 0.1998
    paper_std: 0.0035
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.6481
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.6707000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8705
    sort_std: 0.0004
    global_rank: 14
    paper_rank: 73
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    comparison_source_arxiv: '2206.04216'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.2205
    std: 0.0012
    paper_value: 0.2205
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.826
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.6054999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.6162
    has_value_note: false
    value_note: ''
    sort_value: 0.8367
    sort_std: 0.0007
    global_rank: 29
    paper_rank: 73
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pairwise Learning for Neural Link Prediction
    comparison_source_arxiv: '2112.02936'
    is_best: false
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.1779
    std: null
    paper_value: 0.1779
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.34190000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.5825
    has_value_note: false
    value_note: ''
    sort_value: 0.7604
    sort_std: 0.0
    global_rank: 52
    paper_rank: 73
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    comparison_source_arxiv: '2209.15486'
    is_best: false
    is_std_outlier: false
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.1783
    std: null
    paper_value: 0.1783
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.3406
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.5813
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.0
    global_rank: 53
    paper_rank: 73
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.1711
    std: null
    paper_value: 0.1711
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.3436
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.5719
    has_value_note: false
    value_note: ''
    sort_value: 0.743
    sort_std: 0.0
    global_rank: 55
    paper_rank: 73
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.1467
    std: 0.0018
    paper_value: 0.1467
    paper_std: 0.0018
    metric: MRR
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6141
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2005.00687'
    at_pub_source_title: OGB
    at_pub_source_date_iso: '2020-05-02'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.4674
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6141
    true_std: 0.0011
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.4674
    has_value_note: false
    value_note: ''
    sort_value: 0.6141
    sort_std: 0.0011
    global_rank: 60
    paper_rank: 73
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: OGB
    comparison_source_arxiv: '2005.00687'
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.0872
    std: 0.026
    paper_value: 0.0872
    paper_std: 0.026
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.43139999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5186
    true_std: 0.0443
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.43139999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.5186
    sort_std: 0.0443
    global_rank: 63
    paper_rank: 73
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: true
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.1632
    std: 0.0007
    paper_value: 0.1632
    paper_std: 0.0007
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2906
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2010.16103'
    at_pub_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    at_pub_source_date_iso: '2020-10-30'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1274
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3917
    true_std: 0.0044
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.22849999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.3917
    sort_std: 0.0044
    global_rank: 71
    paper_rank: 73
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: NCN
    model_key: ncn
    model_plain: NCN
    value: 0.2335
    std: 0.0028
    paper_value: 0.2335
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8809
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2310.11009'
    at_pub_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.6474
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2335
    true_std: null
    value_gap_source_arxiv: '2506.24018'
    value_gap_source_title: Bridging Theory and Practice in Link Representation with
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2335
    sort_std: null
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    comparison_source_arxiv: '2310.11009'
    is_best: false
    is_std_outlier: false
  - model: NCNC + GCN
    model_key: ncnc + gcn
    model_plain: NCNC + GCN
    value: 0.2152
    std: 0.0071
    paper_value: 0.2152
    paper_std: 0.0071
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.2152
    sort_std: 0.0071
    global_rank: 74
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
  - model: NCNC + GIN
    model_key: ncnc + gin
    model_plain: NCNC + GIN
    value: 0.2136
    std: 0.0089
    paper_value: 0.2136
    paper_std: 0.0089
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.2136
    sort_std: 0.0089
    global_rank: 74
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
  - model: NCNC + SGCN
    model_key: ncnc + sgcn
    model_plain: NCNC + SGCN
    value: 0.2097
    std: 0.0086
    paper_value: 0.2097
    paper_std: 0.0086
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.2097
    sort_std: 0.0086
    global_rank: 74
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
  - model: NCNC + SAGE
    model_key: ncnc + sage
    model_plain: NCNC + SAGE
    value: 0.2055
    std: 0.0029
    paper_value: 0.2055
    paper_std: 0.0029
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.2055
    sort_std: 0.0029
    global_rank: 74
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
  - model: Katz
    model_key: katz
    model_plain: Katz
    value: 0.141
    std: null
    paper_value: 0.141
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.141
    sort_std: null
    global_rank: 74
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5558
    std: 0.0384
    paper_value: 0.5558
    paper_std: 0.0384
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.48956
    at_pub_std: 0.01143
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2024-09-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.06623999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6621
    true_std: 0.0033
    value_gap_source_arxiv: '2409.17475'
    value_gap_source_title: On the Impact of Feature Heterophily on Link Prediction
      with Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10630000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0033
    global_rank: 7
    paper_rank: 28
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
    is_best: false
    is_std_outlier: false
  - model: Neo-GNN
    model_key: neo-gnn
    model_plain: Neo-GNN
    value: 0.0523
    std: 0.009
    paper_value: 0.0523
    paper_std: 0.009
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5752
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.5229
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
    value_gap: 0.609
    has_value_note: false
    value_note: ''
    sort_value: 0.6613
    sort_std: 0.0061
    global_rank: 8
    paper_rank: 93
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    comparison_source_arxiv: '2206.04216'
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.0567
    std: 0.0036
    paper_value: 0.0567
    paper_std: 0.0036
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.6027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6594
    true_std: 0.0058
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.6027
    has_value_note: false
    value_note: ''
    sort_value: 0.6594
    sort_std: 0.0058
    global_rank: 12
    paper_rank: 93
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    comparison_source_arxiv: '2310.09516'
    is_best: false
    is_std_outlier: false
  - model: NCNC (GIN)
    model_key: ncnc (gin)
    model_plain: NCNC (GIN)
    value: 0.6587
    std: 0.0074
    paper_value: 0.6587
    paper_std: 0.0074
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.6587
    sort_std: 0.0074
    global_rank: 13
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
  - model: SNCNC (SGCN)
    model_key: sncnc (sgcn)
    model_plain: SNCNC (SGCN)
    value: 0.654
    std: 0.0046
    paper_value: 0.654
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.654
    sort_std: 0.0046
    global_rank: 14
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
    value: 0.0643
    std: 0.0032
    paper_value: 0.0643
    paper_std: 0.0032
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.5831
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6474
    true_std: 0.0043
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.5831
    has_value_note: false
    value_note: ''
    sort_value: 0.6474
    sort_std: 0.0043
    global_rank: 15
    paper_rank: 92
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.0507
    std: null
    paper_value: 0.0507
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.5928
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.5928
    has_value_note: false
    value_note: ''
    sort_value: 0.6435
    sort_std: 0.0
    global_rank: 18
    paper_rank: 93
    rank_delta: 75
    rank_delta_abs: 75
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    comparison_source_arxiv: '2310.09516'
    is_best: false
    is_std_outlier: false
  - model: RA
    model_key: ra
    model_plain: RA
    value: 0.0629
    std: null
    paper_value: 0.0629
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.5771000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.64
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.5771000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.64
    sort_std: 0.0
    global_rank: 20
    paper_rank: 92
    rank_delta: 72
    rank_delta_abs: 72
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
    value: 0.0509
    std: 0.0038
    paper_value: 0.0509
    paper_std: 0.0038
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.5967
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6386
    true_std: 0.0051
    value_gap_source_arxiv: '2410.01802'
    value_gap_source_title: 'PROXI: Challenging the GNNs for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.5876999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6386
    sort_std: 0.0051
    global_rank: 21
    paper_rank: 93
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    comparison_source_arxiv: '2310.11009'
    is_best: false
    is_std_outlier: false
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.042
    std: null
    paper_value: 0.042
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.5717
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
    value_gap: 0.5717
    has_value_note: false
    value_note: ''
    sort_value: 0.6137
    sort_std: 0.0
    global_rank: 22
    paper_rank: 93
    rank_delta: 71
    rank_delta_abs: 71
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
    value: 0.459
    std: 0.0867
    paper_value: 0.459
    paper_std: 0.0867
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5463
    at_pub_std: 0.0112
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.08729999999999999
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
    value_gap: 0.13540000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.5944
    sort_std: 0.0137
    global_rank: 23
    paper_rank: 72
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.0418
    std: 0.0033
    paper_value: 0.0418
    paper_std: 0.0033
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5643
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2303.00170'
    at_pub_source_title: Asymmetric Learning for Graph Neural Network based Link Prediction
    at_pub_source_date_iso: '2023-03-01'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.5225000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5643
    true_std: 0.0086
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.5225000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.5643
    sort_std: 0.0086
    global_rank: 27
    paper_rank: 93
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    comparison_source_arxiv: '2303.00170'
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.5413
    std: 0.0097
    paper_value: 0.5413
    paper_std: 0.0097
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5413
    sort_std: 0.0097
    global_rank: 35
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
  - model: SSAGE
    model_key: ssage
    model_plain: SSAGE
    value: 0.4992
    std: 0.0152
    paper_value: 0.4992
    paper_std: 0.0152
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.4992
    sort_std: 0.0152
    global_rank: 51
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
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.0468
    std: 0.0008
    paper_value: 0.0468
    paper_std: 0.0008
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4929
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2303.00170'
    at_pub_source_title: Asymmetric Learning for Graph Neural Network based Link Prediction
    at_pub_source_date_iso: '2023-03-01'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.4461
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4929
    true_std: 0.0064
    value_gap_source_arxiv: '2303.00170'
    value_gap_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.4461
    has_value_note: false
    value_note: ''
    sort_value: 0.4929
    sort_std: 0.0064
    global_rank: 55
    paper_rank: 93
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    comparison_source_arxiv: '2303.00170'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.0537
    std: 0.0014
    paper_value: 0.0537
    paper_std: 0.0014
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2035
    at_pub_std: 0.02168
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2025-04-08'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.1498
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4438
    true_std: 0.0347
    value_gap_source_arxiv: '2504.06193'
    value_gap_source_title: 'Weak Models Can be Good Teachers: A Case Study on Link
      Prediction with MLPs'
    value_gap_source_is_current_paper: false
    value_gap: 0.3901
    has_value_note: false
    value_note: ''
    sort_value: 0.4438
    sort_std: 0.0347
    global_rank: 77
    paper_rank: 93
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.0489
    std: 0.0025
    paper_value: 0.0489
    paper_std: 0.0025
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.3401
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.36920000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4181
    sort_std: 0.0167
    global_rank: 82
    paper_rank: 93
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: NCNC + SAGE
    model_key: ncnc + sage
    model_plain: NCNC + SAGE
    value: 0.1517
    std: 0.0215
    paper_value: 0.1517
    paper_std: 0.0215
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1517
    sort_std: 0.0215
    global_rank: 91
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
  - model: NCNC + GCN
    model_key: ncnc + gcn
    model_plain: NCNC + GCN
    value: 0.1399
    std: 0.0144
    paper_value: 0.1399
    paper_std: 0.0144
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1399
    sort_std: 0.0144
    global_rank: 91
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
  - model: NCNC + GIN
    model_key: ncnc + gin
    model_plain: NCNC + GIN
    value: 0.1128
    std: 0.0256
    paper_value: 0.1128
    paper_std: 0.0256
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1128
    sort_std: 0.0256
    global_rank: 92
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
  - model: NCNC + SGCN
    model_key: ncnc + sgcn
    model_plain: NCNC + SGCN
    value: 0.0672
    std: 0.0085
    paper_value: 0.0672
    paper_std: 0.0085
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0672
    sort_std: 0.0085
    global_rank: 93
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
  - model: Katz
    model_key: katz
    model_plain: Katz
    value: 0.0631
    std: null
    paper_value: 0.0631
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0631
    sort_std: null
    global_rank: 93
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
  - model: PEG
    model_key: peg
    model_plain: PEG
    value: 0.0483
    std: 0.0021
    paper_value: 0.0483
    paper_std: 0.0021
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0483
    sort_std: 0.0021
    global_rank: 94
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
  - model: Shortest Path
    model_key: shortest path
    model_plain: Shortest Path
    value: 0.0266
    std: null
    paper_value: 0.0266
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0266
    sort_std: null
    global_rank: 94
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
  - model: NTGCN + GAE
    model_key: ntgcn + gae
    model_plain: NTGCN + GAE
    value: 0.0066
    std: null
    paper_value: 0.0066
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0066
    sort_std: null
    global_rank: 94
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
  - model: NTSAGE + GAE
    model_key: ntsage + gae
    model_plain: NTSAGE + GAE
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 94
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
  - model: NTGIN + GAE
    model_key: ntgin + gae
    model_plain: NTGIN + GAE
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 94
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
  - model: NCN
    model_key: ncn
    model_plain: NCN
    value: 0.6582
    std: 0.0266
    paper_value: 0.6582
    paper_std: 0.0266
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-03'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8232
    true_std: 0.061
    value_gap_source_arxiv: '2411.01410'
    value_gap_source_title: PageRank Bandits for Link Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.16500000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8232
    sort_std: 0.061
    global_rank: 14
    paper_rank: 17
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BUDDY
    model_key: buddy
    model_plain: BUDDY
    value: 0.5871
    std: 0.0163
    paper_value: 0.5871
    paper_std: 0.0163
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.19800000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7851
    true_std: 0.0136
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.19800000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.7851
    sort_std: 0.0136
    global_rank: 16
    paper_rank: 21
    rank_delta: 5
    rank_delta_abs: 5
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
    value: 0.5194
    std: 0.1033
    paper_value: 0.5194
    paper_std: 0.1033
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.11630000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6357
    true_std: 0.0352
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.11630000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.6357
    sort_std: 0.0352
    global_rank: 18
    paper_rank: 26
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphConv + GAE
    model_key: graphconv + gae
    model_plain: GraphConv + GAE
    value: 0.5636
    std: 0.0045
    paper_value: 0.5636
    paper_std: 0.0045
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5636
    sort_std: 0.0045
    global_rank: 24
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
  - model: SNCNC (SGIN)
    model_key: sncnc (sgin)
    model_plain: SNCNC (SGIN)
    value: 0.5453
    std: 0.1102
    paper_value: 0.5453
    paper_std: 0.1102
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5453
    sort_std: 0.1102
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
  - model: GIN + GAE
    model_key: gin + gae
    model_plain: GIN + GAE
    value: 0.5421
    std: 0.0095
    paper_value: 0.5421
    paper_std: 0.0095
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5421
    sort_std: 0.0095
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.6719
    std: 0.0118
    paper_value: 0.6719
    paper_std: 0.0118
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.539
    at_pub_std: 0.0474
    at_pub_source_arxiv: '2112.02936'
    at_pub_source_title: Pairwise Learning for Neural Link Prediction
    at_pub_source_date_iso: '2021-12-06'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.13290000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.539
    true_std: 0.0474
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.13290000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.539
    sort_std: 0.0474
    global_rank: 26
    paper_rank: 18
    rank_delta: -8
    rank_delta_abs: 8
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Pairwise Learning for Neural Link Prediction
    comparison_source_arxiv: '2112.02936'
    is_best: false
    is_std_outlier: false
  - model: PEG
    model_key: peg
    model_plain: PEG
    value: 0.5012
    std: 0.0655
    paper_value: 0.5012
    paper_std: 0.0655
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5012
    sort_std: 0.0655
    global_rank: 28
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6476
    std: 0.0145
    paper_value: 0.6476
    paper_std: 0.0145
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.499
    at_pub_std: 0.0723
    at_pub_source_arxiv: '2310.00793'
    at_pub_source_title: 'Revisiting Link Prediction: a data perspective'
    at_pub_source_date_iso: '2023-10-01'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.14859999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.499
    true_std: 0.0723
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.14859999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.499
    sort_std: 0.0723
    global_rank: 28
    paper_rank: 18
    rank_delta: -10
    rank_delta_abs: 10
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Revisiting Link Prediction: a data perspective'
    comparison_source_arxiv: '2310.00793'
    is_best: false
    is_std_outlier: false
  - model: NCNC (GCN)
    model_key: ncnc (gcn)
    model_plain: NCNC (GCN)
    value: 0.4653
    std: 0.2924
    paper_value: 0.4653
    paper_std: 0.2924
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.4653
    sort_std: 0.2924
    global_rank: 31
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.1781
    std: 0.098
    paper_value: 0.1781
    paper_std: 0.098
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3707
    at_pub_std: 0.0507
    at_pub_source_arxiv: '2212.12488'
    at_pub_source_title: 'Bring Your Own View: Graph Neural Networks for Link Prediction
      with Personalized Subgraph Selection'
    at_pub_source_date_iso: '2022-12-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.19259999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3707
    true_std: 0.0507
    value_gap_source_arxiv: '2212.12488'
    value_gap_source_title: 'Bring Your Own View: Graph Neural Networks for Link Prediction
      with Personalized Subgraph Selection'
    value_gap_source_is_current_paper: false
    value_gap: 0.19259999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.3707
    sort_std: 0.0507
    global_rank: 33
    paper_rank: 53
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Bring Your Own View: Graph Neural Networks for Link
      Prediction with Personalized Subgraph Selection'
    comparison_source_arxiv: '2212.12488'
    is_best: false
    is_std_outlier: false
  - model: GCN + GAE
    model_key: gcn + gae
    model_plain: GCN + GAE
    value: 0.3448
    std: 0.0152
    paper_value: 0.3448
    paper_std: 0.0152
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.3448
    sort_std: 0.0152
    global_rank: 35
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
  - model: NTGCN + GAE
    model_key: ntgcn + gae
    model_plain: NTGCN + GAE
    value: 0.3323
    std: null
    paper_value: 0.3323
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.3323
    sort_std: null
    global_rank: 35
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
    value: 0.4974
    std: 0.0239
    paper_value: 0.4974
    paper_std: 0.0239
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.19180000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3056
    true_std: 0.0386
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.19180000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3056
    sort_std: 0.0386
    global_rank: 37
    paper_rank: 29
    rank_delta: -8
    rank_delta_abs: 8
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6683
    std: 0.0223
    paper_value: 0.6683
    paper_std: 0.0223
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2951
    at_pub_std: 0.064
    at_pub_source_arxiv: '2206.04216'
    at_pub_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.37320000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2951
    true_std: 0.064
    value_gap_source_arxiv: '2206.04216'
    value_gap_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.37320000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.2951
    sort_std: 0.064
    global_rank: 39
    paper_rank: 18
    rank_delta: -21
    rank_delta_abs: 21
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks
      for Link Prediction'
    comparison_source_arxiv: '2206.04216'
    is_best: false
    is_std_outlier: false
  - model: SAGE + GAE
    model_key: sage + gae
    model_plain: SAGE + GAE
    value: 0.293
    std: 0.0144
    paper_value: 0.293
    paper_std: 0.0144
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.293
    sort_std: 0.0144
    global_rank: 40
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
    value: 0.4401
    std: null
    paper_value: 0.4401
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.276
    at_pub_std: 0.0
    at_pub_source_arxiv: '2209.15486'
    at_pub_source_title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-10-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.16409999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.276
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.16409999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.276
    sort_std: 0.0
    global_rank: 41
    paper_rank: 31
    rank_delta: -10
    rank_delta_abs: 10
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Neural Networks for Link Prediction with Subgraph
      Sketching
    comparison_source_arxiv: '2209.15486'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.6363
    std: 0.0205
    paper_value: 0.6363
    paper_std: 0.0205
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.4033
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.233
    true_std: 0.021
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.4033
    has_value_note: false
    value_note: ''
    sort_value: 0.233
    sort_std: 0.021
    global_rank: 47
    paper_rank: 18
    rank_delta: -29
    rank_delta_abs: 29
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.2214
    std: 0.0338
    paper_value: 0.2214
    paper_std: 0.0338
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.2214
    sort_std: 0.0338
    global_rank: 50
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
  - model: SSAGE
    model_key: ssage
    model_plain: SSAGE
    value: 0.1944
    std: 0.1084
    paper_value: 0.1944
    paper_std: 0.1084
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1944
    sort_std: 0.1084
    global_rank: 51
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
  - model: AA
    model_key: aa
    model_plain: AA
    value: 0.3975
    std: null
    paper_value: 0.3975
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.21140000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1861
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.21140000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.1861
    sort_std: 0.0
    global_rank: 52
    paper_rank: 32
    rank_delta: -20
    rank_delta_abs: 20
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: SGCN + GAE
    model_key: sgcn + gae
    model_plain: SGCN + GAE
    value: 0.1821
    std: 0.1038
    paper_value: 0.1821
    paper_std: 0.1038
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1821
    sort_std: 0.1038
    global_rank: 53
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
  - model: CN
    model_key: cn
    model_plain: CN
    value: 0.3869
    std: null
    paper_value: 0.3869
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.2096
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1773
    true_std: 0.0
    value_gap_source_arxiv: '2310.09516'
    value_gap_source_title: Efficient Link Prediction via GNN Layers Induced by Negative
      Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.2096
    has_value_note: false
    value_note: ''
    sort_value: 0.1773
    sort_std: 0.0
    global_rank: 55
    paper_rank: 32
    rank_delta: -23
    rank_delta_abs: 23
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Labeling Trick: A Theory of Using Graph Neural Networks
      for Multi-Node Representation Learning'
    comparison_source_arxiv: '2010.16103'
    is_best: false
    is_std_outlier: false
  - model: Katz
    model_key: katz
    model_plain: Katz
    value: 0.3869
    std: null
    paper_value: 0.3869
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1773
    at_pub_std: null
    at_pub_source_arxiv: '2310.00793'
    at_pub_source_title: 'Revisiting Link Prediction: a data perspective'
    at_pub_source_date_iso: '2023-10-01'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.2096
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1773
    true_std: null
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.2096
    has_value_note: false
    value_note: ''
    sort_value: 0.1773
    sort_std: null
    global_rank: 57
    paper_rank: 32
    rank_delta: -25
    rank_delta_abs: 25
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Revisiting Link Prediction: a data perspective'
    comparison_source_arxiv: '2310.00793'
    is_best: false
    is_std_outlier: false
  - model: MF
    model_key: mf
    model_plain: MF
    value: 0.595
    std: 0.0168
    paper_value: 0.595
    paper_std: 0.0168
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    gap_vs_at_pub: 0.45799999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.137
    true_std: 0.047
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.45799999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.137
    sort_std: 0.047
    global_rank: 58
    paper_rank: 22
    rank_delta: -36
    rank_delta_abs: 36
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: SSAGE + GAE
    model_key: ssage + gae
    model_plain: SSAGE + GAE
    value: 0.1098
    std: 0.0076
    paper_value: 0.1098
    paper_std: 0.0076
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1098
    sort_std: 0.0076
    global_rank: 60
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
  - model: Shortest Path
    model_key: shortest path
    model_plain: Shortest Path
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 70
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
  - model: SGIN + GAE
    model_key: sgin + gae
    model_plain: SGIN + GAE
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 70
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
  - model: NTSAGE + GAE
    model_key: ntsage + gae
    model_plain: NTSAGE + GAE
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 70
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
  - model: NTGIN + GAE
    model_key: ntgin + gae
    model_plain: NTGIN + GAE
    value: 0.0
    std: null
    paper_value: 0.0
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0
    sort_std: null
    global_rank: 70
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
  - model: NCNC (GIN)
    model_key: ncnc (gin)
    model_plain: NCNC (GIN)
    value: 0.5947
    std: 0.016
    paper_value: 0.5947
    paper_std: 0.016
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.5947
    sort_std: 0.016
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.2388
    std: 0.0163
    paper_value: 0.2388
    paper_std: 0.0163
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5013
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2303.00170'
    at_pub_source_title: Asymmetric Learning for Graph Neural Network based Link Prediction
    at_pub_source_date_iso: '2023-03-01'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.26249999999999996
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
    value_gap: 0.26249999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.0055
    global_rank: 13
    paper_rank: 51
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Asymmetric Learning for Graph Neural Network based Link
      Prediction
    comparison_source_arxiv: '2303.00170'
    is_best: false
    is_std_outlier: false
  - model: SNCNC (SGCN)
    model_key: sncnc (sgcn)
    model_plain: SNCNC (SGCN)
    value: 0.4602
    std: 0.0119
    paper_value: 0.4602
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.4602
    sort_std: 0.0119
    global_rank: 22
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3084
    std: 0.0178
    paper_value: 0.3084
    paper_std: 0.0178
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2957
    at_pub_std: 0.029
    at_pub_source_arxiv: '2310.00793'
    at_pub_source_title: 'Revisiting Link Prediction: a data perspective'
    at_pub_source_date_iso: '2023-10-01'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.012699999999999989
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2957
    true_std: 0.029
    value_gap_source_arxiv: '2310.00793'
    value_gap_source_title: 'Revisiting Link Prediction: a data perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.012699999999999989
    has_value_note: false
    value_note: ''
    sort_value: 0.2957
    sort_std: 0.029
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.1234
    std: 0.0195
    paper_value: 0.1234
    paper_std: 0.0195
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.1234
    sort_std: 0.0195
    global_rank: 62
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
  - model: SSAGE
    model_key: ssage
    model_plain: SSAGE
    value: 0.0886
    std: 0.008
    paper_value: 0.0886
    paper_std: 0.008
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
    date: Jun 24, 2024
    date_display: Jun 2024
    date_iso: '2024-06-24'
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
    sort_value: 0.0886
    sort_std: 0.008
    global_rank: 64
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
main_figure: /figures/2406.16687/main_figure.jpegoptim.jpg
---

