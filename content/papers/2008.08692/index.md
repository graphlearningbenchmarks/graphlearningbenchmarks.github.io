---
title: Enhancing Graph Neural Network-based Fraud Detectors against Camouflaged Fraudsters
arxiv_id: '2008.08692'
source_url: ''
authors:
- name: Yingtong Dou
  orcid: null
  s2_author_id: '8729899'
  s2_url: null
- name: Zhiwei Liu
  orcid: null
  s2_author_id: '1844299386'
  s2_url: null
- name: Li Sun
  orcid: null
  s2_author_id: '71838843'
  s2_url: null
- name: Yutong Deng
  orcid: null
  s2_author_id: '1666175769'
  s2_url: null
- name: Hao Peng
  orcid: null
  s2_author_id: '49349645'
  s2_url: null
- name: Philip S. Yu
  orcid: null
  s2_author_id: '144019071'
  s2_url: null
published_date: Aug 19, 2020
published_date_iso: '2020-08-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) have been widely applied to fraud detection
  problems in recent years, revealing the suspiciousness of nodes by aggregating their
  neighborhood information via different relations. However, few prior works have
  noticed the camouflage behavior of fraudsters, which could hamper the performance
  of GNN-based fraud detectors during the aggregation process. In this paper, we introduce
  two types of camouflages based on recent empirical studies, i.e., the feature camouflage
  and the relation camouflage. Existing GNNs have not addressed these two camouflages,
  which results in their poor performance in fraud detection problems. Alternatively,
  we propose a new model named CAmouflage-REsistant GNN (CARE-GNN), to enhance the
  GNN aggregation process with three unique modules against camouflages. Concretely,
  we first devise a label-aware similarity measure to find informative neighboring
  nodes. Then, we leverage reinforcement learning (RL) to find the optimal amounts
  of neighbors to be selected. Finally, the selected neighbors across different relations
  are aggregated together. Comprehensive experiments on two real-world fraud datasets
  demonstrate the effectiveness of the RL algorithm. The proposed CARE-GNN also outperforms
  state-of-the-art GNNs and GNN-based fraud detectors. We integrate all GNN-based
  fraud detectors as an opensource toolbox. The CARE-GNN code and datasets are available
  at.
codebase_url: https://github.com/YingtongDou/CARE-GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CARE-Att
- CARE-Weight
- CARE-Mean
- CARE-GNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon2M
  rows:
  - model: GraphConsis
    model_key: gfd
    model_plain: GraphConsis
    value: 0.9757
    std: 0.0012
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9757
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphConsis
    model_key: bwgnn
    model_plain: GraphConsis
    value: 0.9742
    std: 0.0048
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9742
    sort_std: 0.0048
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphConsis
    model_key: gdn
    model_plain: GraphConsis
    value: 0.9709
    std: 0.0016
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9709
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7527
    std: null
    paper_value: 0.7527
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9316
    true_std: 0.0087
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.17889999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9316
    sort_std: 0.0087
    global_rank: 9
    paper_rank: 22
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CARE-GNN
    model_key: care-gnn
    model_plain: CARE-GNN
    value: 0.8973
    std: null
    paper_value: 0.8973
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9067
    true_std: 0.0149
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.009399999999999964
    has_value_note: false
    value_note: ''
    sort_value: 0.9067
    sort_std: 0.0149
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CARE-Att
    model_key: care-att
    model_plain: CARE-Att
    value: 0.897
    std: null
    paper_value: 0.897
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: null
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
  - model: CARE-Weight
    model_key: care-weight
    model_plain: CARE-Weight
    value: 0.8969
    std: null
    paper_value: 0.8969
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8969
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8969
    sort_std: null
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CARE-Mean
    model_key: care-mean
    model_plain: CARE-Mean
    value: 0.8952
    std: null
    paper_value: 0.8952
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8952
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8952
    sort_std: null
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7525
    std: null
    paper_value: 0.7525
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 10% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8667
    true_std: null
    value_gap_source_arxiv: '2401.14155'
    value_gap_source_title: Alleviating Structural Distribution Shift in Graph Anomaly
      Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.11420000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8667
    sort_std: null
    global_rank: 15
    paper_rank: 22
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphConsis
    model_key: graphconsis
    model_plain: GraphConsis
    value: 0.855
    std: null
    paper_value: 0.855
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: liu2020alleviating
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 20% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.855
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.855
    sort_std: null
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7516
    std: null
    paper_value: 0.7516
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8102
    true_std: 0.0179
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.058599999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.8102
    sort_std: 0.0179
    global_rank: 18
    paper_rank: 22
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Player2Vec
    model_key: player2vec
    model_plain: Player2Vec
    value: 0.7686
    std: null
    paper_value: 0.7686
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: zhang2019key
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 5% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7686
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7686
    sort_std: null
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SemiGNN
    model_key: semignn
    model_plain: SemiGNN
    value: 0.7621
    std: null
    paper_value: 0.7621
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: wang2019semi
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 10% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7621
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7621
    sort_std: null
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.7558
    std: null
    paper_value: 0.7558
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 20% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7558
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7558
    sort_std: null
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
  - model: GeniePath
    model_key: geniepath
    model_plain: GeniePath
    value: 0.7265
    std: null
    paper_value: 0.7265
    paper_std: null
    metric: AUC
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
    table_ref: Table 3
    source_ref: liu2019geniepath
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised fraud detection on Amazon dataset with 40% training
      split
    date: Aug 19, 2020
    date_display: Aug 2020
    date_iso: '2020-08-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-08-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7265
    true_std: null
    value_gap_source_arxiv: '2008.08692'
    value_gap_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7265
    sort_std: null
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
---

