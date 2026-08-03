---
title: Backdoor Graph Condensation
arxiv_id: '2407.11025'
source_url: ''
authors:
- name: Jiahao Wu
  orcid: null
  s2_author_id: '2109164978'
  s2_url: null
- name: Ning Lu
  orcid: null
  s2_author_id: '2147128045'
  s2_url: null
- name: Z.J. Dai
  orcid: null
  s2_author_id: '2346815031'
  s2_url: null
- name: Wenqi Fan
  orcid: null
  s2_author_id: '2291324376'
  s2_url: null
- name: Shengcai Liu
  orcid: null
  s2_author_id: '2152939552'
  s2_url: null
- name: Qing Li
  orcid: null
  s2_author_id: '2254366521'
  s2_url: null
- name: Ke Tang
  orcid: null
  s2_author_id: '2253405825'
  s2_url: null
published_date: Jul 3, 2024
published_date_iso: '2024-07-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph condensation has recently emerged as a prevalent technique to improve
  the training efficiency for graph neural networks (GNNs). It condenses a large graph
  into a small one such that a GNN trained on this small synthetic graph can achieve
  comparable performance to a GNN trained on the large graph. However, while existing
  graph condensation studies mainly focus on the best trade-off between graph size
  and the GNNs'' performance (model utility), they overlook the security issues of
  graph condensation. To bridge this gap, we first explore backdoor attack against
  the GNNs trained on the condensed graphs. We introduce an effective backdoor attack
  against graph condensation, termed BGC. This attack aims to (1) preserve the condensed
  graph quality despite trigger injection, and (2) ensure trigger efficacy through
  the condensation process, achieving a high attack success rate. Specifically, BGC
  consistently updates triggers during condensation and targets representative nodes
  for poisoning. Extensive experiments demonstrate the effectiveness of our attack.
  BGC achieves a high attack success rate (close to 1.0) and good model utility in
  all cases. Furthermore, the results against multiple defense methods demonstrate
  BGC''s resilience under their defenses. Finally, we analyze the key hyperparameters
  that influence the attack performance. Our code is available at: https://github.com/JiahaoWuGit/BGC.'
codebase_url: https://github.com/JiahaoWuGit/BGC
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
  is_multi_metric: true
  rows:
  - model: GCNII
    model_key: ne-asgcn
    model_plain: GCNII
    metric_values:
    - 0.9758
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
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
    published_venue: ''
    date: Mar 1, 2022
    date_display: Mar 2022
    date_iso: '2022-03-01'
    codebase_url: ''
    uses_external_data: true
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9758
    sort_std: 0.0027
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCNII
    model_key: gcmae
    model_plain: GCNII
    metric_values:
    - 0.9713
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
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
    published_venue: ''
    date: Oct 24, 2023
    date_display: Oct 2023
    date_iso: '2023-10-24'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.9713
    sort_std: 0.0017
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCNII
    model_key: gat+norm.adj.
    model_plain: GCNII
    metric_values:
    - 0.9706
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.13355'
    title: Bag of Tricks for Node Classification with Graph Neural Networks
    published_venue: ''
    date: Mar 24, 2021
    date_display: Mar 2021
    date_iso: '2021-03-24'
    codebase_url: https://github.com/espylapiza/Bag-of-Tricks-for-Node-Classification-with-Graph-Neural-Networks
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9706
    sort_std: 0.0005
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - null
    - 0.9025
    - 0.9985
    metric_stds:
    - null
    - 0.0019
    - 0.0012
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.965
    sort_std: 0.0003
    true_value: 0.965
    true_std: 0.0003
    paper_value: 0.9025
    paper_std: 0.0019
    has_value_gap: true
    has_value_note: false
    value_gap: 0.0625
    value_gap_source_arxiv: '2406.12059'
    value_gap_source_title: A Scalable and Effective Alternative to Graph Transformers
    value_note: ''
    at_pub_value: 0.965
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2406.12059'
    at_pub_source_title: A Scalable and Effective Alternative to Graph Transformers
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: AAAI 2024
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.0625
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: A Scalable and Effective Alternative to Graph Transformers
    comparison_source_arxiv: '2406.12059'
    is_best: false
    is_std_outlier: false
    global_rank: 18
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.9037
    - 0.9999
    metric_stds:
    - null
    - 0.0022
    - 0.0001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9648
    sort_std: null
    true_value: 0.9648
    true_std: null
    paper_value: 0.9037
    paper_std: 0.0022
    has_value_gap: true
    has_value_note: false
    value_gap: 0.06110000000000004
    value_gap_source_arxiv: '1907.10903'
    value_gap_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on
      Node Classification'
    value_note: ''
    at_pub_value: 0.9648
    at_pub_std: null
    at_pub_source_arxiv: '1907.10903'
    at_pub_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on Node
      Classification'
    at_pub_source_date_iso: '2019-07-25'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-07-25'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.06110000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks
      on Node Classification'
    comparison_source_arxiv: '1907.10903'
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    metric_values:
    - null
    - 0.8853
    - 1.0
    metric_stds:
    - null
    - 0.0044
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.95
    sort_std: null
    true_value: 0.95
    true_std: null
    paper_value: 0.8853
    paper_std: 0.0044
    has_value_gap: true
    has_value_note: false
    value_gap: 0.06469999999999998
    value_gap_source_arxiv: '2102.10739'
    value_gap_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    value_note: ''
    at_pub_value: 0.95
    at_pub_std: null
    at_pub_source_arxiv: '2102.10739'
    at_pub_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.06469999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    comparison_source_arxiv: '2102.10739'
    is_best: false
    is_std_outlier: false
    global_rank: 58
  - model: SGC
    model_key: sgc
    model_plain: SGC
    metric_values:
    - null
    - 0.9099
    - 0.9999
    metric_stds:
    - null
    - 0.0022
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.949
    sort_std: null
    true_value: 0.949
    true_std: null
    paper_value: 0.9099
    paper_std: 0.0022
    has_value_gap: true
    has_value_note: false
    value_gap: 0.03909999999999991
    value_gap_source_arxiv: '2102.10739'
    value_gap_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    value_note: ''
    at_pub_value: 0.949
    at_pub_std: 0.012
    at_pub_source_arxiv: '1905.09550'
    at_pub_source_title: 'Revisiting Graph Neural Networks: All We Have is Low-Pass
      Filters'
    at_pub_source_date_iso: '2019-05-23'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.03909999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Revisiting Graph Neural Networks: All We Have is Low-Pass
      Filters'
    comparison_source_arxiv: '1905.09550'
    is_best: false
    is_std_outlier: false
    global_rank: 60
  - model: GCond
    model_key: gcond
    model_plain: GCond
    metric_values:
    - null
    - 0.904
    - 0.9999
    metric_stds:
    - null
    - 0.0041
    - 0.0001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.904
    sort_std: 0.0041
    true_value: 0.904
    true_std: 0.0041
    paper_value: 0.904
    paper_std: 0.0041
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2407.11025'
    value_gap_source_title: Backdoor Graph Condensation
    value_note: ''
    at_pub_value: 0.8963
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2307.15967'
    at_pub_source_title: Graph Condensation for Inductive Node Representation Learning
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00770000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: Graph Condensation for Inductive Node Representation
      Learning
    comparison_source_arxiv: '2307.15967'
    is_best: false
    is_std_outlier: false
    global_rank: 99
  - model: DC-Graph
    model_key: dc-graph
    model_plain: DC-Graph
    metric_values:
    - null
    - 0.9009
    - 0.999
    metric_stds:
    - null
    - 0.0021
    - 0.0003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9009
    sort_std: 0.0021
    true_value: 0.9009
    true_std: 0.0021
    paper_value: 0.9009
    paper_std: 0.0021
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2407.11025'
    value_gap_source_title: Backdoor Graph Condensation
    value_note: ''
    at_pub_value: 0.882
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.018900000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'Structure-free Graph Condensation: From Large-scale
      Graphs to Condensed Graph-free Data'
    comparison_source_arxiv: '2306.02664'
    is_best: false
    is_std_outlier: false
    global_rank: 102
  - model: GCond-X
    model_key: gcond-x
    model_plain: GCond-X
    metric_values:
    - null
    - 0.8914
    - 0.9989
    metric_stds:
    - null
    - 0.0051
    - 0.0007
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8914
    sort_std: 0.0051
    true_value: 0.8914
    true_std: 0.0051
    paper_value: 0.8914
    paper_std: 0.0051
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2407.11025'
    value_gap_source_title: Backdoor Graph Condensation
    value_note: ''
    at_pub_value: 0.884
    at_pub_std: 0.004
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.007399999999999962
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 108
  - model: Cheby.
    model_key: cheby.
    model_plain: Cheby.
    metric_values:
    - null
    - 0.7579
    - 0.9854
    metric_stds:
    - null
    - 0.0073
    - 0.0171
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7579
    sort_std: 0.0073
    true_value: 0.7579
    true_std: 0.0073
    paper_value: 0.7579
    paper_std: 0.0073
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2407.11025'
    value_gap_source_title: Backdoor Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 120
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - null
    - 0.4366
    - 1.0
    metric_stds:
    - null
    - 0.0104
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7312
    sort_std: 0.0009
    true_value: 0.7312
    true_std: 0.0009
    paper_value: 0.4366
    paper_std: 0.0104
    has_value_gap: true
    has_value_note: false
    value_gap: 0.2946
    value_gap_source_arxiv: '2103.13355'
    value_gap_source_title: Bag of Tricks for Node Classification with Graph Neural
      Networks
    value_note: ''
    at_pub_value: 0.824
    at_pub_std: 0.001
    at_pub_source_arxiv: '2203.00949'
    at_pub_source_title: 'GAP: Differentially Private Graph Neural Networks with Aggregation
      Perturbation'
    at_pub_source_date_iso: '2022-03-02'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2021-03-24'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.38739999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'GAP: Differentially Private Graph Neural Networks with
      Aggregation Perturbation'
    comparison_source_arxiv: '2203.00949'
    is_best: false
    is_std_outlier: false
    global_rank: 122
  metrics:
  - F1
  - Accuracy
  - ASR
  primary_metric: F1
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - Accuracy
  - ASR
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
---

