---
title: Generative-Contrastive Heterogeneous Graph Neural Network
arxiv_id: '2404.02810'
source_url: ''
authors:
- name: Yu Wang
  orcid: null
  s2_author_id: '2153605800'
  s2_url: null
- name: Lei Sang
  orcid: null
  s2_author_id: '2274931348'
  s2_url: null
- name: Yi Zhang
  orcid: null
  s2_author_id: '2275044076'
  s2_url: null
- name: Yiwen Zhang
  orcid: null
  s2_author_id: '2154556002'
  s2_url: null
- name: Xindong Wu
  orcid: null
  s2_author_id: '2255396936'
  s2_url: null
published_date: Apr 3, 2024
published_date_iso: '2024-04-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Heterogeneous Graphs (HGs) effectively model complex relationships in the
  real world through multi-type nodes and edges. In recent years, inspired by self-supervised
  learning (SSL), contrastive learning (CL)-based Heterogeneous Graphs Neural Networks
  (HGNNs) have shown great potential in utilizing data augmentation and contrastive
  discriminators for downstream tasks. However, data augmentation remains limited
  due to the graph data''s integrity. Furthermore, the contrastive discriminators
  suffer from sampling bias and lack local heterogeneous information. To tackle the
  above limitations, we propose a novel Generative-Contrastive Heterogeneous Graph
  Neural Network (GC-HGNN). Specifically, we propose a heterogeneous graph generative
  learning method that enhances CL-based paradigm. This paradigm includes: 1) A contrastive
  view augmentation strategy using a masked autoencoder. 2) Position-aware and semantics-aware
  positive sample sampling strategy for generating hard negative samples. 3) A hierarchical
  contrastive learning strategy aimed at capturing local and global information. Furthermore,
  the hierarchical contrastive learning and sampling strategies aim to constitute
  an enhanced contrastive discriminator under the generative-contrastive perspective.
  Finally, we compare our model with seventeen baselines on eight real-world datasets.
  Our model outperforms the latest baselines on node classification and link prediction
  tasks. To reproduce our work, we have open-sourced our code at https://github.com/wangyu0627/GC-HGNN.'
codebase_url: https://github.com/wangyu0627/GC-HGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GC-HGNN
mrr: 0.3444
adjusted_mrr: 0.3444
mrr_dataset_count: 3
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 3
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: ACM
  rows:
  - model: SlotGAT
    model_key: hetgnn
    model_plain: SlotGAT
    value: 0.979
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    venue: Knowledge-Based Systems
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.979
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: comch
    model_plain: SlotGAT
    value: 0.947
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    venue: Knowledge-Based Systems
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: lmsps
    model_plain: SlotGAT
    value: 0.9469
    std: 0.0036
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9469
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MHGCN
    model_key: mhgcn
    model_plain: MHGCN
    value: 0.887
    std: 0.0022
    paper_value: 0.887
    paper_std: 0.0022
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2022'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9197
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.03269999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9375
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.05049999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9375
    sort_std: null
    global_rank: 14
    paper_rank: 76
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.882
    std: 0.0037
    paper_value: 0.882
    paper_std: 0.0037
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2019'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9079
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.025900000000000034
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9185
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.03649999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: null
    global_rank: 50
    paper_rank: 82
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.882
    std: 0.0026
    paper_value: 0.882
    paper_std: 0.0026
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.91
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.028000000000000025
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.916
    true_std: 0.006
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.03400000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: 0.006
    global_rank: 53
    paper_rank: 82
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: HGCML
    model_key: hgcml
    model_plain: HGCML
    value: 0.879
    std: 0.0027
    paper_value: 0.879
    paper_std: 0.0027
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9102
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.031200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9102
    true_std: 0.0013
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.031200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9102
    sort_std: 0.0013
    global_rank: 58
    paper_rank: 86
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: HGMAE
    model_key: hgmae
    model_plain: HGMAE
    value: 0.8915
    std: 0.0031
    paper_value: 0.8915
    paper_std: 0.0031
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8859
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2310.15318'
    at_pub_source_title: 'HetGPT: Harnessing the Power of Prompt Tuning in Pre-Trained
      Heterogeneous Graph Neural Networks'
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.005599999999999938
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.906
    true_std: 0.007
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.014500000000000068
    has_value_note: false
    value_note: ''
    sort_value: 0.906
    sort_std: 0.007
    global_rank: 61
    paper_rank: 73
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GC-HGNN
    model_key: gc-hgnn
    model_plain: GC-HGNN
    value: 0.9036
    std: 0.0031
    paper_value: 0.9036
    paper_std: 0.0031
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9036
    true_std: 0.0031
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9036
    sort_std: 0.0031
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.876
    std: 0.0035
    paper_value: 0.876
    paper_std: 0.0035
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.898
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.898
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.898
    sort_std: null
    global_rank: 71
    paper_rank: 90
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
  - model: HeCo
    model_key: heco
    model_plain: HeCo
    value: 0.8871
    std: 0.0043
    paper_value: 0.8871
    paper_std: 0.0043
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2021'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8897
    at_pub_std: 0.0112
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0026000000000000467
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8897
    true_std: 0.0112
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0026000000000000467
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0112
    global_rank: 75
    paper_rank: 76
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Mp2vec
    model_key: mp2vec
    model_plain: Mp2vec
    value: 0.7286
    std: 0.0092
    paper_value: 0.7286
    paper_std: 0.0092
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7982
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0696
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.881
    true_std: 0.003
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.15239999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.881
    sort_std: 0.003
    global_rank: 83
    paper_rank: 112
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.7405
    std: 0.0047
    paper_value: 0.7405
    paper_std: 0.0047
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8178
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07729999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8178
    true_std: 0.0004
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.07729999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8178
    sort_std: 0.0004
    global_rank: 106
    paper_rank: 112
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: HERec
    model_key: herec
    model_plain: HERec
    value: 0.7445
    std: 0.0045
    paper_value: 0.7445
    paper_std: 0.0045
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2018'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on ACM dataset using Micro-F1 metric.
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6715
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07300000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7445
    true_std: 0.0045
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7445
    sort_std: 0.0045
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
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
- &id001
  dataset: DBLP
  rows:
  - model: HERec
    model_key: herec
    model_plain: HERec
    value: 0.9037
    std: 0.0047
    paper_value: 0.9037
    paper_std: 0.0047
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2018'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9993
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.09560000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9993
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.09560000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9993
    sort_std: null
    global_rank: 1
    paper_rank: 81
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: hetsann
    model_plain: SlotGAT
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
    is_best: true
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.9012
    std: 0.0045
    paper_value: 0.9012
    paper_std: 0.0045
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9941
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.09289999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9941
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.09289999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9941
    sort_std: null
    global_rank: 3
    paper_rank: 82
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: true
    is_std_outlier: false
  - model: MHGCN
    model_key: mhgcn
    model_plain: MHGCN
    value: 0.9062
    std: 0.0019
    paper_value: 0.9062
    paper_std: 0.0019
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2022'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.952
    at_pub_std: 0.0203
    at_pub_source_arxiv: '2208.06129'
    at_pub_source_title: Multiplex Heterogeneous Graph Convolutional Network
    at_pub_source_date_iso: '2022-08-12'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-08-12'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.04579999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.952
    true_std: 0.0203
    value_gap_source_arxiv: '2208.06129'
    value_gap_source_title: Multiplex Heterogeneous Graph Convolutional Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04579999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.0203
    global_rank: 13
    paper_rank: 80
    rank_delta: 67
    rank_delta_abs: 67
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multiplex Heterogeneous Graph Convolutional Network
    comparison_source_arxiv: '2208.06129'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.8518
    std: 0.0049
    paper_value: 0.8518
    paper_std: 0.0049
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2019'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9369
    at_pub_std: null
    at_pub_source_arxiv: '2311.07929'
    at_pub_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    at_pub_source_date_iso: '2023-11-14'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.08509999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9369
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: false
    value_gap: 0.08509999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9369
    sort_std: null
    global_rank: 46
    paper_rank: 99
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    comparison_source_arxiv: '2311.07929'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.9124
    std: 0.0049
    paper_value: 0.9124
    paper_std: 0.0049
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A, Y (features, structure,
      labels)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9365
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.02410000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9349
    true_std: 0.0025
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.022499999999999964
    has_value_note: false
    value_note: ''
    sort_value: 0.9349
    sort_std: 0.0025
    global_rank: 48
    paper_rank: 79
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGMAE
    model_key: hgmae
    model_plain: HGMAE
    value: 0.9189
    std: 0.0035
    paper_value: 0.9189
    paper_std: 0.0035
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9213
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2310.15318'
    at_pub_source_title: 'HetGPT: Harnessing the Power of Prompt Tuning in Pre-Trained
      Heterogeneous Graph Neural Networks'
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0023999999999999577
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.015100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.934
    sort_std: 0.006
    global_rank: 50
    paper_rank: 73
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.9066
    std: 0.0046
    paper_value: 0.9066
    paper_std: 0.0046
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9331
    at_pub_std: null
    at_pub_source_arxiv: '2311.07929'
    at_pub_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    at_pub_source_date_iso: '2023-11-14'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.02650000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9331
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: false
    value_gap: 0.02650000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: null
    global_rank: 52
    paper_rank: 79
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    comparison_source_arxiv: '2311.07929'
    is_best: false
    is_std_outlier: false
  - model: HGCML
    model_key: hgcml
    model_plain: HGCML
    value: 0.9111
    std: 0.0049
    paper_value: 0.9111
    paper_std: 0.0049
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9329
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.02179999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9329
    true_std: 0.0012
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.02179999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9329
    sort_std: 0.0012
    global_rank: 53
    paper_rank: 79
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: GC-HGNN
    model_key: gc-hgnn
    model_plain: GC-HGNN
    value: 0.9301
    std: 0.003
    paper_value: 0.9301
    paper_std: 0.003
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9301
    true_std: 0.003
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9301
    sort_std: 0.003
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
  - model: Mp2vec
    model_key: mp2vec
    model_plain: Mp2vec
    value: 0.903
    std: 0.0038
    paper_value: 0.903
    paper_std: 0.0038
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
    input_feature_source: raw_features
    feature_source_evidence: Table 2 indicates input is A (graph structure)
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9304
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.02739999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9287
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: false
    value_gap: 0.025699999999999945
    has_value_note: false
    value_note: ''
    sort_value: 0.9287
    sort_std: null
    global_rank: 57
    paper_rank: 81
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HeCo
    model_key: heco
    model_plain: HeCo
    value: 0.9059
    std: 0.0025
    paper_value: 0.9059
    paper_std: 0.0025
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Table 2 indicates input is X, A (features, structure)
    table_ref: Table 2
    source_ref: '2021'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on DBLP using Micro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9224
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.01649999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9224
    true_std: 0.0048
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.01649999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9224
    sort_std: 0.0048
    global_rank: 68
    paper_rank: 81
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
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
- &id003
  dataset: Freebase
  rows:
  - model: GC-HGNN
    model_key: gc-hgnn
    model_plain: GC-HGNN
    value: 0.6247
    std: 0.0042
    paper_value: 0.6247
    paper_std: 0.0042
    metric: Macro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6247
    true_std: 0.0042
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6247
    sort_std: 0.0042
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
  - model: HGMAE
    model_key: hgmae
    model_plain: HGMAE
    value: 0.6082
    std: 0.0051
    paper_value: 0.6082
    paper_std: 0.0051
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6082
    true_std: 0.0051
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6082
    sort_std: 0.0051
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
  - model: HeCo
    model_key: heco
    model_plain: HeCo
    value: 0.5987
    std: 0.0033
    paper_value: 0.5987
    paper_std: 0.0033
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    table_ref: Table 2
    source_ref: '2021'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5987
    true_std: 0.0033
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5987
    sort_std: 0.0033
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HERec
    model_key: herec
    model_plain: HERec
    value: 0.5946
    std: 0.0116
    paper_value: 0.5946
    paper_std: 0.0116
    metric: Macro-F1
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
    feature_source_evidence: Uses graph structure A only
    table_ref: Table 2
    source_ref: '2018'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5946
    true_std: 0.0116
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5946
    sort_std: 0.0116
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.592
    std: 0.005
    paper_value: 0.592
    paper_std: 0.005
    metric: Macro-F1
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
    feature_source_evidence: Uses graph structure A only
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.005
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.005
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGCML
    model_key: hgcml
    model_plain: HGCML
    value: 0.5892
    std: 0.0257
    paper_value: 0.5892
    paper_std: 0.0257
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    table_ref: Table 2
    source_ref: '2023'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5892
    true_std: 0.0257
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5892
    sort_std: 0.0257
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
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.585
    std: 0.0093
    paper_value: 0.585
    paper_std: 0.0093
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X, A, and Y (features, structure, labels)
    table_ref: Table 2
    source_ref: '2019'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6011
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.016100000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.585
    true_std: 0.0093
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.585
    sort_std: 0.0093
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.583
    std: 0.0072
    paper_value: 0.583
    paper_std: 0.0072
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X, A, and Y (features, structure, labels)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6176
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.034600000000000075
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.583
    true_std: 0.0072
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.583
    sort_std: 0.0072
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: MHGCN
    model_key: mhgcn
    model_plain: MHGCN
    value: 0.5712
    std: 0.0032
    paper_value: 0.5712
    paper_std: 0.0032
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X, A, and Y (features, structure, labels)
    table_ref: Table 2
    source_ref: '2022'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5712
    true_std: 0.0032
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5712
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
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.5599
    std: 0.0059
    paper_value: 0.5599
    paper_std: 0.0059
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    table_ref: Table 2
    source_ref: '2020'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5599
    true_std: 0.0059
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5599
    sort_std: 0.0059
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Mp2vec
    model_key: mp2vec
    model_plain: Mp2vec
    value: 0.555
    std: 0.0049
    paper_value: 0.555
    paper_std: 0.0049
    metric: Macro-F1
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
    feature_source_evidence: Uses graph structure A only
    table_ref: Table 2
    source_ref: '2017'
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on Freebase using Macro-F1 metric
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.575
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.019999999999999907
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.555
    true_std: 0.0049
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.555
    sort_std: 0.0049
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  rank_metric: Macro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Macro-F1
  paper_metrics:
  - Macro-F1
  metric: Macro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: Freebase
      dataset_slug: freebase
single_proposed_model: GC-HGNN
main_figure: /figures/2404.02810/main_figure.jpegoptim.jpg
---

