---
title: Adaptive Sampling Towards Fast Graph Representation Learning
arxiv_id: '1809.05343'
source_url: ''
authors:
- name: Wen-bing Huang
  orcid: null
  s2_author_id: '2978255'
  s2_url: null
- name: Tong Zhang
  orcid: null
  s2_author_id: '2146324552'
  s2_url: null
- name: Yu Rong
  orcid: null
  s2_author_id: '48537464'
  s2_url: null
- name: Junzhou Huang
  orcid: null
  s2_author_id: '1768190'
  s2_url: null
published_date: Sep 1, 2018
published_date_iso: '2018-09-01'
published_venue: NeurIPS 2018
published_conference: NeurIPS 2018
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Graph Convolutional Networks (GCNs) have become a crucial tool on learning
  representations of graph vertices. The main challenge of adapting GCNs on large-scale
  graphs is the scalability issue that it incurs heavy cost both in computation and
  memory due to the uncontrollable neighborhood expansion across layers. In this paper,
  we accelerate the training of GCNs through developing an adaptive layer-wise sampling
  method. By constructing the network layer by layer in a top-down passway, we sample
  the lower layer conditioned on the top one, where the sampled neighborhoods are
  shared by different parent nodes and the over expansion is avoided owing to the
  fixed-size sampling. More importantly, the proposed sampler is adaptive and applicable
  for explicit variance reduction, which in turn enhances the training of our method.
  Furthermore, we propose a novel and economical approach to promote the message passing
  over distant nodes by applying skip connections. Intensive experiments on several
  benchmarks verify the effectiveness of our method regarding the classification accuracy
  while enjoying faster convergence speed.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  dataset: Reddit
  rows:
  - model: GAP-EDP
    model_key: gap-edp
    model_plain: GAP-EDP
    value: 0.987
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_display: Mar 2022
    date_iso: '2022-03-02'
    venue: USENIX Security Symposium
    codebase_url: https://github.com/sisaman/GAP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.987
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NE-ASGCN
    model_key: ne-asgcn
    model_plain: NE-ASGCN
    value: 0.9758
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.16097'
    title: Neighbor Enhanced Graph Convolutional Networks for Node Classification
      and Recommendation
    date: Mar 1, 2022
    date_display: Mar 2022
    date_iso: '2022-03-01'
    venue: Knowledge-Based Systems
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9758
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HSGT
    model_key: hsgt
    model_plain: HSGT
    value: 0.973
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.02866'
    title: Hierarchical Transformer for Scalable Graph Learning
    date: May 4, 2023
    date_display: May 2023
    date_iso: '2023-05-04'
    venue: International Joint Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.973
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9432
    std: null
    paper_value: 0.9432
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
    source_ref: hamilton 2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-04'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9653
    true_std: 0.0011
    value_gap_source_arxiv: '2305.02866'
    value_gap_source_title: Hierarchical Transformer for Scalable Graph Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.02210000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9653
    sort_std: 0.0011
    global_rank: 20
    paper_rank: 72
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.965
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_display: Jun 2024
    date_iso: '2024-06-17'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 22
    sort_value: 0.965
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Adapt
    model_key: adapt
    model_plain: Adapt
    value: 0.9627
    std: 0.0032
    paper_value: 0.9627
    paper_std: 0.0032
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
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-01'
    value_gap_source_date_label: NeurIPS 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9627
    true_std: 0.0032
    value_gap_source_arxiv: '1809.05343'
    value_gap_source_title: Adaptive Sampling Towards Fast Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9627
    sort_std: 0.0032
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Full
    model_key: full
    model_plain: Full
    value: 0.9568
    std: 0.0069
    paper_value: 0.9568
    paper_std: 0.0069
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
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-01'
    value_gap_source_date_label: NeurIPS 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9568
    true_std: 0.0069
    value_gap_source_arxiv: '1809.05343'
    value_gap_source_title: Adaptive Sampling Towards Fast Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9568
    sort_std: 0.0069
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node-Wise
    model_key: node-wise
    model_plain: Node-Wise
    value: 0.9449
    std: 0.0026
    paper_value: 0.9449
    paper_std: 0.0026
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
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-01'
    value_gap_source_date_label: NeurIPS 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9449
    true_std: 0.0026
    value_gap_source_arxiv: '1809.05343'
    value_gap_source_title: Adaptive Sampling Towards Fast Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9449
    sort_std: 0.0026
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.92
    std: 0.005
    paper_value: 0.92
    paper_std: 0.005
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
    source_ref: chen 2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-07-25'
    value_gap_source_date_label: KDD 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.937
    true_std: 0.0
    value_gap_source_arxiv: '2107.11789'
    value_gap_source_title: 'ROD: Reception-aware Online Distillation for Sparse Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.017000000000000015
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: 0.0
    global_rank: 82
    paper_rank: 100
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IID
    model_key: iid
    model_plain: IID
    value: 0.8611
    std: 0.0437
    paper_value: 0.8611
    paper_std: 0.0437
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
    protocol_note: Standard inductive node classification on Reddit
    date: Sep 1, 2018
    date_display: Sep 2018
    date_iso: '2018-09-01'
    published_venue: NeurIPS 2018
    published_conference: NeurIPS 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-09-01'
    value_gap_source_date_label: NeurIPS 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8611
    true_std: 0.0437
    value_gap_source_arxiv: '1809.05343'
    value_gap_source_title: Adaptive Sampling Towards Fast Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8611
    sort_std: 0.0437
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.824
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
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_display: Mar 2022
    date_iso: '2022-03-02'
    venue: USENIX Security Symposium
    codebase_url: https://github.com/sisaman/GAP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 143
    sort_value: 0.824
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: Reddit
      dataset_slug: reddit
main_figure: /figures/1809.05343/main_figure.jpegoptim.jpg
---

