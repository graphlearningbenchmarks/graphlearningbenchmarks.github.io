---
title: Leveraging Invariant Principle for Heterophilic Graph Structure Distribution
  Shifts
arxiv_id: '2408.09490'
source_url: ''
authors:
- name: Jinluan Yang
  orcid: null
  s2_author_id: '2275639981'
  s2_url: null
- name: Zhengyu Chen
  orcid: null
  s2_author_id: '2255052567'
  s2_url: null
- name: Teng Xiao
  orcid: null
  s2_author_id: '2256584990'
  s2_url: null
- name: Yong Lin
  orcid: null
  s2_author_id: '2316443015'
  s2_url: null
- name: Wenqiao Zhang
  orcid: null
  s2_author_id: '2273572940'
  s2_url: null
- name: Kun Kuang
  orcid: null
  s2_author_id: '2272718198'
  s2_url: null
published_date: Aug 18, 2024
published_date_iso: '2024-08-18'
published_venue: WWW 2024
published_conference: WWW 2024
published_conference_short: WWW
published_conference_slug: www
abstract: Heterophilic Graph Neural Networks (HGNNs) have shown promising results
  for semi-supervised learning tasks on graphs. Notably, most real-world heterophilic
  graphs are composed of a mixture of nodes with different neighbor patterns, exhibiting
  local node-level homophilic and heterophilic structures. However, existing works
  are only devoted to designing better unified HGNN backbones for node classification
  tasks on heterophilic and homophilic graphs simultaneously, and their analyses of
  HGNN performance concerning nodes are only based on the determined data distribution
  without exploring the effect caused by the difference of structural pattern between
  training and testing nodes. How to learn invariant node representations on heterophilic
  graphs to handle this structure difference or distribution shifts remains unexplored.
  In this paper, we first discuss the limitations of previous graph-based invariant
  learning methods in addressing the heterophilic graph structure distribution shifts
  from the perspective of data augmentation. Then, we propose HEI, a framework capable
  of generating invariant node representations through incorporating Heterophily information,
  the node's estimated neighbor pattern, to infer latent Environments without augmentation,
  which are then used for Invariant prediction. We provide detailed theoretical guarantees
  to clarify the reasonability of HEI. Extensive experiments on various benchmarks
  and backbones can also demonstrate the effectiveness and robustness of our method
  compared with existing state-of-the-art baselines.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- HEI
mrr: 0.0667
adjusted_mrr: 0.0222
mrr_dataset_count: 1
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Actor
  rows:
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7623
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7623
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiGGR
    model_key: diggr
    model_plain: DiGGR
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TRIGON
    model_key: trigon
    model_plain: TRIGON
    value: 0.4402
    std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.19071'
    title: Dynamic Triangulation-Based Graph Rewiring for Graph Neural Networks
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Hugo-Attali/TRIGON-CIKM-2025
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HEI
    model_key: hei
    model_plain: HEI
    value: 0.4225
    std: 0.0159
    paper_value: 0.4225
    paper_std: 0.0159
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset (GloGNN++ backbone)
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4225
    true_std: 0.0159
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4225
    sort_std: 0.0159
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CaNet
    model_key: canet
    model_plain: CaNet
    value: 0.4158
    std: 0.0132
    paper_value: 0.4158
    paper_std: 0.0132
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4158
    true_std: 0.0132
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4158
    sort_std: 0.0132
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
  - model: IENE
    model_key: iene
    model_plain: IENE
    value: 0.4158
    std: 0.0137
    paper_value: 0.4158
    paper_std: 0.0137
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4158
    true_std: 0.0137
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4158
    sort_std: 0.0137
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
  - model: FLOOD
    model_key: flood
    model_plain: FLOOD
    value: 0.4154
    std: 0.0134
    paper_value: 0.4154
    paper_std: 0.0134
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4154
    true_std: 0.0134
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4154
    sort_std: 0.0134
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BAGNN
    model_key: bagnn
    model_plain: BAGNN
    value: 0.4126
    std: 0.0152
    paper_value: 0.4126
    paper_std: 0.0152
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4126
    true_std: 0.0152
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4126
    sort_std: 0.0152
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.4096
    std: 0.0152
    paper_value: 0.4096
    paper_std: 0.0152
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4096
    true_std: 0.0152
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4096
    sort_std: 0.0152
    global_rank: 44
    paper_rank: 44
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
    value: 0.4026
    std: 0.0108
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 55
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.3934
    std: 0.0321
    paper_value: 0.3934
    paper_std: 0.0321
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.2765
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2310.00800'
    at_pub_source_title: 'GraphPatcher: Mitigating Degree Bias for Graph Neural Networks
      via Test-time Augmentation'
    at_pub_source_date_iso: '2023-10-01'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.1169
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3934
    true_std: 0.0321
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3934
    sort_std: 0.0321
    global_rank: 79
    paper_rank: 79
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GraphPatcher: Mitigating Degree Bias for Graph Neural
      Networks via Test-time Augmentation'
    comparison_source_arxiv: '2310.00800'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3899
    std: 0.0085
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
    global_rank: 87
    sort_value: 0.3899
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SRGNN
    model_key: srgnn
    model_plain: SRGNN
    value: 0.3562
    std: 0.0275
    paper_value: 0.3562
    paper_std: 0.0275
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3562
    true_std: 0.0275
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3562
    sort_std: 0.0275
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
  - model: StruRW-Mixup
    model_key: strurw-mixup
    model_plain: StruRW-Mixup
    value: 0.3545
    std: 0.0279
    paper_value: 0.3545
    paper_std: 0.0279
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3545
    true_std: 0.0279
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3545
    sort_std: 0.0279
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
  - model: ReNode
    model_key: renode
    model_plain: ReNode
    value: 0.3542
    std: 0.0275
    paper_value: 0.3542
    paper_std: 0.0275
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: High Hom Test split on Actor dataset
    date: Aug 18, 2024
    date_display: Aug 2024
    date_iso: '2024-08-18'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3542
    true_std: 0.0275
    value_gap_source_arxiv: '2408.09490'
    value_gap_source_title: Leveraging Invariant Principle for Heterophilic Graph
      Structure Distribution Shifts
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3542
    sort_std: 0.0275
    global_rank: 258
    paper_rank: 258
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
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
single_proposed_model: HEI
main_figure: /figures/2408.09490/main_figure.jpegoptim.jpg
---

