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
mrr: 0.0046
adjusted_mrr: 0.0046
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
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id005
  dataset: Amazon2M
  rows:
  - model: NIGCN
    model_key: cluster-gcn
    model_plain: NIGCN
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
  - model: NIGCN
    model_key: vrgcn
    model_plain: NIGCN
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
- &id001
  dataset: CiteSeer
  rows:
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: cna
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: is-gib
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
  - model: Diffusion-GCN (PPR) + LayerNorm + FF
    model_key: eerm
    model_plain: Diffusion-GCN (PPR) + LayerNorm + FF
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
    at_pub_value: 0.7933
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.09499999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8128
    true_std: 0.0071
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.11449999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8128
    sort_std: 0.0071
    global_rank: 25
    paper_rank: 610
    rank_delta: 585
    rank_delta_abs: 585
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
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
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.1078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8075
    true_std: 0.0078
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.11399999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8075
    sort_std: 0.0078
    global_rank: 32
    paper_rank: 625
    rank_delta: 593
    rank_delta_abs: 593
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
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.10319999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8033
    true_std: 0.0088
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.11219999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8033
    sort_std: 0.0088
    global_rank: 37
    paper_rank: 630
    rank_delta: 593
    rank_delta_abs: 593
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
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
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.11819999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7981
    true_std: 0.008
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.124
    has_value_note: false
    value_note: ''
    sort_value: 0.7981
    sort_std: 0.008
    global_rank: 43
    paper_rank: 678
    rank_delta: 635
    rank_delta_abs: 635
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
    at_pub_value: 0.7386
    at_pub_std: 0.0173
    at_pub_source_arxiv: '2302.12357'
    at_pub_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    at_pub_source_date_iso: '2023-02-23'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03370000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7422
    true_std: 0.0019
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0373
    has_value_note: false
    value_note: ''
    sort_value: 0.7422
    sort_std: 0.0019
    global_rank: 206
    paper_rank: 576
    rank_delta: 370
    rank_delta_abs: 370
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    comparison_source_arxiv: '2302.12357'
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
    global_rank: 266
    paper_rank: 614
    rank_delta: 348
    rank_delta_abs: 348
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
    value_gap_source_date_iso: '2020-10-29'
    value_gap_source_date_label: NeurIPS 2020
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
    value_gap_source_arxiv: '2010.15421'
    value_gap_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    value_gap_source_is_current_paper: false
    value_gap: 0.027200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.005
    global_rank: 330
    paper_rank: 593
    rank_delta: 263
    rank_delta_abs: 263
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    comparison_source_arxiv: '2010.15421'
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
    value_gap_source_date_iso: '2024-08-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.716
    true_std: 0.003
    value_gap_source_arxiv: '2408.00295'
    value_gap_source_title: Contrastive Graph Representation Learning with Adversarial
      Cross-view Reconstruction and Information Bottleneck
    value_gap_source_is_current_paper: false
    value_gap: 0.0024999999999999467
    has_value_note: false
    value_note: ''
    sort_value: 0.716
    sort_std: 0.003
    global_rank: 494
    paper_rank: 517
    rank_delta: 23
    rank_delta_abs: 23
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
    global_rank: 510
    paper_rank: 510
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
    global_rank: 520
    paper_rank: 636
    rank_delta: 116
    rank_delta_abs: 116
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    comparison_source_arxiv: '2010.15421'
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
    value_gap_source_date_iso: '2020-10-29'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.029899999999999927
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.705
    true_std: 0.004
    value_gap_source_arxiv: '2010.15421'
    value_gap_source_title: Scalable Graph Neural Networks via Bidirectional Propagation
    value_gap_source_is_current_paper: false
    value_gap: 0.029899999999999927
    has_value_note: false
    value_note: ''
    sort_value: 0.705
    sort_std: 0.004
    global_rank: 574
    paper_rank: 676
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
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
    true_value: 0.6963
    true_std: 0.0169
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6963
    sort_std: 0.0169
    global_rank: 615
    paper_rank: 615
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
    global_rank: 687
    paper_rank: 687
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
    global_rank: 759
    paper_rank: 759
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
  dataset: PubMed
  rows:
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
    true_value: 0.8021
    true_std: 0.0179
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8021
    sort_std: 0.0179
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 5
    paper_rank: 5
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
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    true_value: 0.7882
    true_std: 0.019
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7882
    sort_std: 0.019
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    true_value: 0.7837
    true_std: 0.0026
    value_gap_source_arxiv: '2309.04082'
    value_gap_source_title: 'Curve Your Attention: Mixed-Curvature Transformers for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0031999999999999806
    has_value_note: false
    value_note: ''
    sort_value: 0.7837
    sort_std: 0.0026
    global_rank: 11
    paper_rank: 12
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
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
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
    true_value: 0.7692
    true_std: 0.0284
    value_gap_source_arxiv: '2305.14000'
    value_gap_source_title: Node-wise Diffusion for Scalable Graph Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7692
    sort_std: 0.0284
    global_rank: 17
    paper_rank: 17
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
    global_rank: 20
    paper_rank: 20
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
    global_rank: 21
    paper_rank: 21
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
- &id003
  dataset: Reddit
  rows:
  - model: GraphAny
    model_key: node sampled soup
    model_plain: GraphAny
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
  - model: GraphAny
    model_key: gamlp(jk)
    model_plain: GraphAny
    value: 0.9704
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
    global_rank: 2
    sort_value: 0.9704
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphAny
    model_key: graphsaint
    model_plain: GraphAny
    value: 0.97
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
    arxiv_id: '2302.00924'
    title: 'LMC: Fast Training of GNNs via subgraph-wise sampling with Provable Convergence'
    date: Feb 2, 2023
    date_display: Feb 2023
    date_iso: '2023-02-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/MIRALab-USTC/GNN-LMC
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.97
    sort_std: null
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
    global_rank: 16
    paper_rank: 125
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Accelerating Large Scale Real-Time GNN Inference using
      Channel Pruning
    comparison_source_arxiv: '2105.04528'
    is_best: true
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
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
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
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: 0.022599999999999953
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: 0.0
    global_rank: 72
    paper_rank: 114
    rank_delta: 42
    rank_delta_abs: 42
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
    global_rank: 98
    paper_rank: 115
    rank_delta: 17
    rank_delta_abs: 17
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
    global_rank: 99
    paper_rank: 130
    rank_delta: 31
    rank_delta_abs: 31
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
    global_rank: 127
    paper_rank: 127
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
    global_rank: 131
    paper_rank: 131
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
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
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
---

