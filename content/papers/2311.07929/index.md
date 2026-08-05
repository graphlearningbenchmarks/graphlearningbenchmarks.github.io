---
title: Variational Graph Autoencoder for Heterogeneous Information Networks with Missing
  and Inaccurate Attributes
arxiv_id: '2311.07929'
source_url: ''
authors:
- name: Yige Zhao
  orcid: null
  s2_author_id: '2266749154'
  s2_url: null
- name: Jianxiang Yu
  orcid: null
  s2_author_id: '2198507600'
  s2_url: null
- name: Yao Cheng
  orcid: null
  s2_author_id: '2165643958'
  s2_url: null
- name: Chengcheng Yu
  orcid: null
  s2_author_id: '2218698582'
  s2_url: null
- name: Yiding Liu
  orcid: null
  s2_author_id: '2249554788'
  s2_url: null
- name: Xiang Li
  orcid: null
  s2_author_id: '2258789569'
  s2_url: null
- name: Shuaiqiang Wang
  orcid: null
  s2_author_id: '2237948548'
  s2_url: null
published_date: Nov 14, 2023
published_date_iso: '2023-11-14'
published_venue: KDD 2023
published_conference: KDD 2023
published_conference_short: KDD
published_conference_slug: kdd
abstract: Heterogeneous Information Networks (HINs), which consist of various types
  of nodes and edges, have recently witnessed excellent performance in graph mining.
  However, most existing heterogeneous graph neural networks (HGNNs) fail to simultaneously
  handle the problems of missing attributes, inaccurate attributes and scarce node
  labels, which limits their expressiveness. In this paper, we propose a generative
  self-supervised model GraMI\ to address these issues simultaneously. Specifically,
  GraMI\ first initializes all the nodes in the graph with a low-dimensional representation
  matrix. After that, based on the variational graph autoencoder framework, GraMI\
  learns both node-level and attribute-level embeddings in the encoder, which can
  provide fine-grained semantic information to construct node attributes. In the decoder,
  GraMI\ reconstructs both links and attributes. Instead of directly reconstructing
  raw features for attributed nodes, GraMI\ generates the initial low-dimensional
  representation matrix for all the nodes, based on which raw features of attributed
  nodes are further reconstructed. In this way, GraMI\ can not only complete informative
  features for non-attributed nodes, but rectify inaccurate ones for attributed nodes.
  Finally, we conduct extensive experiments to show the superiority of GraMI\ in tackling
  HINs with missing and inaccurate attributes. Our code and data can be found here:.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraMI
mrr: 0.0625
adjusted_mrr: 0.0208
mrr_dataset_count: 1
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: DBLP
  rows:
  - model: HERec
    model_key: herec
    model_plain: HERec
    value: 0.9993
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9993
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.9972
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9972
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.9941
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9941
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraMI
    model_key: grami
    model_plain: GraMI
    value: 0.9503
    std: null
    paper_value: 0.9503
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9503
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9503
    sort_std: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.946
    std: 0.0031
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_display: Oct 2023
    date_iso: '2023-10-25'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 29
    sort_value: 0.946
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9357
    std: null
    paper_value: 0.9357
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9456
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-18'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00990000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9456
    true_std: null
    value_gap_source_arxiv: '2012.10024'
    value_gap_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9456
    sort_std: null
    global_rank: 30
    paper_rank: 49
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8351
    std: null
    paper_value: 0.8351
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9448
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2310.16401'
    at_pub_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.10970000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9448
    true_std: 0.0022
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.10970000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0022
    global_rank: 31
    paper_rank: 121
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    comparison_source_arxiv: '2310.16401'
    is_best: false
    is_std_outlier: false
  - model: HGCA
    model_key: hgca
    model_plain: HGCA
    value: 0.9434
    std: null
    paper_value: 0.9434
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9434
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9434
    sort_std: null
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
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9369
    std: null
    paper_value: 0.9369
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9327
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0041999999999999815
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9369
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9369
    sort_std: null
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
  - model: HGMAE
    model_key: hgmae
    model_plain: HGMAE
    value: 0.9129
    std: null
    paper_value: 0.9129
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9213
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2310.15318'
    at_pub_source_title: 'HetGPT: Harnessing the Power of Prompt Tuning in Pre-Trained
      Heterogeneous Graph Neural Networks'
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.008399999999999963
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.934
    true_std: 0.006
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.021100000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.934
    sort_std: 0.006
    global_rank: 51
    paper_rank: 83
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HetGPT: Harnessing the Power of Prompt Tuning in Pre-Trained
      Heterogeneous Graph Neural Networks'
    comparison_source_arxiv: '2310.15318'
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.9331
    std: null
    paper_value: 0.9331
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.916
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.017100000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9331
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: null
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: Mp2vec
    model_key: mp2vec
    model_plain: Mp2vec
    value: 0.9287
    std: null
    paper_value: 0.9287
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9304
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-18'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0017000000000000348
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9304
    true_std: null
    value_gap_source_arxiv: '2012.10024'
    value_gap_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0017000000000000348
    has_value_note: false
    value_note: ''
    sort_value: 0.9304
    sort_std: null
    global_rank: 57
    paper_rank: 60
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.8476
    std: null
    paper_value: 0.8476
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: 0.9016
    at_pub_std: 0.006
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05399999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9016
    true_std: 0.006
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.05399999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9016
    sort_std: 0.006
    global_rank: 87
    paper_rank: 114
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: SEEGERA
    model_key: seegera
    model_plain: SEEGERA
    value: 0.8664
    std: null
    paper_value: 0.8664
    paper_std: null
    metric: Micro-F1
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 10/10/80 semi-supervised split
    date: Nov 14, 2023
    date_display: Nov 2023
    date_iso: '2023-11-14'
    published_venue: KDD 2023
    published_conference: KDD 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8664
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8664
    sort_std: null
    global_rank: 99
    paper_rank: 99
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
    value: 0.6447
    std: 0.0136
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.07365'
    title: 'GraphControl: Adding Conditional Control to Universal Graph Pre-trained
      Models for Graph Domain Transfer Learning'
    date: Oct 11, 2023
    date_display: Oct 2023
    date_iso: '2023-10-11'
    venue: The Web Conference
    codebase_url: https://github.com/wykk00/GraphControl
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 185
    sort_value: 0.6447
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
single_proposed_model: GraMI
main_figure: /figures/2311.07929/main_figure.jpegoptim.jpg
---

