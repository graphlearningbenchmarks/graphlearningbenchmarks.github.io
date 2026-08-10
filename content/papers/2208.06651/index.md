---
title: Revisiting Adversarial Attacks on Graph Neural Networks for Graph Classification
arxiv_id: '2208.06651'
source_url: ''
authors:
- name: Beini Xie
  orcid: null
  s2_author_id: '2181504062'
  s2_url: null
- name: Heng Chang
  orcid: null
  s2_author_id: '144188238'
  s2_url: null
- name: Xin Wang
  orcid: null
  s2_author_id: '153316152'
  s2_url: null
- name: Tian Bian
  orcid: null
  s2_author_id: '46208160'
  s2_url: null
- name: Shiji Zhou
  orcid: null
  s2_author_id: '2149195194'
  s2_url: null
- name: Daixin Wang
  orcid: null
  s2_author_id: '2057764'
  s2_url: null
- name: Zhiqiang Zhang
  orcid: null
  s2_author_id: '2144443017'
  s2_url: null
- name: Wenwu Zhu
  orcid: null
  s2_author_id: '2156154955'
  s2_url: null
published_date: Aug 13, 2022
published_date_iso: '2022-08-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) have achieved tremendous success in the task
  of graph classification and its diverse downstream real-world applications. Despite
  the huge success in learning graph representations, current GNN models have demonstrated
  their vulnerability to potentially existent adversarial examples on graph-structured
  data. Existing approaches are either limited to structure attacks or restricted
  to local information, urging for the design of a more general attack framework on
  graph classification, which faces significant challenges due to the complexity of
  generating local-node-level adversarial examples using the global-graph-level information.
  To address this "global-to-local" attack challenge, we present a novel and general
  framework CAMA to generate adversarial examples via manipulating graph structure
  and node features. Specifically, we make use of Graph Class Activation Mapping and
  its variant to produce node-level importance corresponding to the graph classification
  task. Then through a heuristic design of algorithms, we can perform both feature
  and structure attacks under unnoticeable perturbation budgets with the help of both
  node-level and subgraph-level importance. Experiments towards attacking four state-of-the-art
  graph classification models on six real-world benchmarks verify the flexibility
  and effectiveness of our framework.
codebase_url: ''
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: IMDB-BINARY
  rows:
  - model: GCFL
    model_key: gcfl
    model_plain: GCFL
    value: 0.8299
    std: 0.052
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8299
    sort_std: 0.052
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.815
    std: 0.024
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
    sort_value: 0.815
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN+BEC
    model_key: gin+bec
    model_plain: GIN+BEC
    value: 0.808
    std: 0.033
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
    global_rank: 3
    sort_value: 0.808
    sort_std: 0.033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.798
    std: 0.023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 5
    sort_value: 0.798
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Clean
    model_key: clean
    model_plain: Clean
    value: 0.7367
    std: null
    paper_value: 0.7367
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: For social networks, node features are initialized with
      the node degree.
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on IMDB-BINARY using 10-fold CV as per canonical task
      description.
    date: Aug 13, 2022
    date_display: Aug 2022
    date_iso: '2022-08-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-08-13'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7367
    true_std: null
    value_gap_source_arxiv: '2208.06651'
    value_gap_source_title: Revisiting Adversarial Attacks on Graph Neural Networks
      for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7367
    sort_std: null
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: IMDB-BINARY
      dataset_slug: imdb-binary
main_figure: /figures/2208.06651/main_figure.jpegoptim.jpg
---

