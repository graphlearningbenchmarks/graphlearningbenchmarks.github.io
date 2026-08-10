---
title: 'EXGC: Bridging Efficiency and Explainability in Graph Condensation'
arxiv_id: '2402.05962'
source_url: ''
authors:
- name: Junfeng Fang
  orcid: null
  s2_author_id: '2159830802'
  s2_url: null
- name: Xinglin Li
  orcid: null
  s2_author_id: '2274737326'
  s2_url: null
- name: Yongduo Sui
  orcid: null
  s2_author_id: '2003767516'
  s2_url: null
- name: Yuan Gao
  orcid: null
  s2_author_id: '2283847842'
  s2_url: null
- name: Guibin Zhang
  orcid: null
  s2_author_id: '2232926268'
  s2_url: null
- name: Kun Wang
  orcid: null
  s2_author_id: '2283296635'
  s2_url: null
- name: Xiang Wang
  orcid: null
  s2_author_id: '2283443460'
  s2_url: null
- name: Xiangnan He
  orcid: null
  s2_author_id: '2240825631'
  s2_url: null
published_date: Feb 5, 2024
published_date_iso: '2024-02-05'
published_venue: WWW 2024
published_conference: WWW 2024
published_conference_short: WWW
published_conference_slug: www
abstract: 'Graph representation learning on vast datasets, like web data, has made
  significant strides. However, the associated computational and storage overheads
  raise concerns. In sight of this, Graph condensation (GCond) has been introduced
  to distill these large real datasets into a more concise yet information-rich synthetic
  graph. Despite acceleration efforts, existing GCond methods mainly grapple with
  efficiency, especially on expansive web data graphs. Hence, in this work, we pinpoint
  two major inefficiencies of current paradigms: (1) the concurrent updating of a
  vast parameter set, and (2) pronounced parameter redundancy. To counteract these
  two limitations correspondingly, we first (1) employ the Mean-Field variational
  approximation for convergence acceleration, and then (2) propose the objective of
  Gradient Information Bottleneck (GDIB) to prune redundancy. By incorporating the
  leading explanation techniques (e.g., GNNExplainer and GSAT) to instantiate the
  GDIB, our EXGC, the Efficient and eXplainable Graph Condensation method is proposed,
  which can markedly boost efficiency and inject explainability. Our extensive evaluations
  across eight datasets underscore EXGC''s superiority and relevance. Code is available
  at.'
codebase_url: https://github.com/MangoKiller/EXGC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- EXGC-X
- EXGC
mrr: 0.0033
adjusted_mrr: 0.0033
mrr_dataset_count: 3
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 3
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
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
    value: 0.8774
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
  - model: Full Graph
    model_key: full graph
    model_plain: Full Graph
    value: 0.7112
    std: 0.0006
    paper_value: 0.7112
    paper_std: 0.0006
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7112
    true_std: 0.0006
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7112
    sort_std: 0.0006
    global_rank: 612
    paper_rank: 612
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.6398
    std: 0.0431
    paper_value: 0.6398
    paper_std: 0.0431
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.706
    at_pub_std: null
    at_pub_source_arxiv: '2206.07746'
    at_pub_source_title: Condensing Graphs via One-Step Gradient Matching
    at_pub_source_date_iso: '2022-06-15'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06619999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.708
    true_std: 0.045
    value_gap_source_arxiv: '2407.08064'
    value_gap_source_title: 'TinyGraph: Joint Feature and Node Condensation for Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.06819999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.708
    sort_std: 0.045
    global_rank: 634
    paper_rank: 862
    rank_delta: 228
    rank_delta_abs: 228
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Condensing Graphs via One-Step Gradient Matching
    comparison_source_arxiv: '2206.07746'
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.3387
    std: 0.0082
    paper_value: 0.3387
    paper_std: 0.0082
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.7049
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2206.09166'
    at_pub_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    at_pub_source_date_iso: '2022-06-18'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-06-18'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.36619999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7049
    true_std: 0.0008
    value_gap_source_arxiv: '2206.09166'
    value_gap_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    value_gap_source_is_current_paper: false
    value_gap: 0.36619999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7049
    sort_std: 0.0008
    global_rank: 653
    paper_rank: 973
    rank_delta: 320
    rank_delta_abs: 320
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture
      Search'
    comparison_source_arxiv: '2206.09166'
    is_best: false
    is_std_outlier: false
  - model: EXGC
    model_key: exgc
    model_plain: EXGC
    value: 0.6916
    std: 0.02
    paper_value: 0.6916
    paper_std: 0.02
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6916
    true_std: 0.02
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6916
    sort_std: 0.02
    global_rank: 712
    paper_rank: 712
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: K-Center
    model_key: k-center
    model_plain: K-Center
    value: 0.3403
    std: 0.0252
    paper_value: 0.3403
    paper_std: 0.0252
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.691
    true_std: 0.001
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.35069999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.691
    sort_std: 0.001
    global_rank: 714
    paper_rank: 973
    rank_delta: 259
    rank_delta_abs: 259
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.3131
    std: 0.012
    paper_value: 0.3131
    paper_std: 0.012
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.69
    true_std: 0.001
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.37689999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.69
    sort_std: 0.001
    global_rank: 716
    paper_rank: 975
    rank_delta: 259
    rank_delta_abs: 259
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EXGC-X
    model_key: exgc-x
    model_plain: EXGC-X
    value: 0.6782
    std: 0.0131
    paper_value: 0.6782
    paper_std: 0.0131
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6782
    true_std: 0.0131
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6782
    sort_std: 0.0131
    global_rank: 761
    paper_rank: 761
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond-X
    model_key: gcond-x
    model_plain: GCond-X
    value: 0.6413
    std: 0.0183
    paper_value: 0.6413
    paper_std: 0.0183
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) for node classification
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6413
    true_std: 0.0183
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6413
    sort_std: 0.0183
    global_rank: 857
    paper_rank: 857
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
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9004
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
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 31
    sort_value: 0.9004
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.3704
    std: 0.0741
    paper_value: 0.3704
    paper_std: 0.0741
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.8699
    at_pub_std: 0.006
    at_pub_source_arxiv: '2112.14531'
    at_pub_source_title: 'Designing the Topology of Graph Neural Networks: A Novel
      Feature Fusion Perspective'
    at_pub_source_date_iso: '2021-12-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-12-29'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.4995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8699
    true_std: 0.006
    value_gap_source_arxiv: '2112.14531'
    value_gap_source_title: 'Designing the Topology of Graph Neural Networks: A Novel
      Feature Fusion Perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.4995
    has_value_note: false
    value_note: ''
    sort_value: 0.8699
    sort_std: 0.006
    global_rank: 192
    paper_rank: 1001
    rank_delta: 809
    rank_delta_abs: 809
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Designing the Topology of Graph Neural Networks: A Novel
      Feature Fusion Perspective'
    comparison_source_arxiv: '2112.14531'
    is_best: false
    is_std_outlier: false
  - model: EXGC
    model_key: exgc
    model_plain: EXGC
    value: 0.8202
    std: 0.0042
    paper_value: 0.8202
    paper_std: 0.0042
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8202
    true_std: 0.0042
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8202
    sort_std: 0.0042
    global_rank: 610
    paper_rank: 610
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EXGC-X
    model_key: exgc-x
    model_plain: EXGC-X
    value: 0.8091
    std: 0.0039
    paper_value: 0.8091
    paper_std: 0.0039
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8091
    true_std: 0.0039
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8091
    sort_std: 0.0039
    global_rank: 701
    paper_rank: 701
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Full Graph
    model_key: full graph
    model_plain: Full Graph
    value: 0.8091
    std: 0.001
    paper_value: 0.8091
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8091
    true_std: 0.001
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8091
    sort_std: 0.001
    global_rank: 702
    paper_rank: 702
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.7276
    std: 0.0045
    paper_value: 0.7276
    paper_std: 0.0045
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.809
    true_std: 0.032
    value_gap_source_arxiv: '2407.08064'
    value_gap_source_title: 'TinyGraph: Joint Feature and Node Condensation for Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.08140000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.809
    sort_std: 0.032
    global_rank: 703
    paper_rank: 881
    rank_delta: 178
    rank_delta_abs: 178
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7768
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 806
    sort_value: 0.7768
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.4347
    std: 0.0055
    paper_value: 0.4347
    paper_std: 0.0055
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.768
    at_pub_std: 0.001
    at_pub_source_arxiv: '2310.11046'
    at_pub_source_title: Fast Graph Condensation with Structure-based Neural Tangent
      Kernel
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.33330000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.768
    true_std: 0.001
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.33330000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.768
    sort_std: 0.001
    global_rank: 824
    paper_rank: 999
    rank_delta: 175
    rank_delta_abs: 175
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Condensation with Structure-based Neural Tangent
      Kernel
    comparison_source_arxiv: '2310.11046'
    is_best: false
    is_std_outlier: false
  - model: K-Center
    model_key: k-center
    model_plain: K-Center
    value: 0.4633
    std: 0.0324
    paper_value: 0.4633
    paper_std: 0.0324
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.767
    at_pub_std: 0.001
    at_pub_source_arxiv: '2310.11046'
    at_pub_source_title: Fast Graph Condensation with Structure-based Neural Tangent
      Kernel
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3037
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.767
    true_std: 0.001
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.3037
    has_value_note: false
    value_note: ''
    sort_value: 0.767
    sort_std: 0.001
    global_rank: 825
    paper_rank: 996
    rank_delta: 171
    rank_delta_abs: 171
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Condensation with Structure-based Neural Tangent
      Kernel
    comparison_source_arxiv: '2310.11046'
    is_best: false
    is_std_outlier: false
  - model: GCond-X
    model_key: gcond-x
    model_plain: GCond-X
    value: 0.691
    std: 0.0031
    paper_value: 0.691
    paper_std: 0.0031
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
      for node classification.
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.691
    true_std: 0.0031
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.691
    sort_std: 0.0031
    global_rank: 912
    paper_rank: 912
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
    global_rank: 18
    sort_value: 0.966
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Full Graph
    model_key: full graph
    model_plain: Full Graph
    value: 0.9396
    std: 0.0003
    paper_value: 0.9396
    paper_std: 0.0003
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
    protocol_note: Test performance on Reddit inductive split with 0.1% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9396
    true_std: 0.0003
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9396
    sort_std: 0.0003
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EXGC
    model_key: exgc
    model_plain: EXGC
    value: 0.9184
    std: 0.0073
    paper_value: 0.9184
    paper_std: 0.0073
    metric: F1
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9184
    true_std: 0.0073
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9184
    sort_std: 0.0073
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EXGC-X
    model_key: exgc-x
    model_plain: EXGC-X
    value: 0.9173
    std: 0.0052
    paper_value: 0.9173
    paper_std: 0.0052
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9173
    true_std: 0.0052
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9173
    sort_std: 0.0052
    global_rank: 141
    paper_rank: 141
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond-X
    model_key: gcond-x
    model_plain: GCond-X
    value: 0.9114
    std: 0.0059
    paper_value: 0.9114
    paper_std: 0.0059
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9114
    true_std: 0.0059
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9114
    sort_std: 0.0059
    global_rank: 144
    paper_rank: 144
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.9106
    std: 0.0093
    paper_value: 0.9106
    paper_std: 0.0093
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9106
    true_std: 0.0093
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9106
    sort_std: 0.0093
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.7868
    std: 0.0094
    paper_value: 0.7868
    paper_std: 0.0094
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7868
    true_std: 0.0094
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7868
    sort_std: 0.0094
    global_rank: 157
    paper_rank: 157
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
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.6992
    std: 0.0232
    paper_value: 0.6992
    paper_std: 0.0232
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: 0.043
    at_pub_std: null
    at_pub_source_arxiv: '1706.02216'
    at_pub_source_title: Inductive Representation Learning on Large Graphs
    at_pub_source_date_iso: '2017-06-07'
    at_pub_source_date_label: NeurIPS 2017
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.6562
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6992
    true_std: 0.0232
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6992
    sort_std: 0.0232
    global_rank: 164
    paper_rank: 164
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Inductive Representation Learning on Large Graphs
    comparison_source_arxiv: '1706.02216'
    is_best: false
    is_std_outlier: false
  - model: K-Center
    model_key: k-center
    model_plain: K-Center
    value: 0.6014
    std: 0.0184
    paper_value: 0.6014
    paper_std: 0.0184
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
    protocol_note: Test performance on Reddit inductive split with 0.5% ratio
    date: Feb 5, 2024
    date_display: Feb 2024
    date_iso: '2024-02-05'
    published_venue: WWW 2024
    published_conference: WWW 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-05'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6014
    true_std: 0.0184
    value_gap_source_arxiv: '2402.05962'
    value_gap_source_title: 'EXGC: Bridging Efficiency and Explainability in Graph
      Condensation'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6014
    sort_std: 0.0184
    global_rank: 169
    paper_rank: 169
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
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Reddit
      dataset_slug: reddit
main_figure: /figures/2402.05962/main_figure.jpegoptim.jpg
---

