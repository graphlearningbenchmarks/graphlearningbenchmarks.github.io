---
title: Graph Contrastive Learning with Implicit Augmentations
arxiv_id: '2211.03710'
source_url: ''
authors:
- name: Huidong Liang
  orcid: null
  s2_author_id: '2152225219'
  s2_url: null
- name: Xingjian Du
  orcid: null
  s2_author_id: '46214809'
  s2_url: null
- name: Bilei Zhu
  orcid: null
  s2_author_id: '1842814'
  s2_url: null
- name: Zejun Ma
  orcid: null
  s2_author_id: '2919563'
  s2_url: null
- name: Ke Chen
  orcid: null
  s2_author_id: '2152953901'
  s2_url: null
- name: Junbin Gao
  orcid: null
  s2_author_id: '32278515'
  s2_url: null
published_date: Nov 7, 2022
published_date_iso: '2022-11-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Existing graph contrastive learning methods rely on augmentation techniques
  based on random perturbations (e.g., randomly adding or dropping edges and nodes).
  Nevertheless, altering certain edges or nodes can unexpectedly change the graph
  characteristics, and choosing the optimal perturbing ratio for each dataset requires
  onerous manual tuning. In this paper, we introduce Implicit Graph Contrastive Learning
  (iGCL), which utilizes augmentations in the latent space learned from a Variational
  Graph Auto-Encoder by reconstructing graph topological structure. Importantly, instead
  of explicitly sampling augmentations from latent distributions, we further propose
  an upper bound for the expected contrastive loss to improve the efficiency of our
  learning algorithm. Thus, graph semantics can be preserved within the augmentations
  in an intelligent way without arbitrary manual design or prior human knowledge.
  Experimental results on both graph-level and node-level tasks show that the proposed
  method achieves state-of-the-art performance compared to other benchmarks, where
  ablation studies in the end demonstrate the effectiveness of modules in iGCL.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- iGCL
mrr: 0.0024
adjusted_mrr: 0.0008
mrr_dataset_count: 1
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
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
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
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.815
    std: 0.002
    paper_value: 0.815
    paper_std: 0.002
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8728
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.057800000000000074
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
    value_gap: 0.08540000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 657
    rank_delta: 626
    rank_delta_abs: 626
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.83
    std: 0.007
    paper_value: 0.83
    paper_std: 0.007
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05900000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.059700000000000086
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 498
    rank_delta: 431
    rank_delta_abs: 431
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.83
    std: 0.007
    paper_value: 0.83
    paper_std: 0.007
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8777
    at_pub_std: 0.0183
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.047700000000000076
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8777
    true_std: 0.0183
    value_gap_source_arxiv: '2110.15777'
    value_gap_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    value_gap_source_is_current_paper: false
    value_gap: 0.047700000000000076
    has_value_note: false
    value_note: ''
    sort_value: 0.8777
    sort_std: 0.0183
    global_rank: 146
    paper_rank: 498
    rank_delta: 352
    rank_delta_abs: 352
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    comparison_source_arxiv: '2110.15777'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.833
    std: 0.004
    paper_value: 0.833
    paper_std: 0.004
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8362
    at_pub_std: 0.0113
    at_pub_source_arxiv: '2208.06743'
    at_pub_source_title: Enhancing Graph Contrastive Learning with Node Similarity
    at_pub_source_date_iso: '2022-08-13'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0032000000000000917
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.872
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.002
    global_rank: 176
    paper_rank: 460
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.823
    std: 0.006
    paper_value: 0.823
    paper_std: 0.006
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8508
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.027800000000000047
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.863
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.002
    global_rank: 227
    paper_rank: 566
    rank_delta: 339
    rank_delta_abs: 339
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.83
    std: 0.003
    paper_value: 0.83
    paper_std: 0.003
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8526
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022600000000000064
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8526
    true_std: 0.0008
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.022600000000000064
    has_value_note: false
    value_note: ''
    sort_value: 0.8526
    sort_std: 0.0008
    global_rank: 276
    paper_rank: 498
    rank_delta: 222
    rank_delta_abs: 222
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.831
    std: 0.003
    paper_value: 0.831
    paper_std: 0.003
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8207
    at_pub_std: 0.001
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.010299999999999976
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8409
    true_std: 0.0085
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.00990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.0085
    global_rank: 363
    paper_rank: 489
    rank_delta: 126
    rank_delta_abs: 126
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: iGCL
    model_key: igcl
    model_plain: iGCL
    value: 0.836
    std: 0.006
    paper_value: 0.836
    paper_std: 0.006
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.006
    value_gap_source_arxiv: '2211.03710'
    value_gap_source_title: Graph Contrastive Learning with Implicit Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.006
    global_rank: 423
    paper_rank: 423
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.763
    std: 0.002
    paper_value: 0.763
    paper_std: 0.002
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8059
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.04289999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.836
    true_std: 0.0052
    value_gap_source_arxiv: '2405.14742'
    value_gap_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07299999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0052
    global_rank: 418
    paper_rank: 838
    rank_delta: 420
    rank_delta_abs: 420
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.749
    std: 0.004
    paper_value: 0.749
    paper_std: 0.004
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
    date: Nov 7, 2022
    date_display: Nov 2022
    date_iso: '2022-11-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8011
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.052100000000000035
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8011
    true_std: 0.0022
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.052100000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.8011
    sort_std: 0.0022
    global_rank: 736
    paper_rank: 859
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7768
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 806
    sort_value: 0.7768
    sort_std: null
    comparison_type: global_top
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
single_proposed_model: iGCL
main_figure: /figures/2211.03710/main_figure.jpegoptim.jpg
---

