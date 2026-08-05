---
title: 'Rethinking and Accelerating Graph Condensation: A Training-Free Approach with
  Class Partition'
arxiv_id: '2405.13707'
source_url: ''
authors:
- name: Xinyi Gao
  orcid: null
  s2_author_id: '2192083394'
  s2_url: null
- name: Guanhua Ye
  orcid: null
  s2_author_id: '1849611'
  s2_url: null
- name: Tong Chen
  orcid: null
  s2_author_id: '2280284086'
  s2_url: null
- name: Wentao Zhang
  orcid: null
  s2_author_id: '2280283715'
  s2_url: null
- name: Junliang Yu
  orcid: null
  s2_author_id: '28584977'
  s2_url: null
- name: Hongzhi Yin
  orcid: null
  s2_author_id: '2267513105'
  s2_url: null
published_date: May 22, 2024
published_date_iso: '2024-05-22'
published_venue: WWW 2024
published_conference: WWW 2024
published_conference_short: WWW
published_conference_slug: www
abstract: 'The increasing prevalence of large-scale graphs poses a significant challenge
  for graph neural network training, attributed to their substantial computational
  requirements. In response, graph condensation (GC) emerges as a promising data-centric
  solution aiming to substitute the large graph with a small yet informative condensed
  graph to facilitate data-efficient GNN training. However, existing GC methods suffer
  from intricate optimization processes, necessitating excessive computing resources
  and training time. In this paper, we revisit existing GC optimization strategies
  and identify two pervasive issues therein: (1) various GC optimization strategies
  converge to coarse-grained class-level node feature matching between the original
  and condensed graphs; (2) existing GC methods rely on a Siamese graph network architecture
  that requires time-consuming bi-level optimization with iterative gradient computations.
  To overcome these issues, we propose a training-free GC framework termed Class-partitioned
  Graph Condensation (CGC), which refines the node distribution matching from the
  class-to-class paradigm into a novel class-to-node paradigm, transforming the GC
  optimization into a class partition problem which can be efficiently solved by any
  clustering methods. Moreover, CGC incorporates a pre-defined graph structure to
  enable a closed-form solution for condensed node features, eliminating the need
  for back-and-forth gradient descent in existing GC approaches. Extensive experiments
  demonstrate that CGC achieves an exceedingly efficient condensation process with
  advanced accuracy. Compared with the state-of-the-art GC methods, CGC condenses
  the Ogbn-products graph within 30 seconds, achieving a speedup ranging from $10^2
  $ to $10^4 $ and increasing accuracy by up to 4.2\'
codebase_url: https://github.com/XYGaoG/CGC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CGC
mrr: 0.0
adjusted_mrr: 0.0
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
  - model: TinyGraph
    model_key: ne-asgcn
    model_plain: TinyGraph
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
    global_rank: 1
    sort_value: 0.9758
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TinyGraph
    model_key: hsgt
    model_plain: TinyGraph
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
    global_rank: 2
    sort_value: 0.973
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TinyGraph
    model_key: gcmae
    model_plain: TinyGraph
    value: 0.9713
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.15523'
    title: Generative and Contrastive Paradigms Are Complementary for Graph Self-Supervised
      Learning
    date: Oct 24, 2023
    date_display: Oct 2023
    date_iso: '2023-10-24'
    venue: IEEE International Conference on Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9713
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimDM
    model_key: simdm
    model_plain: SimDM
    value: 0.906
    std: 0.001
    paper_value: 0.906
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
    protocol_note: Accuracy on condensed graph using GCN
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.906
    true_std: 0.001
    value_gap_source_arxiv: '2405.13707'
    value_gap_source_title: 'Rethinking and Accelerating Graph Condensation: A Training-Free
      Approach with Class Partition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.906
    sort_std: 0.001
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCDM
    model_key: gcdm
    model_plain: GCDM
    value: 0.897
    std: 0.002
    paper_value: 0.897
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
    source_ref: liu2022graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on condensed graph using GCN
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.808
    at_pub_std: 0.031
    at_pub_source_arxiv: '2401.12231'
    at_pub_source_title: Disentangled Condensation for Large-scale Graphs
    at_pub_source_date_iso: '2024-01-18'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.08899999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: 0.002
    value_gap_source_arxiv: '2405.13707'
    value_gap_source_title: 'Rethinking and Accelerating Graph Condensation: A Training-Free
      Approach with Class Partition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: 0.002
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Disentangled Condensation for Large-scale Graphs
    comparison_source_arxiv: '2401.12231'
    is_best: false
    is_std_outlier: false
  - model: GCDM-X
    model_key: gcdm-x
    model_plain: GCDM-X
    value: 0.872
    std: 0.001
    paper_value: 0.872
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
    source_ref: liu2022graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on condensed graph using GCN
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.872
    true_std: 0.001
    value_gap_source_arxiv: '2405.13707'
    value_gap_source_title: 'Rethinking and Accelerating Graph Condensation: A Training-Free
      Approach with Class Partition'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.001
    global_rank: 128
    paper_rank: 128
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
single_proposed_model: CGC
main_figure: /figures/2405.13707/main_figure.jpegoptim.jpg
---

