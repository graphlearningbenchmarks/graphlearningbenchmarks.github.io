---
title: Node-wise Diffusion for Scalable Graph Learning
arxiv_id: '2305.14000'
source_url: ''
authors:
- name: Keke Huang
  orcid: null
  s2_author_id: '2112440523'
  s2_url: null
- name: Jing Tang
  orcid: null
  s2_author_id: '144066821'
  s2_url: null
- name: Juncheng Liu
  orcid: null
  s2_author_id: '2108378854'
  s2_url: null
- name: Renchi Yang
  orcid: null
  s2_author_id: '2115421976'
  s2_url: null
- name: Xiaokui Xiao
  orcid: null
  s2_author_id: '152496559'
  s2_url: null
published_date: Apr 30, 2023
published_date_iso: '2023-04-30'
published_venue: WWW 2023
published_conference: WWW 2023
published_conference_short: WWW
published_conference_slug: www
abstract: Graph Neural Networks (GNNs) have shown superior performance for semi-supervised
  learning of numerous web applications, such as classification on web services and
  pages, analysis of online social networks, and recommendation in e-commerce. The
  state of the art derives representations for all nodes in graphs following the same
  diffusion (message passing) model without discriminating their uniqueness. However,
  (i) labeled nodes involved in model training usually account for a small portion
  of graphs in the semi-supervised setting, and (ii) different nodes locate at different
  graph local contexts and it inevitably degrades the representation qualities if
  treating them undistinguishedly in diffusion. To address the above issues, we develop
  NDM, a universal node-wise diffusion model, to capture the unique characteristics
  of each node in diffusion, by which NDM is able to yield high-quality node representations.
  In what follows, we customize NDM for semi-supervised learning and design the NIGCN
  model. In particular, NIGCN advances the efficiency significantly since it (i) produces
  representations for labeled nodes only and (ii) adopts well-designed neighbor sampling
  techniques tailored for node representation generation. Extensive experimental results
  on various types of web datasets, including citation, social and co-purchasing graphs,
  not only verify the state-of-the-art effectiveness of NIGCN but also strongly support
  the remarkable scalability of NIGCN. In particular, NIGCN completes representation
  generation and training within $10$ seconds on the dataset with hundreds of millions
  of nodes and billions of edges, up to orders of magnitude speedups over the baselines,
  while achieving the highest F1-scores on classification can be accessed at..
codebase_url: https://github.com/kkhuang81/NIGCN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NIGCN
mrr: 0.0064
adjusted_mrr: 0.0064
mrr_dataset_count: 3
benchmark_categories:
- Classic
- OGB
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id005
  dataset: Amazon2M
  rows:
  - model: Cluster-GCN
    model_key: cluster-gcn
    model_plain: Cluster-GCN
    value: 0.9041
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: May 20, 2019
    date_display: May 2019
    date_iso: '2019-05-20'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/google-research/google-research
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9041
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: VRGCN
    model_key: vrgcn
    model_plain: VRGCN
    value: 0.9021
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
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: May 20, 2019
    date_display: May 2019
    date_iso: '2019-05-20'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/google-research/google-research
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9021
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.6345
    std: 0.007
    paper_value: 0.6345
    paper_std: 0.007
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6345
    true_std: 0.007
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6345
    sort_std: 0.007
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
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.6078
    std: 0.0104
    paper_value: 0.6078
    paper_std: 0.0104
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6078
    true_std: 0.0104
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6078
    sort_std: 0.0104
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPRGo
    model_key: pprgo
    model_plain: PPRGo
    value: 0.601
    std: 0.0117
    paper_value: 0.601
    paper_std: 0.0117
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.601
    true_std: 0.0117
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.601
    sort_std: 0.0117
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
  - model: AGP
    model_key: agp
    model_plain: AGP
    value: 0.5572
    std: 0.0168
    paper_value: 0.5572
    paper_std: 0.0168
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5572
    true_std: 0.0168
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5572
    sort_std: 0.0168
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
  - model: NDLS
    model_key: ndls
    model_plain: NDLS
    value: 0.501
    std: 0.0209
    paper_value: 0.501
    paper_std: 0.0209
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.501
    true_std: 0.0209
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.501
    sort_std: 0.0209
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.4771
    std: 0.0107
    paper_value: 0.4771
    paper_std: 0.0107
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4771
    true_std: 0.0107
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4771
    sort_std: 0.0107
    global_rank: 8
    paper_rank: 8
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
    value: 0.4132
    std: 0.011
    paper_value: 0.4132
    paper_std: 0.011
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning task on Amazon dataset
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4132
    true_std: 0.011
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4132
    sort_std: 0.011
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
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
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
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
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
    input_feature_source: raw_features
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
  - model: EERM
    model_key: eerm
    model_plain: EERM
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
    input_feature_source: raw_features
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6741
    std: 0.0177
    paper_value: 0.6741
    paper_std: 0.0177
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.7923
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.11819999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8774
    true_std: 0.0041
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.20329999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8774
    sort_std: 0.0041
    global_rank: 20
    paper_rank: 770
    rank_delta: 750
    rank_delta_abs: 750
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6911
    std: 0.0146
    paper_value: 0.6911
    paper_std: 0.0146
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.10319999999999996
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
    value_gap: 0.18579999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 712
    rank_delta: 691
    rank_delta_abs: 691
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.6983
    std: 0.0127
    paper_value: 0.6983
    paper_std: 0.0127
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.805
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.10670000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8142
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1159
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 693
    rank_delta: 664
    rank_delta_abs: 664
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
    value: 0.6935
    std: 0.0093
    paper_value: 0.6935
    paper_std: 0.0093
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.8013
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1078
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
    value_gap: 0.11450000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 706
    rank_delta: 660
    rank_delta_abs: 660
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7049
    std: 0.0129
    paper_value: 0.7049
    paper_std: 0.0129
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.7765
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0716
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7965
    true_std: 0.0102
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.09160000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0102
    global_rank: 68
    paper_rank: 652
    rank_delta: 584
    rank_delta_abs: 584
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7618
    std: 0.0078
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 165
    sort_value: 0.7618
    sort_std: 0.0078
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NDLS
    model_key: ndls
    model_plain: NDLS
    value: 0.6963
    std: 0.0169
    paper_value: 0.6963
    paper_std: 0.0169
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-06'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.736
    true_std: null
    value_gap_source_arxiv: '2408.03152'
    value_gap_source_title: 'TSC: A Simple Two-Sided Constraint against Over-Smoothing'
    value_gap_source_is_current_paper: false
    value_gap: 0.03969999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.736
    sort_std: null
    global_rank: 312
    paper_rank: 697
    rank_delta: 385
    rank_delta_abs: 385
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDC
    model_key: gdc
    model_plain: GDC
    value: 0.6969
    std: 0.0142
    paper_value: 0.6969
    paper_std: 0.0142
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.734
    at_pub_std: 0.003
    at_pub_source_arxiv: '2301.09474'
    at_pub_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    at_pub_source_date_iso: '2023-01-23'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-01-23'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.03710000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.734
    true_std: 0.003
    value_gap_source_arxiv: '2301.09474'
    value_gap_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    value_gap_source_is_current_paper: false
    value_gap: 0.03710000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.003
    global_rank: 328
    paper_rank: 697
    rank_delta: 369
    rank_delta_abs: 369
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    comparison_source_arxiv: '2301.09474'
    is_best: false
    is_std_outlier: false
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.7018
    std: 0.019
    paper_value: 0.7018
    paper_std: 0.019
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.729
    at_pub_std: 0.005
    at_pub_source_arxiv: '2010.15421'
    at_pub_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    at_pub_source_date_iso: '2020-10-29'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.027200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.729
    true_std: 0.005
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.027200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.005
    global_rank: 393
    paper_rank: 676
    rank_delta: 283
    rank_delta_abs: 283
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    comparison_source_arxiv: '2010.15421'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7289
    std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 401
    sort_value: 0.7289
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.6751
    std: 0.0476
    paper_value: 0.6751
    paper_std: 0.0476
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.705
    at_pub_std: 0.004
    at_pub_source_arxiv: '2010.15421'
    at_pub_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    at_pub_source_date_iso: '2020-10-29'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-10-06'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.029899999999999927
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.723
    true_std: 0.0017
    value_gap_source_arxiv: '2510.04522'
    value_gap_source_title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion
      Framework for Graph Generation and Prediction'
    value_gap_source_is_current_paper: false
    value_gap: 0.04789999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.0017
    global_rank: 482
    paper_rank: 768
    rank_delta: 286
    rank_delta_abs: 286
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRAND(+)
    model_key: grand(+)
    model_plain: GRAND(+)
    value: 0.7142
    std: 0.0189
    paper_value: 0.7142
    paper_std: 0.0189
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7142
    true_std: 0.0189
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7142
    sort_std: 0.0189
    global_rank: 576
    paper_rank: 576
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.7135
    std: 0.0082
    paper_value: 0.7135
    paper_std: 0.0082
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7135
    true_std: 0.0082
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7135
    sort_std: 0.0082
    global_rank: 586
    paper_rank: 586
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPRGo
    model_key: pprgo
    model_plain: PPRGo
    value: 0.6892
    std: 0.0172
    paper_value: 0.6892
    paper_std: 0.0172
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.713
    at_pub_std: 0.003
    at_pub_source_arxiv: '2010.15421'
    at_pub_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    at_pub_source_date_iso: '2020-10-29'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-10-29'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.023799999999999932
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.713
    true_std: 0.003
    value_gap_source_arxiv: '2010.15421'
    value_gap_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    value_gap_source_is_current_paper: false
    value_gap: 0.023799999999999932
    has_value_note: false
    value_note: ''
    sort_value: 0.713
    sort_std: 0.003
    global_rank: 589
    paper_rank: 720
    rank_delta: 131
    rank_delta_abs: 131
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    comparison_source_arxiv: '2010.15421'
    is_best: false
    is_std_outlier: false
  - model: AGP
    model_key: agp
    model_plain: AGP
    value: 0.6715
    std: 0.0204
    paper_value: 0.6715
    paper_std: 0.0204
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6715
    true_std: 0.0204
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6715
    sort_std: 0.0204
    global_rank: 785
    paper_rank: 785
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: shaDow-GCN
    model_key: shadow-gcn
    model_plain: shaDow-GCN
    value: 0.6354
    std: 0.0111
    paper_value: 0.6354
    paper_std: 0.0111
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
    protocol_note: Transductive learning on Planetoid split (randomly sampled 20 nodes
      per class for training, 500 for val, 1000 for test).
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6354
    true_std: 0.0111
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6354
    sort_std: 0.0111
    global_rank: 866
    paper_rank: 866
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
  dataset: PubMed
  rows:
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.891
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.13021'
    title: Multi-Scale Attributed Node Embedding
    date: Sep 25, 2019
    date_display: Sep 2019
    date_iso: '2019-09-25'
    venue: J. Complex Networks
    codebase_url: https://github.com/benedekrozemberczki/MUSAE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.891
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8021
    std: 0.0179
    paper_value: 0.8021
    paper_std: 0.0179
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.884
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.08189999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.884
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.08189999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.001
    global_rank: 2
    paper_rank: 20
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7805
    std: 0.0164
    paper_value: 0.7805
    paper_std: 0.0164
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.875
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.09450000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.875
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.09450000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.875
    sort_std: 0.001
    global_rank: 3
    paper_rank: 30
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7882
    std: 0.019
    paper_value: 0.7882
    paper_std: 0.019
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.869
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.08079999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.08079999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.001
    global_rank: 4
    paper_rank: 26
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7692
    std: 0.0284
    paper_value: 0.7692
    paper_std: 0.0284
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.864
    at_pub_std: 0.001
    at_pub_source_arxiv: '1909.13021'
    at_pub_source_title: Multi-Scale Attributed Node Embedding
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.0948
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.864
    true_std: 0.001
    value_gap_source_arxiv: '1909.13021'
    value_gap_source_title: Multi-Scale Attributed Node Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.0948
    has_value_note: false
    value_note: ''
    sort_value: 0.864
    sort_std: 0.001
    global_rank: 6
    paper_rank: 35
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Attributed Node Embedding
    comparison_source_arxiv: '1909.13021'
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.809
    std: 0.0202
    paper_value: 0.809
    paper_std: 0.0202
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.809
    true_std: 0.0202
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.809
    sort_std: 0.0202
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
  - model: NDLS
    model_key: ndls
    model_plain: NDLS
    value: 0.8038
    std: 0.0141
    paper_value: 0.8038
    paper_std: 0.0141
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8038
    true_std: 0.0141
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8038
    sort_std: 0.0141
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.8009
    std: 0.0151
    paper_value: 0.8009
    paper_std: 0.0151
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8009
    true_std: 0.0151
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8009
    sort_std: 0.0151
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
  - model: GRAND(+)
    model_key: grand(+)
    model_plain: GRAND(+)
    value: 0.7918
    std: 0.0193
    paper_value: 0.7918
    paper_std: 0.0193
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7918
    true_std: 0.0193
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7918
    sort_std: 0.0193
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
  - model: AGP
    model_key: agp
    model_plain: AGP
    value: 0.7897
    std: 0.0133
    paper_value: 0.7897
    paper_std: 0.0133
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7897
    true_std: 0.0133
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7897
    sort_std: 0.0133
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT
    model_key: graphsaint
    model_plain: GraphSAINT
    value: 0.7865
    std: 0.0417
    paper_value: 0.7865
    paper_std: 0.0417
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7865
    true_std: 0.0417
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7865
    sort_std: 0.0417
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPRGo
    model_key: pprgo
    model_plain: PPRGo
    value: 0.782
    std: 0.0196
    paper_value: 0.782
    paper_std: 0.0196
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.0196
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.0196
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
  - model: GDC
    model_key: gdc
    model_plain: GDC
    value: 0.7767
    std: 0.0165
    paper_value: 0.7767
    paper_std: 0.0165
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7767
    true_std: 0.0165
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7767
    sort_std: 0.0165
    global_rank: 31
    paper_rank: 31
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
    value: 0.7731
    std: 0.0059
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.7731
    sort_std: 0.0059
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7411
    std: 0.0255
    paper_value: 0.7411
    paper_std: 0.0255
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-08'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7511
    true_std: 0.0127
    value_gap_source_arxiv: '2309.04082'
    value_gap_source_title: 'Curve Your Attention: Mixed-Curvature Transformers for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.7511
    sort_std: 0.0127
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
  - model: shaDow-GCN
    model_key: shadow-gcn
    model_plain: shaDow-GCN
    value: 0.7179
    std: 0.0292
    paper_value: 0.7179
    paper_std: 0.0292
    metric: F1
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
    protocol_note: Transductive learning on Planetoid split (Yang et al. 2016) using
      20 training, 500 validation, and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7179
    true_std: 0.0292
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7179
    sort_std: 0.0292
    global_rank: 39
    paper_rank: 39
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
    value: 0.6717
    std: 0.0091
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 41
    sort_value: 0.6717
    sort_std: 0.0091
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
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
    value: 0.8916
    std: 0.0116
    paper_value: 0.8916
    paper_std: 0.0116
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.966
    at_pub_std: null
    at_pub_source_arxiv: '2105.04528'
    at_pub_source_title: Accelerating Large Scale Real-Time GNN Inference using Channel
      Pruning
    at_pub_source_date_iso: '2021-05-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.07440000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: false
    value_gap: 0.07440000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
    global_rank: 18
    paper_rank: 152
    rank_delta: 134
    rank_delta_abs: 134
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    comparison_source_arxiv: '2105.04528'
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.953
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.10803'
    title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
    date: May 22, 2022
    date_display: May 2022
    date_iso: '2022-05-22'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/THUDM/GraphMAE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 68
    sort_value: 0.953
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.9264
    std: 0.0102
    paper_value: 0.9264
    paper_std: 0.0102
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.949
    at_pub_std: null
    at_pub_source_arxiv: '1812.04202'
    at_pub_source_title: 'Deep Learning on Graphs: A Survey'
    at_pub_source_date_iso: '2018-12-11'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022599999999999953
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: 0.0
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.022599999999999953
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0
    global_rank: 87
    paper_rank: 134
    rank_delta: 47
    rank_delta_abs: 47
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Deep Learning on Graphs: A Survey'
    comparison_source_arxiv: '1812.04202'
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.9243
    std: 0.01
    paper_value: 0.9243
    paper_std: 0.01
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.937
    at_pub_std: null
    at_pub_source_arxiv: '1801.10247'
    at_pub_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    at_pub_source_date_iso: '2018-01-30'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.012700000000000045
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.012700000000000045
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
    global_rank: 112
    paper_rank: 135
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    comparison_source_arxiv: '1801.10247'
    is_best: false
    is_std_outlier: false
  - model: PPRGo
    model_key: pprgo
    model_plain: PPRGo
    value: 0.7821
    std: 0.0307
    paper_value: 0.7821
    paper_std: 0.0307
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.937
    at_pub_std: null
    at_pub_source_arxiv: '2105.04528'
    at_pub_source_title: Accelerating Large Scale Real-Time GNN Inference using Channel
      Pruning
    at_pub_source_date_iso: '2021-05-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-05-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.15490000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2105.04528'
    value_gap_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    value_gap_source_is_current_paper: false
    value_gap: 0.15490000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
    global_rank: 113
    paper_rank: 157
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    comparison_source_arxiv: '2105.04528'
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.9342
    std: 0.0048
    paper_value: 0.9342
    paper_std: 0.0048
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9342
    true_std: 0.0048
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9342
    sort_std: 0.0048
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGP
    model_key: agp
    model_plain: AGP
    value: 0.9218
    std: 0.0088
    paper_value: 0.9218
    paper_std: 0.0088
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9218
    true_std: 0.0088
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9218
    sort_std: 0.0088
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NDLS
    model_key: ndls
    model_plain: NDLS
    value: 0.8525
    std: 0.0124
    paper_value: 0.8525
    paper_std: 0.0124
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8525
    true_std: 0.0124
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8525
    sort_std: 0.0124
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.7609
    std: 0.0175
    paper_value: 0.7609
    paper_std: 0.0175
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive learning on Reddit with 20 training, 500 validation,
      and 1000 testing nodes per class.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.392
    at_pub_std: 0.003
    at_pub_source_arxiv: '2207.09179'
    at_pub_source_title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented
      Optimization'
    at_pub_source_date_iso: '2022-07-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.3689
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7609
    true_std: 0.0175
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7609
    sort_std: 0.0175
    global_rank: 158
    paper_rank: 158
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented
      Optimization'
    comparison_source_arxiv: '2207.09179'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7216
    std: 0.0015
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/GraphAny
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 162
    sort_value: 0.7216
    sort_std: 0.0015
    comparison_type: global_top
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
- &id004
  dataset: ogbn-papers100M
  rows:
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.4981
    std: 0.011
    paper_value: 0.4981
    paper_std: 0.011
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive learning on Papers100M as per table caption and text.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4981
    true_std: 0.011
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4981
    sort_std: 0.011
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4859
    std: 0.0177
    paper_value: 0.4859
    paper_std: 0.0177
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive learning on Papers100M as per table caption and text.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4859
    true_std: 0.0177
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4859
    sort_std: 0.0177
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGP
    model_key: agp
    model_plain: AGP
    value: 0.4671
    std: 0.0199
    paper_value: 0.4671
    paper_std: 0.0199
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive learning on Papers100M as per table caption and text.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4671
    true_std: 0.0199
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4671
    sort_std: 0.0199
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
  - model: GBP
    model_key: gbp
    model_plain: GBP
    value: 0.4491
    std: 0.0123
    paper_value: 0.4491
    paper_std: 0.0123
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-papers100m (score=80)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive learning on Papers100M as per table caption and text.
    date: Apr 30, 2023
    date_display: Apr 2023
    date_iso: '2023-04-30'
    published_venue: WWW 2023
    published_conference: WWW 2023
    at_pub_value: 0.348
    at_pub_std: 0.001
    at_pub_source_arxiv: '2207.09179'
    at_pub_source_title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented
      Optimization'
    at_pub_source_date_iso: '2022-07-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-04-30'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.10110000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4491
    true_std: 0.0123
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4491
    sort_std: 0.0123
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented
      Optimization'
    comparison_source_arxiv: '2207.09179'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: OGB
  datasets:
  - *id004
- benchmark: Other Graph Benchmarks
  datasets:
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Reddit
      dataset_slug: reddit
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-papers100M
      dataset_slug: ogbn-papers100m
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
single_proposed_model: NIGCN
main_figure: /figures/2305.14000/main_figure.jpegoptim.jpg
---

