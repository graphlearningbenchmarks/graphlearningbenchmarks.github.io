---
title: 'BAED: a New Paradigm for Few-shot Graph Learning with Explanation in the Loop'
arxiv_id: '2603.01941'
source_url: ''
authors:
- name: Chao Chen
  orcid: null
  s2_author_id: '2354363111'
  s2_url: null
- name: Xujia Li
  orcid: null
  s2_author_id: '2355122204'
  s2_url: null
- name: Dongsheng Hong
  orcid: null
  s2_author_id: '2355172914'
  s2_url: null
- name: Shanshan Lin
  orcid: null
  s2_author_id: '2391721326'
  s2_url: null
- name: Xiangwen Liao
  orcid: null
  s2_author_id: '2271907316'
  s2_url: null
- name: Chuanyi Liu
  orcid: null
  s2_author_id: '2410633631'
  s2_url: null
- name: Lei Chen
  orcid: null
  s2_author_id: '2318958221'
  s2_url: null
published_date: Feb 1, 2026
published_date_iso: '2026-02-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: The challenges of training and inference in few-shot environments persist
  in the area of graph representation learning. The quality and quantity of labels
  are often insufficient due to the extensive expert knowledge required to annotate
  graph data. In this context, Few-Shot Graph Learning (FSGL) approaches have been
  developed over the years. Through sophisticated neural blackarchitectures and customized
  training pipelines, these approaches enhance model adaptability to new label distributions.
  However, compromises in blackthe model's robustness and interpretability can result
  in overfitting to noise in labeled data and blackdegraded performance. This paper
  introduces the first explanation-in-the-loop framework for the FSGL problem, called
  BAED. We novelly employ the belief propagation algorithm to facilitate label augmentation
  on graphs. Then, leveraging an auxiliary graph neural network and the gradient backpropagation
  method, our framework effectively extracts explanatory blacksubgraphs surrounding
  target blacknodes. The final blackpredictions are based on these informative subgraphs
  while mitigating the influence of redundant information from neighboring nodes.
  Extensive experiments on seven benchmark datasets demonstrate superior prediction
  accuracy, training efficiency, and explanation quality of BAED. As a pioneer, this
  work highlights the potential of the explanation-based research paradigm in FSGL.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- BAED
mrr: 0.0039
adjusted_mrr: 0.0013
mrr_dataset_count: 1
benchmark_categories:
- Classic
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
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
- &id001
  dataset: Coauthor-CS
  rows:
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.969
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: gwn-fa
    model_plain: DoG
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: gwn-sym
    model_plain: DoG
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.183
    std: null
    paper_value: 0.183
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9514
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2505.20034'
    at_pub_source_title: Graph Wave Networks
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.7684
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9514
    true_std: 0.0025
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.7684
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0025
    global_rank: 19
    paper_rank: 256
    rank_delta: 237
    rank_delta_abs: 237
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Wave Networks
    comparison_source_arxiv: '2505.20034'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.216
    std: null
    paper_value: 0.216
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9437
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2505.20034'
    at_pub_source_title: Graph Wave Networks
    at_pub_source_date_iso: '2025-04-22'
    at_pub_source_date_label: WWW 2025
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.7277
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9437
    true_std: 0.0028
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.7277
    has_value_note: false
    value_note: ''
    sort_value: 0.9437
    sort_std: 0.0028
    global_rank: 33
    paper_rank: 253
    rank_delta: 220
    rank_delta_abs: 220
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Wave Networks
    comparison_source_arxiv: '2505.20034'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.28
    std: null
    paper_value: 0.28
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.927
    at_pub_std: 0.001
    at_pub_source_arxiv: '2111.10698'
    at_pub_source_title: Towards Graph Self-Supervised Learning with Contrastive Adjusted
      Zooming
    at_pub_source_date_iso: '2021-11-20'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-11-20'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.647
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.927
    true_std: 0.001
    value_gap_source_arxiv: '2111.10698'
    value_gap_source_title: Towards Graph Self-Supervised Learning with Contrastive
      Adjusted Zooming
    value_gap_source_is_current_paper: false
    value_gap: 0.647
    has_value_note: false
    value_note: ''
    sort_value: 0.927
    sort_std: 0.001
    global_rank: 118
    paper_rank: 244
    rank_delta: 126
    rank_delta_abs: 126
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Graph Self-Supervised Learning with Contrastive
      Adjusted Zooming
    comparison_source_arxiv: '2111.10698'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.119
    std: null
    paper_value: 0.119
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.914
    at_pub_std: 0.002
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.795
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.914
    true_std: 0.002
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.795
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: 0.002
    global_rank: 163
    paper_rank: 257
    rank_delta: 94
    rank_delta_abs: 94
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: HiD
    model_key: hid
    model_plain: HiD
    value: 0.278
    std: null
    paper_value: 0.278
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.278
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.278
    sort_std: null
    global_rank: 245
    paper_rank: 245
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCI
    model_key: dci
    model_plain: DCI
    value: 0.26
    std: null
    paper_value: 0.26
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.26
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.26
    sort_std: null
    global_rank: 246
    paper_rank: 246
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPN
    model_key: gpn
    model_plain: GPN
    value: 0.259
    std: null
    paper_value: 0.259
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.259
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.259
    sort_std: null
    global_rank: 247
    paper_rank: 247
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: tsGCN
    model_key: tsgcn
    model_plain: tsGCN
    value: 0.255
    std: null
    paper_value: 0.255
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.255
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.255
    sort_std: null
    global_rank: 248
    paper_rank: 248
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
    value: 0.226
    std: null
    paper_value: 0.226
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.226
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.226
    sort_std: null
    global_rank: 253
    paper_rank: 253
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BAED
    model_key: baed
    model_plain: BAED
    value: 0.21
    std: null
    paper_value: 0.21
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.21
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.21
    sort_std: null
    global_rank: 255
    paper_rank: 255
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+IG
    model_key: sage+ig
    model_plain: SAGE+IG
    value: 0.21
    std: null
    paper_value: 0.21
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.21
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.21
    sort_std: null
    global_rank: 254
    paper_rank: 254
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+SM
    model_key: sage+sm
    model_plain: SAGE+SM
    value: 0.192
    std: null
    paper_value: 0.192
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.192
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.192
    sort_std: null
    global_rank: 256
    paper_rank: 256
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DLRGAE
    model_key: dlrgae
    model_plain: DLRGAE
    value: 0.181
    std: null
    paper_value: 0.181
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS dataset.
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.181
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.181
    sort_std: null
    global_rank: 257
    paper_rank: 257
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
  dataset: DBLP
  rows:
  - model: STPGC
    model_key: hg-scm
    model_plain: STPGC
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
  - model: STPGC
    model_key: advsyngnn
    model_plain: STPGC
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
    global_rank: 2
    sort_value: 0.9486
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: STPGC
    model_key: simplehgn
    model_plain: STPGC
    value: 0.9446
    std: 0.0022
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
    global_rank: 3
    sort_value: 0.9446
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.443
    std: null
    paper_value: 0.443
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8859
    at_pub_std: 0.001
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.4429
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8859
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.4429
    has_value_note: false
    value_note: ''
    sort_value: 0.8859
    sort_std: 0.001
    global_rank: 23
    paper_rank: 133
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    comparison_source_arxiv: '2206.04739'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.443
    std: null
    paper_value: 0.443
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8758
    at_pub_std: 0.002
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.4328
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8758
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.4328
    has_value_note: false
    value_note: ''
    sort_value: 0.8758
    sort_std: 0.002
    global_rank: 28
    paper_rank: 133
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    comparison_source_arxiv: '2206.04739'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.443
    std: null
    paper_value: 0.443
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.872
    at_pub_std: null
    at_pub_source_arxiv: '2112.08331'
    at_pub_source_title: Model Stealing Attacks Against Inductive Graph Neural Networks
    at_pub_source_date_iso: '2021-12-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.429
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.872
    true_std: null
    value_gap_source_arxiv: '2112.08331'
    value_gap_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.429
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: null
    global_rank: 31
    paper_rank: 133
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    comparison_source_arxiv: '2112.08331'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.443
    std: null
    paper_value: 0.443
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.858
    at_pub_std: null
    at_pub_source_arxiv: '2112.08331'
    at_pub_source_title: Model Stealing Attacks Against Inductive Graph Neural Networks
    at_pub_source_date_iso: '2021-12-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-12-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.415
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.858
    true_std: null
    value_gap_source_arxiv: '2112.08331'
    value_gap_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.415
    has_value_note: false
    value_note: ''
    sort_value: 0.858
    sort_std: null
    global_rank: 37
    paper_rank: 133
    rank_delta: 96
    rank_delta_abs: 96
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Model Stealing Attacks Against Inductive Graph Neural
      Networks
    comparison_source_arxiv: '2112.08331'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.448
    std: null
    paper_value: 0.448
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.817
    at_pub_std: null
    at_pub_source_arxiv: '2006.04131'
    at_pub_source_title: Deep Graph Contrastive Representation Learning
    at_pub_source_date_iso: '2020-06-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.36899999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.817
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.36899999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: null
    global_rank: 68
    paper_rank: 132
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Deep Graph Contrastive Representation Learning
    comparison_source_arxiv: '2006.04131'
    is_best: false
    is_std_outlier: false
  - model: GPN
    model_key: gpn
    model_plain: GPN
    value: 0.517
    std: null
    paper_value: 0.517
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.754
    at_pub_std: 0.023
    at_pub_source_arxiv: '2210.12130'
    at_pub_source_title: Graph Few-shot Learning with Task-specific Structures
    at_pub_source_date_iso: '2022-10-21'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-21'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.237
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.754
    true_std: 0.023
    value_gap_source_arxiv: '2210.12130'
    value_gap_source_title: Graph Few-shot Learning with Task-specific Structures
    value_gap_source_is_current_paper: false
    value_gap: 0.237
    has_value_note: false
    value_note: ''
    sort_value: 0.754
    sort_std: 0.023
    global_rank: 99
    paper_rank: 129
    rank_delta: 30
    rank_delta_abs: 30
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Few-shot Learning with Task-specific Structures
    comparison_source_arxiv: '2210.12130'
    is_best: false
    is_std_outlier: true
  - model: SAGE+SM
    model_key: sage+sm
    model_plain: SAGE+SM
    value: 0.698
    std: null
    paper_value: 0.698
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.698
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.698
    sort_std: null
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE+IG
    model_key: sage+ig
    model_plain: SAGE+IG
    value: 0.69
    std: null
    paper_value: 0.69
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.69
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.69
    sort_std: null
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DCI
    model_key: dci
    model_plain: DCI
    value: 0.449
    std: null
    paper_value: 0.449
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.449
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.449
    sort_std: null
    global_rank: 132
    paper_rank: 132
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HiD
    model_key: hid
    model_plain: HiD
    value: 0.447
    std: null
    paper_value: 0.447
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.447
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.447
    sort_std: null
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DLRGAE
    model_key: dlrgae
    model_plain: DLRGAE
    value: 0.443
    std: null
    paper_value: 0.443
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.443
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.443
    sort_std: null
    global_rank: 134
    paper_rank: 134
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: tsGCN
    model_key: tsgcn
    model_plain: tsGCN
    value: 0.442
    std: null
    paper_value: 0.442
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
    protocol_note: Standard node classification task on DBLP
    date: Feb 1, 2026
    date_display: Feb 2026
    date_iso: '2026-02-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-01'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.442
    true_std: null
    value_gap_source_arxiv: '2603.01941'
    value_gap_source_title: 'BAED: a New Paradigm for Few-shot Graph Learning with
      Explanation in the Loop'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.442
    sort_std: null
    global_rank: 135
    paper_rank: 135
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
single_proposed_model: BAED
---

