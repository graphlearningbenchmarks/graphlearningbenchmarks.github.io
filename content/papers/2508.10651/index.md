---
title: Graph Learning via Logic-Based Weisfeiler-Leman Variants and Tabularization
arxiv_id: '2508.10651'
source_url: ''
authors:
- name: Reijo Jaakkola
  orcid: null
  s2_author_id: '49285311'
  s2_url: null
- name: Tomi Janhunen
  orcid: null
  s2_author_id: '2273836389'
  s2_url: null
- name: Antti Kuusisto
  orcid: null
  s2_author_id: '2279335040'
  s2_url: null
- name: Magdalena Ortiz
  orcid: null
  s2_author_id: '2375138916'
  s2_url: null
- name: Matias Selin
  orcid: null
  s2_author_id: '2375903653'
  s2_url: null
- name: Mantas Šimkus
  orcid: null
  s2_author_id: '1685510'
  s2_url: null
published_date: Aug 14, 2025
published_date_iso: '2025-08-14'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: We present a novel approach for graph classification based on tabularizing
  graph data via new variants of the Weisfeiler–Leman algorithm and then applying
  methods for tabular data. The variants are obtained by modifying the underlying
  logical framework, and we establish a precise theoretical characterization of their
  expressive power using a novel generalization of the bisimulation game for generalized
  quantifiers. We then test our method on 14 datasets that span a range of application
  domains. The experiments demonstrate that on datasets with up to 40 000 samples,
  our approach generally matches the predictive performance of graph neural networks
  and graph transformers, without requiring a GPU or extensive hyperparameter tuning.
  Even when our method's tuning time is included and the baselines' is not, our method
  is 5--20 times faster. When tuning time is included for all methods, the gap is
  significantly greater in favour of our method.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Q-WL-RF
mrr: 0.0303
adjusted_mrr: 0.0202
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
    std: 0.003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.841
    std: 0.021
    paper_value: 0.841
    paper_std: 0.021
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
    input_feature_source: raw_features
    feature_source_evidence: Graph Neural Networks (GNNs) ... learn from both node
      features and graph topology.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.933
    at_pub_std: 0.029
    at_pub_source_arxiv: '2112.00911'
    at_pub_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.09200000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.09200000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 530
    rank_delta: 487
    rank_delta_abs: 487
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    comparison_source_arxiv: '2112.00911'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.817
    std: 0.021
    paper_value: 0.817
    paper_std: 0.021
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
    input_feature_source: raw_features
    feature_source_evidence: Graph Neural Networks (GNNs) ... learn from both node
      features and graph topology.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.922
    at_pub_std: 0.044
    at_pub_source_arxiv: '2503.01079'
    at_pub_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    at_pub_source_date_iso: '2025-03-03'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-03-03'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.1050000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.044
    value_gap_source_arxiv: '2503.01079'
    value_gap_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.1050000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.044
    global_rank: 71
    paper_rank: 636
    rank_delta: 565
    rank_delta_abs: 565
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    comparison_source_arxiv: '2503.01079'
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.83
    std: 0.019
    paper_value: 0.83
    paper_std: 0.019
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
    input_feature_source: raw_features
    feature_source_evidence: By running WL and counting the frequency of each resulting
      node label, we obtain a fixed-length feature vector for each graph, converting
      the graph dataset into a tabular dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1912.06058'
    at_pub_source_title: Coloring graph neural networks for node disambiguation
    at_pub_source_date_iso: '2019-12-12'
    at_pub_source_date_label: IJCAI 2019
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.07400000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.07400000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 171
    paper_rank: 573
    rank_delta: 402
    rank_delta_abs: 402
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
    value: 0.904
    std: 0.078
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12245'
    title: Asynchronous Neural Networks for Learning in Graphs
    date: May 24, 2022
    date_display: May 2022
    date_iso: '2022-05-24'
    venue: arXiv.org
    codebase_url: https://github.com/beabevi/ESAN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.904
    sort_std: 0.078
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.83
    std: 0.014
    paper_value: 0.83
    paper_std: 0.014
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
    input_feature_source: raw_features
    feature_source_evidence: Graph Neural Networks (GNNs) and Graph Transformers (GTs)
      achieve strong results on graph-structured data by learning from both node features
      and graph topology.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85
    at_pub_std: 0.0316
    at_pub_source_arxiv: '2406.00403'
    at_pub_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    at_pub_source_date_iso: '2024-06-01'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.85
    true_std: 0.0316
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.0316
    global_rank: 485
    paper_rank: 573
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Q-WL-RF
    model_key: q-wl-rf
    model_plain: Q-WL-RF
    value: 0.84
    std: 0.02
    paper_value: 0.84
    paper_std: 0.02
    metric: Accuracy
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
    feature_source_evidence: By running WL and counting the frequency of each resulting
      node label, we obtain a fixed-length feature vector for each graph, converting
      the graph dataset into a tabular dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.84
    true_std: 0.02
    value_gap_source_arxiv: '2508.10651'
    value_gap_source_title: Graph Learning via Logic-Based Weisfeiler-Leman Variants
      and Tabularization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: 0.02
    global_rank: 537
    paper_rank: 537
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.828
    std: 0.014
    paper_value: 0.828
    paper_std: 0.014
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Graph Neural Networks (GNNs) and Graph Transformers (GTs)
      achieve strong results on graph-structured data by learning from both node features
      and graph topology.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to mutag (score=83)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.828
    true_std: 0.014
    value_gap_source_arxiv: '2508.10651'
    value_gap_source_title: Graph Learning via Logic-Based Weisfeiler-Leman Variants
      and Tabularization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.828
    sort_std: 0.014
    global_rank: 587
    paper_rank: 587
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: NCI1
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.836
    std: 0.024
    paper_value: 0.836
    paper_std: 0.024
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9934
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15739999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9934
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.15739999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9934
    sort_std: null
    global_rank: 2
    paper_rank: 52
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.791
    std: 0.018
    paper_value: 0.791
    paper_std: 0.018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9727
    at_pub_std: null
    at_pub_source_arxiv: '2202.10156'
    at_pub_source_title: 1-WL Expressiveness Is (Almost) All You Need
    at_pub_source_date_iso: '2022-02-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.18169999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9727
    true_std: null
    value_gap_source_arxiv: '2202.10156'
    value_gap_source_title: 1-WL Expressiveness Is (Almost) All You Need
    value_gap_source_is_current_paper: false
    value_gap: 0.18169999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9727
    sort_std: null
    global_rank: 3
    paper_rank: 285
    rank_delta: 282
    rank_delta_abs: 282
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 1-WL Expressiveness Is (Almost) All You Need
    comparison_source_arxiv: '2202.10156'
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.855
    std: 0.015
    paper_value: 0.855
    paper_std: 0.015
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
    input_feature_source: raw_features
    feature_source_evidence: By running WL and counting the frequency of each resulting
      node label, we obtain a fixed-length feature vector for each graph, converting
      the graph dataset into a tabular dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.018
    at_pub_source_arxiv: '2205.14368'
    at_pub_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0050000000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0050000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 10
    paper_rank: 17
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Q-WL-RF
    model_key: q-wl-rf
    model_plain: Q-WL-RF
    value: 0.857
    std: 0.015
    paper_value: 0.857
    paper_std: 0.015
    metric: Accuracy
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
    feature_source_evidence: By running WL and counting the frequency of each resulting
      node label, we obtain a fixed-length feature vector for each graph, converting
      the graph dataset into a tabular dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.857
    true_std: 0.015
    value_gap_source_arxiv: '2508.10651'
    value_gap_source_title: Graph Learning via Logic-Based Weisfeiler-Leman Variants
      and Tabularization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.857
    sort_std: 0.015
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
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.825
    std: 0.015
    paper_value: 0.825
    paper_std: 0.015
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8421
    at_pub_std: 0.0225
    at_pub_source_arxiv: '2406.00403'
    at_pub_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    at_pub_source_date_iso: '2024-06-01'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.017100000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8421
    true_std: 0.0225
    value_gap_source_arxiv: '2406.00403'
    value_gap_source_title: Dual-perspective Cross Contrastive Learning in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.017100000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8421
    sort_std: 0.0225
    global_rank: 38
    paper_rank: 114
    rank_delta: 76
    rank_delta_abs: 76
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
    value: 0.8303
    std: 0.0137
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.01794'
    title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
      through In-depth Benchmarking'
    date: Oct 3, 2023
    date_display: Oct 2023
    date_iso: '2023-10-03'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Armagaan/gnn-x-bench
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 82
    sort_value: 0.8303
    sort_std: 0.0137
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.827
    std: 0.014
    paper_value: 0.827
    paper_std: 0.014
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Aug 14, 2025
    date_display: Aug 2025
    date_iso: '2025-08-14'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.827
    true_std: 0.014
    value_gap_source_arxiv: '2508.10651'
    value_gap_source_title: Graph Learning via Logic-Based Weisfeiler-Leman Variants
      and Tabularization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.827
    sort_std: 0.014
    global_rank: 107
    paper_rank: 107
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
single_proposed_model: Q-WL-RF
main_figure: /figures/2508.10651/main_figure.jpegoptim.jpg
---

