---
title: Deep Graph Contrastive Representation Learning
arxiv_id: '2006.04131'
source_url: ''
authors:
- name: Yanqiao Zhu
  orcid: null
  s2_author_id: '2653121'
  s2_url: null
- name: Yichen Xu
  orcid: null
  s2_author_id: '47103911'
  s2_url: null
- name: Feng Yu
  orcid: null
  s2_author_id: '2155385667'
  s2_url: null
- name: Q. Liu
  orcid: null
  s2_author_id: '48873756'
  s2_url: null
- name: Shu Wu
  orcid: null
  s2_author_id: '50425438'
  s2_url: null
- name: Liang Wang
  orcid: null
  s2_author_id: '123865558'
  s2_url: null
published_date: Jun 7, 2020
published_date_iso: '2020-06-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph representation learning nowadays becomes fundamental in analyzing
  graph-structured data. Inspired by recent success of contrastive methods, in this
  paper, we propose a novel framework for unsupervised graph representation learning
  by leveraging a contrastive objective at the node level. Specifically, we generate
  two graph views by corruption and learn node representations by maximizing the agreement
  of node representations in these two views. To provide diverse node contexts for
  the contrastive objective, we propose a hybrid scheme for generating graph views
  on both structure and attribute levels. Besides, we provide theoretical justification
  behind our motivation from two perspectives, mutual information and the classical
  triplet loss. We perform empirical experiments on both transductive and inductive
  learning tasks using a variety of real-world datasets. Experimental experiments
  demonstrate that despite its simplicity, our proposed method consistently outperforms
  existing state-of-the-art methods by large margins. Moreover, our unsupervised method
  even surpasses its supervised counterparts on transductive tasks, demonstrating
  its great potential in real-world applications.
codebase_url: https://github.com/CRIPAC-DIG/GRACE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GRACE
mrr: 0.0085
adjusted_mrr: 0.0085
mrr_dataset_count: 5
benchmark_categories:
- Classic
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: DBLP
  rows:
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    value: 0.949
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.949
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9489
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9489
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AdvSynGNN
    model_key: advsyngnn
    model_plain: AdvSynGNN
    value: 0.9486
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9486
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.812
    std: null
    paper_value: 0.812
    paper_std: null
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
    protocol_note: Transductive node classification using X and A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.941
    true_std: 0.003
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.1289999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.941
    sort_std: 0.003
    global_rank: 11
    paper_rank: 80
    rank_delta: 69
    rank_delta_abs: 69
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
    value: 0.832
    std: 0.001
    paper_value: 0.832
    paper_std: 0.001
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
    protocol_note: Transductive node classification using X and A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.88
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.04800000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.88
    sort_std: 0.002
    global_rank: 34
    paper_rank: 69
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.827
    std: null
    paper_value: 0.827
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification using X, A, and Y.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.715
    at_pub_std: 0.027
    at_pub_source_arxiv: '2004.13970'
    at_pub_source_title: Directed Graph Convolutional Network
    at_pub_source_date_iso: '2020-04-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.11199999999999999
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8758
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.048800000000000066
    has_value_note: false
    value_note: ''
    sort_value: 0.8758
    sort_std: 0.002
    global_rank: 36
    paper_rank: 69
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Directed Graph Convolutional Network
    comparison_source_arxiv: '2004.13970'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.872
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
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 38
    sort_value: 0.872
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.842
    std: 0.001
    paper_value: 0.842
    paper_std: 0.001
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
    protocol_note: Transductive node classification using X and A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.842
    true_std: 0.001
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.842
    sort_std: 0.001
    global_rank: 61
    paper_rank: 61
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
    value: 0.817
    std: null
    paper_value: 0.817
    paper_std: null
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
    protocol_note: Transductive node classification using X and A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.817
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: null
    global_rank: 77
    paper_rank: 77
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.817
    std: null
    paper_value: 0.817
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification using X, A, and Y.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.692
    at_pub_std: 0.028
    at_pub_source_arxiv: '2004.13970'
    at_pub_source_title: Directed Graph Convolutional Network
    at_pub_source_date_iso: '2020-04-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.125
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.817
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: null
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Directed Graph Convolutional Network
    comparison_source_arxiv: '2004.13970'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8118
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.04739'
    title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive Learning
      on Hypergraphs'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/wooner49/TriCL
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 82
    sort_value: 0.8118
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.788
    std: null
    paper_value: 0.788
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification using adjacency matrix A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.788
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: null
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + features
    model_key: deepwalk + features
    model_plain: DeepWalk + features
    value: 0.781
    std: null
    paper_value: 0.781
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification using X and A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.781
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.781
    sort_std: null
    global_rank: 98
    paper_rank: 98
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
    value: 0.759
    std: null
    paper_value: 0.759
    paper_std: null
    metric: Accuracy
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification using adjacency matrix A.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.759
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.759
    sort_std: null
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.716
    std: null
    paper_value: 0.716
    paper_std: null
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
    protocol_note: Transductive node classification using only node features X.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.716
    true_std: 0.001
    value_gap_source_arxiv: '2402.10468'
    value_gap_source_title: Adversarial Curriculum Graph Contrastive Learning with
      Pair-wise Augmentation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.716
    sort_std: 0.001
    global_rank: 130
    paper_rank: 130
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
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: PPI
  rows:
  - model: GAMLP(JK)
    model_key: gamlp(jk)
    model_plain: GAMLP(JK)
    value: 0.9982
    std: 0.01
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9982
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphCON-GCN
    model_key: graphcon-gcn
    model_plain: GraphCON-GCN
    value: 0.996
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.996
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.9956
    std: 0.02
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02133'
    title: Simple and Deep Graph Convolutional Networks
    date: Jul 4, 2020
    date_display: Jul 2020
    date_iso: '2020-07-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/DropEdge/DropEdge
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9956
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.985
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 21
    sort_value: 0.985
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GaAN-mean
    model_key: gaan-mean
    model_plain: GaAN-mean
    value: 0.969
    std: 0.002
    paper_value: 0.969
    paper_std: 0.002
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.969
    true_std: 0.002
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.969
    sort_std: 0.002
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.662
    std: 0.001
    paper_value: 0.662
    paper_std: 0.001
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6971
    true_std: 0.0017
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.03510000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6971
    sort_std: 0.0017
    global_rank: 124
    paper_rank: 137
    rank_delta: 13
    rank_delta_abs: 13
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
    value: 0.638
    std: 0.002
    paper_value: 0.638
    paper_std: 0.002
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.638
    at_pub_std: 0.002
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.638
    true_std: 0.002
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.638
    sort_std: 0.002
    global_rank: 148
    paper_rank: 148
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-LSTM
    model_key: graphsage-lstm
    model_plain: GraphSAGE-LSTM
    value: 0.482
    std: null
    paper_value: 0.482
    paper_std: null
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.612
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2019-09-07'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.13
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.612
    true_std: null
    value_gap_source_arxiv: '1909.03184'
    value_gap_source_title: 'Auto-GNN: Neural Architecture Search of Graph Neural
      Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.13
    has_value_note: false
    value_note: ''
    sort_value: 0.612
    sort_std: null
    global_rank: 156
    paper_rank: 170
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-pool
    model_key: graphsage-pool
    model_plain: GraphSAGE-pool
    value: 0.502
    std: null
    paper_value: 0.502
    paper_std: null
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.602
    at_pub_std: null
    at_pub_source_arxiv: '1910.02370'
    at_pub_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    at_pub_source_date_iso: '2019-10-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-10-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.09999999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.602
    true_std: null
    value_gap_source_arxiv: '1910.02370'
    value_gap_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    value_gap_source_is_current_paper: false
    value_gap: 0.09999999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.602
    sort_std: null
    global_rank: 159
    paper_rank: 169
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    comparison_source_arxiv: '1910.02370'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-GCN
    model_key: graphsage-gcn
    model_plain: GraphSAGE-GCN
    value: 0.465
    std: null
    paper_value: 0.465
    paper_std: null
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.601
    at_pub_std: null
    at_pub_source_arxiv: '1910.02370'
    at_pub_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    at_pub_source_date_iso: '2019-10-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-10-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.13599999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.601
    true_std: null
    value_gap_source_arxiv: '1910.02370'
    value_gap_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    value_gap_source_is_current_paper: false
    value_gap: 0.13599999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.601
    sort_std: null
    global_rank: 160
    paper_rank: 173
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    comparison_source_arxiv: '1910.02370'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-mean
    model_key: graphsage-mean
    model_plain: GraphSAGE-mean
    value: 0.486
    std: null
    paper_value: 0.486
    paper_std: null
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.598
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2019-10-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.11199999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.598
    true_std: null
    value_gap_source_arxiv: '1910.02370'
    value_gap_source_title: 'GraphZoom: A Multi-level Spectral Approach for Accurate
      and Scalable Graph Embedding'
    value_gap_source_is_current_paper: false
    value_gap: 0.11199999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.598
    sort_std: null
    global_rank: 161
    paper_rank: 169
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.422
    std: null
    paper_value: 0.422
    paper_std: null
    metric: F1
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
    protocol_note: Inductive node classification using micro-averaged F1 score.
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.422
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2022-07-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.425
    true_std: 0.003
    value_gap_source_arxiv: '2207.11996'
    value_gap_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.425
    sort_std: 0.003
    global_rank: 177
    paper_rank: 178
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Reddit
  rows:
  - model: Node Sampled Soup
    model_key: node sampled soup
    model_plain: Node Sampled Soup
    value: 0.9728
    std: 0.0008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_display: Jun 2023
    date_iso: '2023-06-18'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/VITA-Group/graph_ladling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9728
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EnGCN
    model_key: engcn
    model_plain: EnGCN
    value: 0.9714
    std: 0.0003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9714
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.971
    std: 0.0
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.971
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.966
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.04528'
    title: Accelerating Large Scale Real-Time GNN Inference using Channel Pruning
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    venue: Proceedings of the VLDB Endowment
    codebase_url: https://github.com/tedzhouhk/GCNP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 19
    sort_value: 0.966
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GaAN-mean
    model_key: gaan-mean
    model_plain: GaAN-mean
    value: 0.958
    std: 0.001
    paper_value: 0.958
    paper_std: 0.001
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.958
    true_std: 0.001
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.001
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
  - model: GraphSAGE-LSTM
    model_key: graphsage-lstm
    model_plain: GraphSAGE-LSTM
    value: 0.907
    std: null
    paper_value: 0.907
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.954
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2017-06-07'
    value_gap_source_date_label: NeurIPS 2017
    gap_vs_at_pub: 0.04699999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.954
    true_std: null
    value_gap_source_arxiv: '1706.02216'
    value_gap_source_title: Inductive Representation Learning on Large Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.04699999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.954
    sort_std: null
    global_rank: 65
    paper_rank: 153
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.942
    std: 0.0
    paper_value: 0.942
    paper_std: 0.0
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9501
    true_std: 0.0036
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.008099999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9501
    sort_std: 0.0036
    global_rank: 84
    paper_rank: 102
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-mean
    model_key: graphsage-mean
    model_plain: GraphSAGE-mean
    value: 0.897
    std: null
    paper_value: 0.897
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.95
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2017-06-07'
    value_gap_source_date_label: NeurIPS 2017
    gap_vs_at_pub: 0.052999999999999936
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '1706.02216'
    value_gap_source_title: Inductive Representation Learning on Large Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.052999999999999936
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 85
    paper_rank: 156
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE-pool
    model_key: graphsage-pool
    model_plain: GraphSAGE-pool
    value: 0.892
    std: null
    paper_value: 0.892
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.948
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2017-06-07'
    value_gap_source_date_label: NeurIPS 2017
    gap_vs_at_pub: 0.05599999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.948
    true_std: null
    value_gap_source_arxiv: '1706.02216'
    value_gap_source_title: Inductive Representation Learning on Large Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.05599999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: null
    global_rank: 94
    paper_rank: 158
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.94
    std: 0.001
    paper_value: 0.94
    paper_std: 0.001
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.94
    at_pub_std: 0.001
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2021-01-27'
    value_gap_source_date_label: TMLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9414
    true_std: 0.0003
    value_gap_source_arxiv: '2101.11525'
    value_gap_source_title: Calibrating and Improving Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0014000000000000679
    has_value_note: false
    value_note: ''
    sort_value: 0.9414
    sort_std: 0.0003
    global_rank: 105
    paper_rank: 108
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.937
    std: null
    paper_value: 0.937
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.937
    at_pub_std: null
    at_pub_source_arxiv: '1801.10247'
    at_pub_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    at_pub_source_date_iso: '2018-01-30'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
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
  - model: GraphSAGE-GCN
    model_key: graphsage-gcn
    model_plain: GraphSAGE-GCN
    value: 0.908
    std: null
    paper_value: 0.908
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.93
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2017-06-07'
    value_gap_source_date_label: NeurIPS 2017
    gap_vs_at_pub: 0.02200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.93
    true_std: null
    value_gap_source_arxiv: '1706.02216'
    value_gap_source_title: Inductive Representation Learning on Large Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.93
    sort_std: null
    global_rank: 135
    paper_rank: 152
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7435
    std: 0.0016
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.14908'
    title: 'ATLAS: Adaptive Topology-based Learning at Scale for Homophilic and Heterophilic
      Graphs'
    date: Dec 16, 2025
    date_display: Dec 2025
    date_iso: '2025-12-16'
    venue: arXiv.org
    codebase_url: https://github.com/atlaspaper16/ATLAS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 165
    sort_value: 0.7435
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk + features
    model_key: deepwalk + features
    model_plain: DeepWalk + features
    value: 0.691
    std: null
    paper_value: 0.691
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.691
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.691
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.691
    sort_std: null
    global_rank: 171
    paper_rank: 171
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Raw features
    model_key: raw features
    model_plain: Raw features
    value: 0.585
    std: null
    paper_value: 0.585
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.585
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2022-07-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.585
    true_std: 0.001
    value_gap_source_arxiv: '2207.11996'
    value_gap_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.585
    sort_std: 0.001
    global_rank: 187
    paper_rank: 187
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
    value: 0.324
    std: null
    paper_value: 0.324
    paper_std: null
    metric: F1
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
    table_ref: Table 1(b)
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive task using micro-averaged F1 score
    date: Jun 7, 2020
    date_display: Jun 2020
    date_iso: '2020-06-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.324
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2022-07-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.324
    true_std: null
    value_gap_source_arxiv: '2207.11996'
    value_gap_source_title: Generative Subgraph Contrast for Self-Supervised Graph
      Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.324
    sort_std: null
    global_rank: 203
    paper_rank: 203
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
    - dataset: PPI
      dataset_slug: ppi
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
single_proposed_model: GRACE
main_figure: /figures/2006.04131/main_figure.jpegoptim.jpg
---

