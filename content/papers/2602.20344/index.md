---
title: Hierarchical Molecular Representation Learning via Fragment-Based Self-Supervised
  Embedding Prediction
arxiv_id: '2602.20344'
source_url: ''
authors:
- name: Jiele Wu
  orcid: null
  s2_author_id: '2367821910'
  s2_url: null
- name: Haozhe Ma
  orcid: null
  s2_author_id: '2218208338'
  s2_url: null
- name: Zhihan Guo
  orcid: null
  s2_author_id: '2387739748'
  s2_url: null
- name: Thanh Vinh Vo
  orcid: null
  s2_author_id: '51056329'
  s2_url: null
- name: Tze-Yun Leong
  orcid: null
  s2_author_id: '2298470929'
  s2_url: null
published_date: Feb 23, 2026
published_date_iso: '2026-02-23'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph self-supervised learning (GSSL) has demonstrated strong potential
  for generating expressive graph embeddings without the need for human annotations,
  making it particularly valuable in domains with high labeling costs such as molecular
  graph analysis. However, existing GSSL methods mostly focus on node- or edge-level
  information, often ignoring chemically relevant substructures which strongly influence
  molecular properties. In this work, we propose Graph Semantic Predictive Network
  (GraSPNet), a hierarchical self-supervised framework that explicitly models both
  atomic-level and fragment-level semantics. GraSPNet decomposes molecular graphs
  into chemically meaningful fragments without predefined vocabularies and learns
  node- and fragment-level representations through multi-level message passing with
  masked semantic prediction at both levels. This hierarchical semantic supervision
  enables GraSPNet to learn multi-resolution structural information that is both expressive
  and transferable. Extensive experiments on multiple molecular property prediction
  benchmarks demonstrate that GraSPNet learns chemically meaningful representations
  and consistently outperforms state-of-the-art GSSL methods in transfer learning
  settings.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraSPNet
mrr: 0.022
adjusted_mrr: 0.022
mrr_dataset_count: 3
benchmark_categories:
- MoleculeNet
benchmark_coverage:
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 3
  total: 9
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ESOL
  rows:
  - model: 10% ZINC + 10% PubChem
    model_key: 10% zinc + 10% pubchem
    model_plain: 10% ZINC + 10% PubChem
    value: 0.2775
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.2775
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MAT
    model_key: mat
    model_plain: MAT
    value: 0.278
    std: 0.02
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2002.08264'
    title: Molecule Attention Transformer
    date: Feb 19, 2020
    date_display: Feb 2020
    date_iso: '2020-02-19'
    venue: Graph Representation Learning workshop and Machine Learning and the Physical
      Sciences workshop at NeurIPS 2019
    codebase_url: https://github.com/gmum/MAT
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.278
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.2787
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2787
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.564
    std: 0.015
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.13987'
    title: On Structural Expressive Power of Graph Transformers
    date: May 23, 2023
    date_display: May 2023
    date_iso: '2023-05-23'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 13
    sort_value: 0.564
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimSGT
    model_key: simsgt
    model_plain: SimSGT
    value: 1.213
    std: 0.032
    paper_value: 1.213
    paper_std: 0.032
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.932
    at_pub_std: 0.026
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.281
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.932
    true_std: 0.026
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.281
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.026
    global_rank: 80
    paper_rank: 121
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    comparison_source_arxiv: '2412.15589'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 1.39
    std: 0.363
    paper_value: 1.39
    paper_std: 0.363
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.959
    at_pub_std: 0.047
    at_pub_source_arxiv: '2110.04126'
    at_pub_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    at_pub_source_date_iso: '2021-10-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.43099999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.959
    true_std: 0.047
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.43099999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.047
    global_rank: 85
    paper_rank: 130
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 3D Infomax improves GNNs for Molecular Property Prediction
    comparison_source_arxiv: '2110.04126'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 1.978
    std: 0.029
    paper_value: 1.978
    paper_std: 0.029
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.12
    at_pub_std: 0.019
    at_pub_source_arxiv: '2110.07728'
    at_pub_source_title: 16 Pre-training Molecular Graph Representation with 3D Geometry
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.8579999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.12
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.8579999999999999
    has_value_note: false
    value_note: ''
    sort_value: 1.12
    sort_std: null
    global_rank: 112
    paper_rank: 147
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 16 Pre-training Molecular Graph Representation with 3D
      Geometry
    comparison_source_arxiv: '2110.07728'
    is_best: false
    is_std_outlier: false
  - model: GraSPNet
    model_key: graspnet
    model_plain: GraSPNet
    value: 1.161
    std: 0.037
    paper_value: 1.161
    paper_std: 0.037
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.161
    true_std: 0.037
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.161
    sort_std: 0.037
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGSSL
    model_key: mgssl
    model_plain: MGSSL
    value: 2.936
    std: 0.071
    paper_value: 2.936
    paper_std: 0.071
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.179
    at_pub_std: 0.008
    at_pub_source_arxiv: '2310.07351'
    at_pub_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 1.757
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.179
    true_std: 0.008
    value_gap_source_arxiv: '2310.07351'
    value_gap_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    value_gap_source_is_current_paper: false
    value_gap: 1.757
    has_value_note: false
    value_note: ''
    sort_value: 1.179
    sort_std: 0.008
    global_rank: 119
    paper_rank: 155
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Atom-Motif Contrastive Transformer for Molecular Property
      Prediction
    comparison_source_arxiv: '2310.07351'
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 2.19
    std: 0.026
    paper_value: 2.19
    paper_std: 0.026
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.196
    at_pub_std: 0.037
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.196
    true_std: 0.037
    value_gap_source_arxiv: '2209.15101'
    value_gap_source_title: Improving Molecular Pretraining with Complementary Featurizations
    value_gap_source_is_current_paper: false
    value_gap: 0.994
    has_value_note: false
    value_note: ''
    sort_value: 1.196
    sort_std: 0.037
    global_rank: 120
    paper_rank: 151
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: GROVE
    model_key: grove
    model_plain: GROVE
    value: 1.237
    std: 0.403
    paper_value: 1.237
    paper_std: 0.403
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.237
    at_pub_std: 0.403
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.237
    true_std: 0.403
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.237
    sort_std: 0.403
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GraphFP
    model_key: graphfp
    model_plain: GraphFP
    value: 2.136
    std: 0.096
    paper_value: 2.136
    paper_std: 0.096
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.136
    at_pub_std: 0.096
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-04-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 1.935
    true_std: null
    value_gap_source_arxiv: '2604.06336'
    value_gap_source_title: 'BiScale-GTR: Fragment-Aware Graph Transformers for Multi-Scale
      Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.20100000000000007
    has_value_note: false
    value_note: ''
    sort_value: 1.935
    sort_std: null
    global_rank: 146
    paper_rank: 150
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePred
    model_key: edgepred
    model_plain: EdgePred
    value: 2.368
    std: 0.07
    paper_value: 2.368
    paper_std: 0.07
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.368
    at_pub_std: 0.07
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.368
    true_std: 0.07
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.368
    sort_std: 0.07
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 2.953
    std: 0.049
    paper_value: 2.953
    paper_std: 0.049
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.953
    at_pub_std: 0.049
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.953
    true_std: 0.049
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.953
    sort_std: 0.049
    global_rank: 156
    paper_rank: 156
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 2.954
    std: 0.087
    paper_value: 2.954
    paper_std: 0.087
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.954
    at_pub_std: 0.087
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.954
    true_std: 0.087
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.954
    sort_std: 0.087
    global_rank: 157
    paper_rank: 157
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: FreeSolv
  rows:
  - model: 10% ZINC + 10% PubChem
    model_key: 10% zinc + 10% pubchem
    model_plain: 10% ZINC + 10% PubChem
    value: 0.205
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.205
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.2308
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.2308
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoLFormer-Base
    model_key: molformer-base
    model_plain: MoLFormer-Base
    value: 0.2596
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2596
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraSPNet
    model_key: graspnet
    model_plain: GraSPNet
    value: 1.232
    std: 0.05
    paper_value: 1.232
    paper_std: 0.05
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.232
    true_std: 0.05
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.232
    sort_std: 0.05
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
  - model: SimSGT
    model_key: simsgt
    model_plain: SimSGT
    value: 1.953
    std: 0.038
    paper_value: 1.953
    paper_std: 0.038
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.953
    at_pub_std: 0.038
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.953
    true_std: 0.038
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.953
    sort_std: 0.038
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 2.346
    std: 0.122
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_display: Jun 2021
    date_iso: '2021-06-11'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 73
    sort_value: 2.346
    sort_std: 0.122
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphFP
    model_key: graphfp
    model_plain: GraphFP
    value: 2.528
    std: 0.016
    paper_value: 2.528
    paper_std: 0.016
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.528
    at_pub_std: 0.016
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.528
    true_std: 0.016
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.528
    sort_std: 0.016
    global_rank: 79
    paper_rank: 79
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GROVE
    model_key: grove
    model_plain: GROVE
    value: 2.712
    std: 0.327
    paper_value: 2.712
    paper_std: 0.327
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.712
    at_pub_std: 0.327
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.712
    true_std: 0.327
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.712
    sort_std: 0.327
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGSSL
    model_key: mgssl
    model_plain: MGSSL
    value: 2.94
    std: 0.051
    paper_value: 2.94
    paper_std: 0.051
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.84
    at_pub_std: 0.19
    at_pub_source_arxiv: '2309.04589'
    at_pub_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    at_pub_source_date_iso: '2023-09-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 2.84
    true_std: 0.19
    value_gap_source_arxiv: '2309.04589'
    value_gap_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    value_gap_source_is_current_paper: false
    value_gap: 0.10000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 2.84
    sort_std: 0.19
    global_rank: 94
    paper_rank: 98
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 3.033
    std: 0.026
    paper_value: 3.033
    paper_std: 0.026
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.033
    at_pub_std: 0.026
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.033
    true_std: 0.026
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.033
    sort_std: 0.026
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 3.195
    std: 0.058
    paper_value: 3.195
    paper_std: 0.058
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.057
    at_pub_std: 0.17
    at_pub_source_arxiv: '2309.04589'
    at_pub_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    at_pub_source_date_iso: '2023-09-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.1379999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 3.057
    true_std: 0.17
    value_gap_source_arxiv: '2309.04589'
    value_gap_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    value_gap_source_is_current_paper: false
    value_gap: 0.1379999999999999
    has_value_note: false
    value_note: ''
    sort_value: 3.057
    sort_std: 0.17
    global_rank: 102
    paper_rank: 106
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 3.166
    std: 0.027
    paper_value: 3.166
    paper_std: 0.027
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.166
    at_pub_std: 0.027
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.166
    true_std: 0.027
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.166
    sort_std: 0.027
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePred
    model_key: edgepred
    model_plain: EdgePred
    value: 3.192
    std: 0.023
    paper_value: 3.192
    paper_std: 0.023
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.192
    at_pub_std: 0.023
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.192
    true_std: 0.023
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.192
    sort_std: 0.023
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 3.282
    std: 0.002
    paper_value: 3.282
    paper_std: 0.002
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 3.282
    at_pub_std: 0.002
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 3.282
    true_std: 0.002
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 3.282
    sort_std: 0.002
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 4.023
    std: 0.039
    paper_value: 4.023
    paper_std: 0.039
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 4.023
    at_pub_std: 0.039
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 4.023
    true_std: 0.039
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 4.023
    sort_std: 0.039
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: Lipophilicity
  rows:
  - model: MoLFormer-XL
    model_key: molformer-xl
    model_plain: MoLFormer-XL
    value: 0.5289
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.5289
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: 10% ZINC + 10% PubChem
    model_key: 10% zinc + 10% pubchem
    model_plain: 10% ZINC + 10% PubChem
    value: 0.5331
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.5331
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GeomGCL
    model_key: geomgcl
    model_plain: GeomGCL
    value: 0.541
    std: null
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_display: Jun 2021
    date_iso: '2021-06-17'
    venue: Nature Machine Intelligence
    codebase_url: https://github.com/IBM/molformer
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.541
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.655
    std: 0.036
    metric: RMSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 13
    sort_value: 0.655
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ContextPred
    model_key: contextpred
    model_plain: ContextPred
    value: 1.053
    std: 0.048
    paper_value: 1.053
    paper_std: 0.048
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.702
    at_pub_std: 0.02
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.351
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.702
    true_std: 0.02
    value_gap_source_arxiv: '2209.15101'
    value_gap_source_title: Improving Molecular Pretraining with Complementary Featurizations
    value_gap_source_is_current_paper: false
    value_gap: 0.351
    has_value_note: false
    value_note: ''
    sort_value: 0.702
    sort_std: 0.02
    global_rank: 23
    paper_rank: 96
    rank_delta: 73
    rank_delta_abs: 73
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: JOAO
    model_key: joao
    model_plain: JOAO
    value: 1.093
    std: 0.097
    paper_value: 1.093
    paper_std: 0.097
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.708
    at_pub_std: 0.007
    at_pub_source_arxiv: '2209.15101'
    at_pub_source_title: Improving Molecular Pretraining with Complementary Featurizations
    at_pub_source_date_iso: '2022-09-29'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-05-01'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.385
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.708
    true_std: null
    value_gap_source_arxiv: '2305.13315'
    value_gap_source_title: 3D Molecular Geometry Analysis with 2D Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.385
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: null
    global_rank: 27
    paper_rank: 97
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Molecular Pretraining with Complementary Featurizations
    comparison_source_arxiv: '2209.15101'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 1.014
    std: 0.018
    paper_value: 1.014
    paper_std: 0.018
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.714
    at_pub_std: 0.011
    at_pub_source_arxiv: '2312.07633'
    at_pub_source_title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    at_pub_source_date_iso: '2023-12-12'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-12-12'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.30000000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.714
    true_std: 0.011
    value_gap_source_arxiv: '2312.07633'
    value_gap_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.30000000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.011
    global_rank: 30
    paper_rank: 94
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: SE(3)-Invariant Multiparameter Persistent Homology for
      Chiral-Sensitive Molecular Property Prediction
    comparison_source_arxiv: '2312.07633'
    is_best: false
    is_std_outlier: false
  - model: SimSGT
    model_key: simsgt
    model_plain: SimSGT
    value: 0.835
    std: 0.037
    paper_value: 0.835
    paper_std: 0.037
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.771
    at_pub_std: 0.041
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.06399999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.771
    true_std: 0.041
    value_gap_source_arxiv: '2412.15589'
    value_gap_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.06399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.771
    sort_std: 0.041
    global_rank: 52
    paper_rank: 69
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraSPNet
    model_key: graspnet
    model_plain: GraSPNet
    value: 0.813
    std: 0.052
    paper_value: 0.813
    paper_std: 0.052
    metric: RMSE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.813
    true_std: 0.052
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.813
    sort_std: 0.052
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GROVE
    model_key: grove
    model_plain: GROVE
    value: 0.823
    std: 0.027
    paper_value: 0.823
    paper_std: 0.027
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.823
    at_pub_std: 0.027
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.823
    true_std: 0.027
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.823
    sort_std: 0.027
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
  - model: MGSSL
    model_key: mgssl
    model_plain: MGSSL
    value: 1.106
    std: 0.077
    paper_value: 1.106
    paper_std: 0.077
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.869
    at_pub_std: 0.06
    at_pub_source_arxiv: '2309.04589'
    at_pub_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    at_pub_source_date_iso: '2023-09-08'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2370000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.06
    value_gap_source_arxiv: '2309.04589'
    value_gap_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    value_gap_source_is_current_paper: false
    value_gap: 0.2370000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.06
    global_rank: 77
    paper_rank: 97
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Motif-aware Attribute Masking for Molecular Graph Pre-training
    comparison_source_arxiv: '2309.04589'
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.97
    std: 0.023
    paper_value: 0.97
    paper_std: 0.023
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.97
    at_pub_std: 0.023
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.97
    true_std: 0.023
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.97
    sort_std: 0.023
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AttrMasking
    model_key: attrmasking
    model_plain: AttrMasking
    value: 0.982
    std: 0.052
    paper_value: 0.982
    paper_std: 0.052
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.982
    at_pub_std: 0.052
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.982
    true_std: 0.052
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.982
    sort_std: 0.052
    global_rank: 92
    paper_rank: 92
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePred
    model_key: edgepred
    model_plain: EdgePred
    value: 1.085
    std: 0.061
    paper_value: 1.085
    paper_std: 0.061
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.085
    at_pub_std: 0.061
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.085
    true_std: 0.061
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.085
    sort_std: 0.061
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphFP
    model_key: graphfp
    model_plain: GraphFP
    value: 1.371
    std: 0.058
    paper_value: 1.371
    paper_std: 0.058
    metric: RMSE
    higher_is_better: false
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
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.371
    at_pub_std: 0.058
    at_pub_source_arxiv: '2412.15589'
    at_pub_source_title: Pre-training Graph Neural Networks on Molecules by Using
      Subgraph-Conditioned Graph Information Bottleneck
    at_pub_source_date_iso: '2024-12-20'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2026-02-23'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.371
    true_std: 0.058
    value_gap_source_arxiv: '2602.20344'
    value_gap_source_title: Hierarchical Molecular Representation Learning via Fragment-Based
      Self-Supervised Embedding Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.371
    sort_std: 0.058
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: RMSE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: RMSE
  paper_metrics:
  - RMSE
  metric: RMSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: MoleculeNet
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: ESOL
      dataset_slug: esol
    - dataset: FreeSolv
      dataset_slug: freesolv
    - dataset: Lipophilicity
      dataset_slug: lipophilicity
single_proposed_model: GraSPNet
main_figure: /figures/2602.20344/main_figure.jpegoptim.jpg
---

