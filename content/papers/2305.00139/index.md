---
title: Leveraging Label Non-Uniformity for Node Classification in Graph Neural Networks
arxiv_id: '2305.00139'
source_url: ''
authors:
- name: Feng Ji
  orcid: null
  s2_author_id: '2113422945'
  s2_url: null
- name: See Hian Lee
  orcid: null
  s2_author_id: '2107984162'
  s2_url: null
- name: Hanyang Meng
  orcid: null
  s2_author_id: '2215827170'
  s2_url: null
- name: Kai Zhao
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jielong Yang
  orcid: null
  s2_author_id: '18159894'
  s2_url: null
- name: Wee Peng Tay
  orcid: null
  s2_author_id: '3118058'
  s2_url: null
published_date: Apr 29, 2023
published_date_iso: '2023-04-29'
published_venue: ICML 2023
published_conference: ICML 2023
published_conference_short: ICML
published_conference_slug: icml
abstract: 'In node classification using graph neural networks (GNNs), a typical model
  generates logits for different class labels at each node. A softmax layer often
  outputs a label prediction based on the largest logit. We demonstrate that it is
  possible to infer hidden graph structural information from the dataset using these
  logits. We introduce the key notion of label non-uniformity, which is derived from
  the Wasserstein distance between the softmax distribution of the logits and the
  uniform distribution. We demonstrate that nodes with small label non-uniformity
  are harder to classify correctly. We theoretically analyze how the label non-uniformity
  varies across the graph, which provides insights into boosting the model performance:
  increasing training samples with high non-uniformity or dropping edges to reduce
  the maximal cut size of the node set of small non-uniformity. These mechanisms can
  be easily added to a base GNN model. Experimental results demonstrate that our approach
  improves the performance of many benchmark base models.'
codebase_url: http://github.com/amblee0306/label-non-uniformity-gnn
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- wGNN
- wGNN1
- wGNN2
mrr: 0.0037
adjusted_mrr: 0.0037
mrr_dataset_count: 4
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9036
    std: 0.0085
    paper_value: 0.9036
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.9294
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.025800000000000045
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
    value_gap: 0.06330000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 5
    paper_rank: 421
    rank_delta: 416
    rank_delta_abs: 416
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9066
    std: 0.0052
    paper_value: 0.9066
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.9309
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2106.05470'
    at_pub_source_title: Automated Self-Supervised Learning for Graphs
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02429999999999999
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
    value_gap: 0.056599999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 16
    paper_rank: 401
    rank_delta: 385
    rank_delta_abs: 385
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Automated Self-Supervised Learning for Graphs
    comparison_source_arxiv: '2106.05470'
    is_best: false
    is_std_outlier: false
  - model: simple multi-step model
    model_key: simple multi-step model
    model_plain: simple multi-step model
    value: 0.935
    std: 0.0028
    paper_value: 0.935
    paper_std: 0.0028
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.935
    true_std: 0.0028
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.0028
    global_rank: 168
    paper_rank: 168
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MaskGAE*
    model_key: maskgae
    model_plain: MaskGAE*
    value: 0.9155
    std: 0.0023
    paper_value: 0.9155
    paper_std: 0.0023
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9342
    true_std: 0.0026
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.01870000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.9342
    sort_std: 0.0026
    global_rank: 173
    paper_rank: 357
    rank_delta: 184
    rank_delta_abs: 184
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.9049
    std: 0.0064
    paper_value: 0.9049
    paper_std: 0.0064
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.9221
    at_pub_std: null
    at_pub_source_arxiv: '2012.03476'
    at_pub_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    at_pub_source_date_iso: '2020-12-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.017199999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9221
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.017199999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9221
    sort_std: null
    global_rank: 318
    paper_rank: 413
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    comparison_source_arxiv: '2012.03476'
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.9004
    std: 0.0054
    paper_value: 0.9004
    paper_std: 0.0054
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9004
    true_std: 0.0054
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: 0.0054
    global_rank: 432
    paper_rank: 432
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.896
    std: 0.013
    paper_value: 0.896
    paper_std: 0.013
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Photo dataset
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.896
    true_std: 0.013
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.896
    sort_std: 0.013
    global_rank: 441
    paper_rank: 441
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
- &id006
  dataset: Chameleon
  rows:
  - model: FE-GNN
    model_key: hetero-s (gat 8-layer)
    model_plain: FE-GNN
    value: 0.8693
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8693
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FE-GNN
    model_key: trans.conv+cna
    model_plain: FE-GNN
    value: 0.8586
    std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8586
    sort_std: 0.018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FE-GNN
    model_key: gat
    model_plain: FE-GNN
    value: 0.856
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.856
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: simple multi-step model
    model_key: simple multi-step model
    model_plain: simple multi-step model
    value: 0.6445
    std: 0.024
    paper_value: 0.6445
    paper_std: 0.024
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6445
    true_std: 0.024
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6445
    sort_std: 0.024
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN2
    model_key: wgnn2
    model_plain: wGNN2
    value: 0.6428
    std: 0.0194
    paper_value: 0.6428
    paper_std: 0.0194
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
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6428
    true_std: 0.0194
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6428
    sort_std: 0.0194
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Self-training
    model_key: self-training
    model_plain: Self-training
    value: 0.6397
    std: 0.0233
    paper_value: 0.6397
    paper_std: 0.0233
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6397
    true_std: 0.0233
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6397
    sort_std: 0.0233
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN1
    model_key: wgnn1
    model_plain: wGNN1
    value: 0.6395
    std: 0.0194
    paper_value: 0.6395
    paper_std: 0.0194
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
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6395
    true_std: 0.0194
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6395
    sort_std: 0.0194
    global_rank: 123
    paper_rank: 123
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.5298
    std: 0.0284
    paper_value: 0.5298
    paper_std: 0.0284
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5298
    true_std: 0.0284
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5298
    sort_std: 0.0284
    global_rank: 198
    paper_rank: 198
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PTDNet
    model_key: ptdnet
    model_plain: PTDNet
    value: 0.5035
    std: 0.0193
    paper_value: 0.5035
    paper_std: 0.0193
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Geom-GCN 10 fixed splits.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5035
    true_std: 0.0193
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5035
    sort_std: 0.0193
    global_rank: 215
    paper_rank: 215
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
  dataset: CiteSeer
  rows:
  - model: SGC+TSC
    model_key: cna
    model_plain: SGC+TSC
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: is-gib
    model_plain: SGC+TSC
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: eerm
    model_plain: SGC+TSC
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7123
    std: 0.0066
    paper_value: 0.7123
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.08199999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.16459999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 594
    rank_delta: 573
    rank_delta_abs: 573
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.7072
    std: 0.0056
    paper_value: 0.7072
    paper_std: 0.0056
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.813
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.1057999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.813
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1057999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.813
    sort_std: null
    global_rank: 35
    paper_rank: 640
    rank_delta: 605
    rank_delta_abs: 605
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7021
    std: 0.0052
    paper_value: 0.7021
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.8013
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.09920000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1059000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 673
    rank_delta: 627
    rank_delta_abs: 627
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: PTDNet
    model_key: ptdnet
    model_plain: PTDNet
    value: 0.727
    std: 0.018
    paper_value: 0.727
    paper_std: 0.018
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.784
    at_pub_std: null
    at_pub_source_arxiv: '2106.02892'
    at_pub_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    at_pub_source_date_iso: '2021-06-05'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-06-05'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.05700000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.784
    true_std: null
    value_gap_source_arxiv: '2106.02892'
    value_gap_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    value_gap_source_is_current_paper: false
    value_gap: 0.05700000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: null
    global_rank: 99
    paper_rank: 414
    rank_delta: 315
    rank_delta_abs: 315
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    comparison_source_arxiv: '2106.02892'
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.701
    std: 0.0137
    paper_value: 0.701
    paper_std: 0.0137
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-24'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.751
    true_std: 0.0007
    value_gap_source_arxiv: '2310.15523'
    value_gap_source_title: Generative and Contrastive Paradigms Are Complementary
      for Graph Self-Supervised Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.751
    sort_std: 0.0007
    global_rank: 217
    paper_rank: 678
    rank_delta: 461
    rank_delta_abs: 461
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN
    model_key: wgnn
    model_plain: wGNN
    value: 0.7395
    std: 0.0046
    paper_value: 0.7395
    paper_std: 0.0046
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7395
    true_std: 0.0046
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7395
    sort_std: 0.0046
    global_rank: 276
    paper_rank: 276
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN1
    model_key: wgnn1
    model_plain: wGNN1
    value: 0.7355
    std: 0.0046
    paper_value: 0.7355
    paper_std: 0.0046
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7355
    true_std: 0.0046
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7355
    sort_std: 0.0046
    global_rank: 314
    paper_rank: 314
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Self-training
    model_key: self-training
    model_plain: Self-training
    value: 0.7324
    std: 0.0044
    paper_value: 0.7324
    paper_std: 0.0044
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.7221
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2006.10141'
    at_pub_source_title: 'Self-supervised Learning on Graphs: Deep Insights and New
      Directions'
    at_pub_source_date_iso: '2020-06-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.010300000000000087
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7324
    true_std: 0.0044
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7324
    sort_std: 0.0044
    global_rank: 346
    paper_rank: 346
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Self-supervised Learning on Graphs: Deep Insights and
      New Directions'
    comparison_source_arxiv: '2006.10141'
    is_best: false
    is_std_outlier: false
  - model: wGNN2
    model_key: wgnn2
    model_plain: wGNN2
    value: 0.7198
    std: 0.0052
    paper_value: 0.7198
    paper_std: 0.0052
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7198
    true_std: 0.0052
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7198
    sort_std: 0.0052
    global_rank: 519
    paper_rank: 519
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.708
    std: 0.014
    paper_value: 0.708
    paper_std: 0.014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.708
    true_std: 0.014
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: 0.014
    global_rank: 637
    paper_rank: 637
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.6954
    std: 0.0079
    paper_value: 0.6954
    paper_std: 0.0079
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6954
    true_std: 0.0079
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6954
    sort_std: 0.0079
    global_rank: 696
    paper_rank: 696
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.6643
    std: 0.0156
    paper_value: 0.6643
    paper_std: 0.0156
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6643
    true_std: 0.0156
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6643
    sort_std: 0.0156
    global_rank: 795
    paper_rank: 795
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8065
    std: 0.0049
    paper_value: 0.8065
    paper_std: 0.0049
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.8733
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.06679999999999997
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
    value_gap: 0.09389999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 750
    rank_delta: 717
    rank_delta_abs: 717
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.81
    std: 0.0055
    paper_value: 0.81
    paper_std: 0.0055
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.89
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-08-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.07999999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.89
    true_std: null
    value_gap_source_arxiv: '2008.09864'
    value_gap_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: null
    global_rank: 70
    paper_rank: 735
    rank_delta: 665
    rank_delta_abs: 665
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8191
    std: 0.0048
    paper_value: 0.8191
    paper_std: 0.0048
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.06989999999999996
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
    value_gap: 0.0706
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: null
    global_rank: 72
    paper_rank: 655
    rank_delta: 583
    rank_delta_abs: 583
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: wGNN
    model_key: wgnn
    model_plain: wGNN
    value: 0.8523
    std: 0.0069
    paper_value: 0.8523
    paper_std: 0.0069
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8523
    true_std: 0.0069
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8523
    sort_std: 0.0069
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PTDNet
    model_key: ptdnet
    model_plain: PTDNet
    value: 0.828
    std: 0.026
    paper_value: 0.828
    paper_std: 0.026
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.844
    at_pub_std: 0.023
    at_pub_source_arxiv: '2011.07057'
    at_pub_source_title: 'Learning to Drop: Robust Graph Neural Network via Topological
      Denoising'
    at_pub_source_date_iso: '2020-11-13'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-13'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.844
    true_std: 0.023
    value_gap_source_arxiv: '2011.07057'
    value_gap_source_title: 'Learning to Drop: Robust Graph Neural Network via Topological
      Denoising'
    value_gap_source_is_current_paper: false
    value_gap: 0.016000000000000014
    has_value_note: false
    value_note: ''
    sort_value: 0.844
    sort_std: 0.023
    global_rank: 359
    paper_rank: 552
    rank_delta: 193
    rank_delta_abs: 193
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN1
    model_key: wgnn1
    model_plain: wGNN1
    value: 0.8288
    std: 0.0041
    paper_value: 0.8288
    paper_std: 0.0041
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8288
    true_std: 0.0041
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8288
    sort_std: 0.0041
    global_rank: 551
    paper_rank: 551
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.8236
    std: 0.0084
    paper_value: 0.8236
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8236
    true_std: 0.0084
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8236
    sort_std: 0.0084
    global_rank: 599
    paper_rank: 599
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Self-training
    model_key: self-training
    model_plain: Self-training
    value: 0.8227
    std: 0.0033
    paper_value: 0.8227
    paper_std: 0.0033
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8227
    true_std: 0.0033
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8227
    sort_std: 0.0033
    global_rank: 623
    paper_rank: 623
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.8203
    std: 0.0076
    paper_value: 0.8203
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8203
    true_std: 0.0076
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8203
    sort_std: 0.0076
    global_rank: 644
    paper_rank: 644
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.8128
    std: 0.0075
    paper_value: 0.8128
    paper_std: 0.0075
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8128
    true_std: 0.0075
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8128
    sort_std: 0.0075
    global_rank: 710
    paper_rank: 710
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN2
    model_key: wgnn2
    model_plain: wGNN2
    value: 0.811
    std: 0.0025
    paper_value: 0.811
    paper_std: 0.0025
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.0025
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.0025
    global_rank: 728
    paper_rank: 728
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.7965
    std: 0.0138
    paper_value: 0.7965
    paper_std: 0.0138
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7965
    true_std: 0.0138
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0138
    global_rank: 787
    paper_rank: 787
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7903
    std: 0.0038
    paper_value: 0.7903
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.10670000000000002
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
    value_gap: 0.13929999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: null
    global_rank: 21
    paper_rank: 609
    rank_delta: 588
    rank_delta_abs: 588
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7891
    std: 0.0042
    paper_value: 0.7891
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: 0.1079
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
    value_gap: 0.13419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: null
    global_rank: 23
    paper_rank: 627
    rank_delta: 604
    rank_delta_abs: 604
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.7918
    std: 0.0033
    paper_value: 0.7918
    paper_std: 0.0033
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.909
    at_pub_std: null
    at_pub_source_arxiv: '2106.02892'
    at_pub_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    at_pub_source_date_iso: '2021-06-05'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-06-05'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.11720000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.909
    true_std: null
    value_gap_source_arxiv: '2106.02892'
    value_gap_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    value_gap_source_is_current_paper: false
    value_gap: 0.11720000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.909
    sort_std: null
    global_rank: 47
    paper_rank: 594
    rank_delta: 547
    rank_delta_abs: 547
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    comparison_source_arxiv: '2106.02892'
    is_best: false
    is_std_outlier: false
  - model: MaskGAE
    model_key: maskgae
    model_plain: MaskGAE
    value: 0.8011
    std: 0.0051
    paper_value: 0.8011
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8748
    true_std: 0.002
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.07369999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8748
    sort_std: 0.002
    global_rank: 212
    paper_rank: 461
    rank_delta: 249
    rank_delta_abs: 249
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PTDNet
    model_key: ptdnet
    model_plain: PTDNet
    value: 0.798
    std: 0.024
    paper_value: 0.798
    paper_std: 0.024
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.854
    at_pub_std: null
    at_pub_source_arxiv: '2106.02892'
    at_pub_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    at_pub_source_date_iso: '2021-06-05'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-06-05'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.05599999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.854
    true_std: null
    value_gap_source_arxiv: '2106.02892'
    value_gap_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    value_gap_source_is_current_paper: false
    value_gap: 0.05599999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.854
    sort_std: null
    global_rank: 264
    paper_rank: 496
    rank_delta: 232
    rank_delta_abs: 232
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Training Robust Graph Neural Networks with Topology Adaptive
      Edge Dropping
    comparison_source_arxiv: '2106.02892'
    is_best: false
    is_std_outlier: false
  - model: simple multi-step model
    model_key: simple multi-step model
    model_plain: simple multi-step model
    value: 0.8178
    std: 0.0022
    paper_value: 0.8178
    paper_std: 0.0022
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8178
    true_std: 0.0022
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8178
    sort_std: 0.0022
    global_rank: 354
    paper_rank: 354
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Self-training
    model_key: self-training
    model_plain: Self-training
    value: 0.8032
    std: 0.0018
    paper_value: 0.8032
    paper_std: 0.0018
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.7935
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2006.10141'
    at_pub_source_title: 'Self-supervised Learning on Graphs: Deep Insights and New
      Directions'
    at_pub_source_date_iso: '2020-06-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.009700000000000042
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8032
    true_std: 0.0018
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8032
    sort_std: 0.0018
    global_rank: 441
    paper_rank: 441
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Self-supervised Learning on Graphs: Deep Insights and
      New Directions'
    comparison_source_arxiv: '2006.10141'
    is_best: false
    is_std_outlier: false
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.7962
    std: 0.0038
    paper_value: 0.7962
    paper_std: 0.0038
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7962
    true_std: 0.0038
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7962
    sort_std: 0.0038
    global_rank: 509
    paper_rank: 509
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.7911
    std: 0.0178
    paper_value: 0.7911
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7911
    true_std: 0.0178
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7911
    sort_std: 0.0178
    global_rank: 598
    paper_rank: 598
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIL
    model_key: gil
    model_plain: GIL
    value: 0.7718
    std: 0.01
    paper_value: 0.7718
    paper_std: 0.01
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7718
    true_std: 0.01
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7718
    sort_std: 0.01
    global_rank: 761
    paper_rank: 761
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
- &id005
  dataset: Texas
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
    value: 0.9672
    std: 0.0147
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: gpf-plus
    model_plain: R-SoftGraphAIN
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: simple multi-step model
    model_key: simple multi-step model
    model_plain: simple multi-step model
    value: 0.5811
    std: 0.0972
    paper_value: 0.5811
    paper_std: 0.0972
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Texas node classification.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5811
    true_std: 0.0972
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5811
    sort_std: 0.0972
    global_rank: 566
    paper_rank: 566
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.5811
    std: 0.0472
    paper_value: 0.5811
    paper_std: 0.0472
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
    source_ref: Che21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Texas node classification.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5811
    true_std: 0.0472
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5811
    sort_std: 0.0472
    global_rank: 567
    paper_rank: 567
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: wGNN1
    model_key: wgnn1
    model_plain: wGNN1
    value: 0.5541
    std: 0.0735
    paper_value: 0.5541
    paper_std: 0.0735
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
    protocol_note: Standard split for Texas node classification.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5541
    true_std: 0.0735
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5541
    sort_std: 0.0735
    global_rank: 595
    paper_rank: 595
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Self-training
    model_key: self-training
    model_plain: Self-training
    value: 0.5414
    std: 0.0745
    paper_value: 0.5414
    paper_std: 0.0745
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
    source_ref: Liq18
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for Texas node classification.
    date: Apr 29, 2023
    date_display: Apr 2023
    date_iso: '2023-04-29'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-29'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5414
    true_std: 0.0745
    value_gap_source_arxiv: '2305.00139'
    value_gap_source_title: Leveraging Label Non-Uniformity for Node Classification
      in Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5414
    sort_std: 0.0745
    global_rank: 605
    paper_rank: 605
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
- benchmark: Heterophilic Graphs
  datasets:
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Chameleon
      dataset_slug: chameleon
main_figure: /figures/2305.00139/main_figure.jpegoptim.jpg
---

