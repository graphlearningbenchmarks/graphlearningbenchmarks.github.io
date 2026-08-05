---
title: Pre-Training Graph Neural Networks for Generic Structural Feature Extraction
arxiv_id: '1905.13728'
source_url: ''
authors:
- name: Ziniu Hu
  orcid: null
  s2_author_id: '3407296'
  s2_url: null
- name: Changjun Fan
  orcid: null
  s2_author_id: '1729964'
  s2_url: null
- name: Ting Chen
  orcid: null
  s2_author_id: '145358498'
  s2_url: null
- name: Kai-Wei Chang
  orcid: null
  s2_author_id: '2782886'
  s2_url: null
- name: Yizhou Sun
  orcid: null
  s2_author_id: '2367272188'
  s2_url: null
published_date: May 31, 2019
published_date_iso: '2019-05-31'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph neural networks (GNNs) are shown to be successful in modeling applications
  with graph structures. However, training an accurate GNN model requires a large
  collection of labeled data and expressive features, which might be inaccessible
  for some applications. To tackle this problem, we propose a pre-training framework
  that captures generic graph structural information that is transferable across tasks.
  Our framework can leverage the following three tasks: 1) denoising link reconstruction,
  2) centrality score ranking, and 3) cluster preserving. The pre-training procedure
  can be conducted purely on the synthetic graphs, and the pre-trained GNN is then
  adapted for downstream applications. With the proposed pre-training procedure, the
  generic structural information is learned and preserved, thus the pre-trained GNN
  requires less amount of labeled data and fewer domain-specific features to achieve
  high performance on different downstream tasks. Comprehensive experiments demonstrate
  that our proposed framework can significantly enhance the performance of various
  tasks at the level of node, link, and graph.'
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
  evaluated: 2
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.8894
    std: 0.0054
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_display: Feb 2024
    date_iso: '2024-02-08'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8894
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.888
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
    feature_source_evidence: APPNP is a standard GNN.
    is_global_top: true
    global_rank: 2
    sort_value: 0.888
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.881
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
    feature_source_evidence: GraphSAGE is a standard GNN that pools node attributes.
    is_global_top: true
    global_rank: 3
    sort_value: 0.881
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.879
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
    feature_source_evidence: GCN is a standard GNN that pools node attributes.
    is_global_top: true
    global_rank: 6
    sort_value: 0.879
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Pre-train (Cluster)
    model_key: pre-train (cluster)
    model_plain: Pre-train (Cluster)
    value: 0.679
    std: 0.008
    paper_value: 0.679
    paper_std: 0.008
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split);
      results reported in F1-score.
    date: May 31, 2019
    date_display: May 2019
    date_iso: '2019-05-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-31'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.679
    true_std: 0.008
    value_gap_source_arxiv: '1905.13728'
    value_gap_source_title: Pre-Training Graph Neural Networks for Generic Structural
      Feature Extraction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.679
    sort_std: 0.008
    global_rank: 42
    paper_rank: 42
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
    value: 0.657
    std: 0.019
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2103.14991'
    title: Graph Unlearning
    date: Mar 27, 2021
    date_display: Mar 2021
    date_iso: '2021-03-27'
    venue: Conference on Computer and Communications Security
    codebase_url: https://github.com/MinChen00/Graph-Unlearning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 43
    sort_value: 0.657
    sort_std: 0.019
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
- &id002
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
    value: 0.884
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
    global_rank: 2
    sort_value: 0.884
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.875
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
    global_rank: 3
    sort_value: 0.875
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.864
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
    global_rank: 6
    sort_value: 0.864
    sort_std: 0.001
    comparison_type: global_top
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
  - model: Pre-train (All Tasks)
    model_key: pre-train (all tasks)
    model_plain: Pre-train (All Tasks)
    value: 0.66
    std: 0.014
    paper_value: 0.66
    paper_std: 0.014
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) as per canonical definition;
      task is node classification.
    date: May 31, 2019
    date_display: May 2019
    date_iso: '2019-05-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-31'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.66
    true_std: 0.014
    value_gap_source_arxiv: '1905.13728'
    value_gap_source_title: Pre-Training Graph Neural Networks for Generic Structural
      Feature Extraction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.66
    sort_std: 0.014
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
main_figure: /figures/1905.13728/main_figure.jpegoptim.jpg
---

