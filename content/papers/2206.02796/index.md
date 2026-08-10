---
title: Mixed Graph Contrastive Network for Semi-Supervised Node Classification
arxiv_id: '2206.02796'
source_url: ''
authors:
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Yiqi Wang
  orcid: null
  s2_author_id: '2289502260'
  s2_url: null
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: Yi Wen
  orcid: null
  s2_author_id: '2260472167'
  s2_url: null
- name: Lingyuan Meng
  orcid: null
  s2_author_id: '13325191'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
- name: En Zhu
  orcid: null
  s2_author_id: '2144622766'
  s2_url: null
published_date: Jun 6, 2022
published_date_iso: '2022-06-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) have achieved promising performance in semi-supervised
  node classification in recent years. However, the problem of insufficient supervision,
  together with representation collapse, largely limits the performance of the GNNs
  in this field. To alleviate the collapse of node representations in semi-supervised
  scenario, we propose a novel graph contrastive learning method, termed Mixed Graph
  Contrastive Network (MGCN). In our method, we improve the discriminative capability
  of the latent embeddings by an interpolation-based augmentation strategy and a correlation
  reduction mechanism. Specifically, we first conduct the interpolation-based augmentation
  in the latent space and then force the prediction model to change linearly between
  samples. Second, we enable the learned network to tell apart samples across two
  interpolation-perturbed views through forcing the correlation matrix across views
  to approximate an identity matrix. By combining the two settings, we extract rich
  supervision information from both the abundant unlabeled nodes and the rare yet
  valuable labeled nodes for discriminative representation learning. Extensive experimental
  results on six datasets demonstrate the effectiveness and the generality of MGCN
  compared to the existing state-of-the-art methods. The code of MGCN is available
  at https://github.com/xihongyang1999/MGCN on Github.
codebase_url: https://github.com/xihongyang1999/MGCN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MGCN
mrr: 0.0044
adjusted_mrr: 0.0044
mrr_dataset_count: 6
benchmark_categories:
- Classic
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 2
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id006
  dataset: ACM
  is_multi_metric: true
  rows:
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    metric_values:
    - 0.9469
    - null
    metric_stds:
    - 0.0036
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    published_venue: ''
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9469
    sort_std: 0.0036
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
  - model: PSHGCN
    model_key: pshgcn
    model_plain: PSHGCN
    metric_values:
    - 0.9427
    - null
    metric_stds:
    - 0.0023
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    published_venue: ''
    date: May 31, 2023
    date_display: May 2023
    date_iso: '2023-05-31'
    codebase_url: https://github.com/ivam-he/PSHGCN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.9427
    sort_std: 0.0023
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
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    metric_values:
    - 0.9406
    - null
    metric_stds:
    - 0.0022
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.01927'
    title: 'SlotGAT: Slot-based Message Passing for Heterogeneous Graphs'
    published_venue: ''
    date: May 3, 2024
    date_display: May 2024
    date_iso: '2024-05-03'
    codebase_url: https://github.com/scottjiao/SlotGAT_ICML23
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9406
    sort_std: 0.0022
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.8388
    - null
    metric_stds:
    - 0.0035
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9278
    sort_std: null
    true_value: 0.9278
    true_std: null
    paper_value: 0.8388
    paper_std: 0.0035
    has_value_gap: true
    has_value_note: false
    value_gap: 0.08899999999999997
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_note: ''
    at_pub_value: 0.9278
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.08899999999999997
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.8495
    - null
    metric_stds:
    - 0.0021
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9246
    sort_std: null
    true_value: 0.9246
    true_std: null
    paper_value: 0.8495
    paper_std: 0.0021
    has_value_gap: true
    has_value_note: false
    value_gap: 0.07509999999999994
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_note: ''
    at_pub_value: 0.9246
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.07509999999999994
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: SGC
    model_key: sgc
    model_plain: SGC
    metric_values:
    - 0.7299
    - null
    metric_stds:
    - 0.0296
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9235
    sort_std: null
    true_value: 0.9235
    true_std: null
    paper_value: 0.7299
    paper_std: 0.0296
    has_value_gap: true
    has_value_note: false
    value_gap: 0.1936
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_note: ''
    at_pub_value: 0.9235
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.1936
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: true
    is_std_outlier: false
    global_rank: 31
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    metric_values:
    - 0.8093
    - null
    metric_stds:
    - 0.0226
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9228
    sort_std: 0.0027
    true_value: 0.9228
    true_std: 0.0027
    paper_value: 0.8093
    paper_std: 0.0226
    has_value_gap: true
    has_value_note: false
    value_gap: 0.11349999999999993
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 35
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.9135
    - null
    metric_stds:
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.08294'
    title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous Graphs
    published_venue: ''
    date: Jul 16, 2020
    date_display: Jul 2020
    date_iso: '2020-07-16'
    codebase_url: https://github.com/mlvlab/SELAR
    uses_external_data: false
    is_global_top: true
    global_rank: 49
    is_best: false
    sort_value: 0.9135
    sort_std: null
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.3765
    - null
    metric_stds:
    - 0.0001
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9063
    sort_std: 0.0076
    true_value: 0.9063
    true_std: 0.0076
    paper_value: 0.3765
    paper_std: 0.0001
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5298
    value_gap_source_arxiv: '2310.14481'
    value_gap_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-23'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 56
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.8126
    - null
    metric_stds:
    - 0.0148
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8844
    sort_std: 0.003
    true_value: 0.8844
    true_std: 0.003
    paper_value: 0.8126
    paper_std: 0.0148
    has_value_gap: true
    has_value_note: false
    value_gap: 0.07179999999999997
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_note: ''
    at_pub_value: 0.881
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06840000000000002
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
    global_rank: 78
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - 0.8378
    - null
    metric_stds:
    - 0.0027
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8803
    sort_std: 0.0138
    true_value: 0.8803
    true_std: 0.0138
    paper_value: 0.8378
    paper_std: 0.0027
    has_value_gap: true
    has_value_note: false
    value_gap: 0.04249999999999998
    value_gap_source_arxiv: '2206.12547'
    value_gap_source_title: Geometry Contrastive Learning on Heterogeneous Graphs
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-25'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 83
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    metric_values:
    - 0.8788
    - 0.8788
    metric_stds:
    - 0.0054
    - 0.0054
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8788
    sort_std: 0.0054
    true_value: 0.8788
    true_std: 0.0054
    paper_value: 0.8788
    paper_std: 0.0054
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: 0.86
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.01880000000000004
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
    global_rank: 85
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - 0.8593
    - null
    metric_stds:
    - 0.0056
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8764
    sort_std: 0.0031
    true_value: 0.8764
    true_std: 0.0031
    paper_value: 0.8593
    paper_std: 0.0056
    has_value_gap: true
    has_value_note: false
    value_gap: 0.017100000000000004
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 88
  - model: Graph Mixup
    model_key: graph mixup
    model_plain: Graph Mixup
    metric_values:
    - 0.8644
    - null
    metric_stds:
    - 0.0125
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.8644
    sort_std: 0.0125
    true_value: 0.8644
    true_std: 0.0125
    paper_value: 0.8644
    paper_std: 0.0125
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 92
  - model: MixupForGraph
    model_key: mixupforgraph
    model_plain: MixupForGraph
    metric_values:
    - 0.8624
    - null
    metric_stds:
    - 0.0062
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8624
    sort_std: 0.0062
    true_value: 0.8624
    true_std: 0.0062
    paper_value: 0.8624
    paper_std: 0.0062
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 93
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    metric_values:
    - 0.8609
    - null
    metric_stds:
    - 0.0199
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8609
    sort_std: 0.0199
    true_value: 0.8609
    true_std: 0.0199
    paper_value: 0.8609
    paper_std: 0.0199
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 94
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - 0.8604
    - null
    metric_stds:
    - 0.0067
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8604
    sort_std: 0.0067
    true_value: 0.8604
    true_std: 0.0067
    paper_value: 0.8604
    paper_std: 0.0067
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 97
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    metric_values:
    - 0.8575
    - null
    metric_stds:
    - 0.0055
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8575
    sort_std: 0.0055
    true_value: 0.8575
    true_std: 0.0055
    paper_value: 0.8575
    paper_std: 0.0055
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 98
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    metric_values:
    - 0.812
    - null
    metric_stds:
    - 0.0011
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.812
    sort_std: 0.0011
    true_value: 0.812
    true_std: 0.0011
    paper_value: 0.812
    paper_std: 0.0011
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 106
  - model: GCN-Cheby
    model_key: gcn-cheby
    model_plain: GCN-Cheby
    metric_values:
    - 0.7998
    - null
    metric_stds:
    - 0.0307
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7998
    sort_std: 0.0307
    true_value: 0.7998
    true_std: 0.0307
    paper_value: 0.7998
    paper_std: 0.0307
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 107
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - 0.7923
    - null
    metric_stds:
    - 0.0173
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7923
    sort_std: 0.0173
    true_value: 0.7923
    true_std: 0.0173
    paper_value: 0.7923
    paper_std: 0.0173
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    metric_values:
    - 0.7461
    - null
    metric_stds:
    - 0.0067
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7461
    sort_std: 0.0067
    true_value: 0.7461
    true_std: 0.0067
    paper_value: 0.7461
    paper_std: 0.0067
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 110
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.7102
    - null
    metric_stds:
    - 0.0221
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7102
    sort_std: 0.0221
    true_value: 0.7102
    true_std: 0.0221
    paper_value: 0.7102
    paper_std: 0.0221
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 113
  metrics:
  - Micro-F1
  - Accuracy
  primary_metric: Micro-F1
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  - Accuracy
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9412
    std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9412
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9398
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
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9398
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9351
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9351
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8463
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
    arxiv_id: '2407.11907'
    title: 'GraphFM: A generalist graph transformer that learns transferable representations
      across diverse domains'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/nerdslab/GraphFM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 365
    sort_value: 0.8463
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.8399
    std: 0.009
    paper_value: 0.8399
    paper_std: 0.009
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
    protocol_note: Semi-supervised classification on Computers dataset
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8399
    true_std: 0.009
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8399
    sort_std: 0.009
    global_rank: 398
    paper_rank: 398
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
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9669
    std: 0.0014
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9669
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.9264
    std: 0.0024
    paper_value: 0.9264
    paper_std: 0.0024
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
    protocol_note: Semi-supervised classification on Photo dataset
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9264
    true_std: 0.0024
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9264
    sort_std: 0.0024
    global_rank: 297
    paper_rank: 297
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
    value: 0.9128
    std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 426
    sort_value: 0.9128
    sort_std: 0.0063
    comparison_type: global_top
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6763
    std: 0.0038
    paper_value: 0.6763
    paper_std: 0.0038
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
    source_ref: GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8797
    true_std: 0.0024
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.20340000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8797
    sort_std: 0.0024
    global_rank: 18
    paper_rank: 765
    rank_delta: 747
    rank_delta_abs: 747
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6152
    std: 0.0044
    paper_value: 0.6152
    paper_std: 0.0044
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
    source_ref: Graphsage
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7923
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.17710000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8774
    true_std: 0.0041
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2622
    has_value_note: false
    value_note: ''
    sort_value: 0.8774
    sort_std: 0.0041
    global_rank: 20
    paper_rank: 891
    rank_delta: 871
    rank_delta_abs: 871
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
    value: 0.673
    std: 0.0035
    paper_value: 0.673
    paper_std: 0.0035
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.12129999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.20389999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 775
    rank_delta: 754
    rank_delta_abs: 754
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.6859
    std: 0.003
    paper_value: 0.6859
    paper_std: 0.003
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
    source_ref: PPNP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.805
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1191000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8142
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.12830000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8142
    sort_std: 0.0026
    global_rank: 29
    paper_rank: 735
    rank_delta: 706
    rank_delta_abs: 706
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.672
    std: 0.0046
    paper_value: 0.672
    paper_std: 0.0046
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8013
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.12929999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.136
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 780
    rank_delta: 734
    rank_delta_abs: 734
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
    value: 0.5889
    std: 0.0047
    paper_value: 0.5889
    paper_std: 0.0047
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
    source_ref: SGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7765
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.1876
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7965
    true_std: 0.0102
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.2076
    has_value_note: false
    value_note: ''
    sort_value: 0.7965
    sort_std: 0.0102
    global_rank: 68
    paper_rank: 916
    rank_delta: 848
    rank_delta_abs: 848
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.6543
    std: 0.0294
    paper_value: 0.6543
    paper_std: 0.0294
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
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7882
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.13390000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.789
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.13470000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.002
    global_rank: 83
    paper_rank: 832
    rank_delta: 749
    rank_delta_abs: 749
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.6798
    std: 0.0005
    paper_value: 0.6798
    paper_std: 0.0005
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
    source_ref: MVGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7808
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.10100000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7808
    true_std: 0.0006
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.10100000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0006
    global_rank: 108
    paper_rank: 754
    rank_delta: 646
    rank_delta_abs: 646
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7618
    std: 0.0078
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
    global_rank: 165
    sort_value: 0.7618
    sort_std: 0.0078
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.6778
    std: 0.0085
    paper_value: 0.6778
    paper_std: 0.0085
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
    source_ref: bgrl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7182
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04039999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08220000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.002
    global_rank: 171
    paper_rank: 762
    rank_delta: 591
    rank_delta_abs: 591
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.6625
    std: 0.0394
    paper_value: 0.6625
    paper_std: 0.0394
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
    source_ref: GCA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7133
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05080000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7523
    true_std: 0.0119
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08979999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7523
    sort_std: 0.0119
    global_rank: 211
    paper_rank: 809
    rank_delta: 598
    rank_delta_abs: 598
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.6624
    std: 0.0074
    paper_value: 0.6624
    paper_std: 0.0074
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
    source_ref: graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.747
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2203.14082'
    at_pub_source_title: Metropolis-Hastings Data Augmentation for Graph Neural Networks
    at_pub_source_date_iso: '2022-03-26'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-03-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.08460000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.747
    true_std: 0.0059
    value_gap_source_arxiv: '2203.14082'
    value_gap_source_title: Metropolis-Hastings Data Augmentation for Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08460000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.747
    sort_std: 0.0059
    global_rank: 234
    paper_rank: 809
    rank_delta: 575
    rank_delta_abs: 575
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Metropolis-Hastings Data Augmentation for Graph Neural
      Networks
    comparison_source_arxiv: '2203.14082'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.6654
    std: 0.0001
    paper_value: 0.6654
    paper_std: 0.0001
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
    source_ref: GRACE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.717
    at_pub_std: 0.006
    at_pub_source_arxiv: '2009.07111'
    at_pub_source_title: Contrastive and Generative Graph Convolutional Networks for
      Graph-based Semi-Supervised Learning
    at_pub_source_date_iso: '2020-09-15'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.05159999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.0796
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 798
    rank_delta: 553
    rank_delta_abs: 553
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Contrastive and Generative Graph Convolutional Networks
      for Graph-based Semi-Supervised Learning
    comparison_source_arxiv: '2009.07111'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5288
    std: 0.0051
    paper_value: 0.5288
    paper_std: 0.0051
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
    source_ref: MLP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6958
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.16699999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7289
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.20009999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 941
    rank_delta: 540
    rank_delta_abs: 540
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    value: 0.6085
    std: 0.0076
    paper_value: 0.6085
    paper_std: 0.0076
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
    source_ref: JKNet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.707
    at_pub_std: 0.007
    at_pub_source_arxiv: '2203.00638'
    at_pub_source_title: 'PaSca: a Graph Neural Architecture Search System under the
      Scalable Paradigm'
    at_pub_source_date_iso: '2022-03-01'
    at_pub_source_date_label: WWW 2022
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: 0.09849999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.707
    true_std: 0.007
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.09849999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.707
    sort_std: 0.007
    global_rank: 640
    paper_rank: 897
    rank_delta: 257
    rank_delta_abs: 257
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    comparison_source_arxiv: '2203.00638'
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.6918
    std: 0.0043
    paper_value: 0.6918
    paper_std: 0.0043
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6918
    true_std: 0.0043
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6918
    sort_std: 0.0043
    global_rank: 711
    paper_rank: 711
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph Mixup
    model_key: graph mixup
    model_plain: Graph Mixup
    value: 0.6753
    std: 0.0087
    paper_value: 0.6753
    paper_std: 0.0087
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
    source_ref: graphmixup
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6753
    true_std: 0.0087
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6753
    sort_std: 0.0087
    global_rank: 768
    paper_rank: 768
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-Cheby
    model_key: gcn-cheby
    model_plain: GCN-Cheby
    value: 0.6567
    std: 0.0038
    paper_value: 0.6567
    paper_std: 0.0038
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
    source_ref: GCN_CHEBY
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6567
    true_std: 0.0038
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6567
    sort_std: 0.0038
    global_rank: 830
    paper_rank: 830
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    value: 0.6258
    std: 0.0144
    paper_value: 0.6258
    paper_std: 0.0144
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
    source_ref: adagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6258
    true_std: 0.0144
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6258
    sort_std: 0.0144
    global_rank: 881
    paper_rank: 881
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixupForGraph
    model_key: mixupforgraph
    model_plain: MixupForGraph
    value: 0.5741
    std: 0.0033
    paper_value: 0.5741
    paper_std: 0.0033
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
    source_ref: GRAPH_MIXUP_1
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5741
    true_std: 0.0033
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5741
    sort_std: 0.0033
    global_rank: 926
    paper_rank: 926
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
    value: 0.7521
    std: 0.0038
    paper_value: 0.7521
    paper_std: 0.0038
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8728
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.12070000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1483
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 854
    rank_delta: 823
    rank_delta_abs: 823
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.7951
    std: 0.0036
    paper_value: 0.7951
    paper_std: 0.0036
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
    source_ref: GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8941
    true_std: 0.007
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.09899999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8941
    sort_std: 0.007
    global_rank: 48
    paper_rank: 755
    rank_delta: 707
    rank_delta_abs: 707
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
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.7941
    std: 0.0038
    paper_value: 0.7941
    paper_std: 0.0038
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
    source_ref: PPNP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8787
    at_pub_std: null
    at_pub_source_arxiv: '2109.11338'
    at_pub_source_title: Orthogonal Graph Neural Networks
    at_pub_source_date_iso: '2021-09-23'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08460000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8904
    true_std: 0.015
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.09629999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 65
    paper_rank: 761
    rank_delta: 696
    rank_delta_abs: 696
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Orthogonal Graph Neural Networks
    comparison_source_arxiv: '2109.11338'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.767
    std: 0.0042
    paper_value: 0.767
    paper_std: 0.0042
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.122
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.12270000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 824
    rank_delta: 757
    rank_delta_abs: 757
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7089
    std: 0.0054
    paper_value: 0.7089
    paper_std: 0.0054
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
    source_ref: Graphsage
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8777
    at_pub_std: 0.0183
    at_pub_source_arxiv: '2110.15777'
    at_pub_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.16880000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8777
    true_std: 0.0183
    value_gap_source_arxiv: '2110.15777'
    value_gap_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    value_gap_source_is_current_paper: false
    value_gap: 0.16880000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8777
    sort_std: 0.0183
    global_rank: 146
    paper_rank: 899
    rank_delta: 753
    rank_delta_abs: 753
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling
      Both Homophily and Heterophily'
    comparison_source_arxiv: '2110.15777'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7887
    std: 0.0041
    paper_value: 0.7887
    paper_std: 0.0041
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
    source_ref: bgrl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8144
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.025700000000000056
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08430000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 170
    paper_rank: 780
    rank_delta: 610
    rank_delta_abs: 610
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7862
    std: 0.0062
    paper_value: 0.7862
    paper_std: 0.0062
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
    source_ref: GRACE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.821
    at_pub_std: 0.016
    at_pub_source_arxiv: '2012.07437'
    at_pub_source_title: Rethinking the Promotion Brought by Contrastive Learning
      to Semi-Supervised Node Classification
    at_pub_source_date_iso: '2020-12-14'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03479999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.872
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08579999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.002
    global_rank: 176
    paper_rank: 787
    rank_delta: 611
    rank_delta_abs: 611
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Rethinking the Promotion Brought by Contrastive Learning
      to Semi-Supervised Node Classification
    comparison_source_arxiv: '2012.07437'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7081
    std: 0.0067
    paper_value: 0.7081
    paper_std: 0.0067
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
    source_ref: SGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8425
    at_pub_std: 0.001
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.13440000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8683
    true_std: 0.0128
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.1602
    has_value_note: false
    value_note: ''
    sort_value: 0.8683
    sort_std: 0.0128
    global_rank: 202
    paper_rank: 899
    rank_delta: 697
    rank_delta_abs: 697
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7806
    std: 0.0007
    paper_value: 0.7806
    paper_std: 0.0007
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
    source_ref: MVGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8538
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.07320000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.868
    true_std: 0.005
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.08740000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.005
    global_rank: 205
    paper_rank: 795
    rank_delta: 590
    rank_delta_abs: 590
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GCN-Cheby
    model_key: gcn-cheby
    model_plain: GCN-Cheby
    value: 0.7139
    std: 0.0051
    paper_value: 0.7139
    paper_std: 0.0051
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
    source_ref: GCN-Cheby
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8676
    true_std: 0.0095
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.15370000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8676
    sort_std: 0.0095
    global_rank: 209
    paper_rank: 896
    rank_delta: 687
    rank_delta_abs: 687
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7374
    std: 0.0143
    paper_value: 0.7374
    paper_std: 0.0143
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
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8508
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.11339999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.863
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.12559999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.002
    global_rank: 227
    paper_rank: 874
    rank_delta: 647
    rank_delta_abs: 647
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    value: 0.7322
    std: 0.0064
    paper_value: 0.7322
    paper_std: 0.0064
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
    source_ref: JKNet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8579
    true_std: 0.0001
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.12570000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8579
    sort_std: 0.0001
    global_rank: 247
    paper_rank: 878
    rank_delta: 631
    rank_delta_abs: 631
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.7449
    std: 0.037
    paper_value: 0.7449
    paper_std: 0.037
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
    source_ref: GCA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8207
    at_pub_std: 0.001
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.07579999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8409
    true_std: 0.0085
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.09599999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.0085
    global_rank: 363
    paper_rank: 865
    rank_delta: 502
    rank_delta_abs: 502
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.7854
    std: 0.0032
    paper_value: 0.7854
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
    source_ref: graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8394
    at_pub_std: 0.0057
    at_pub_source_arxiv: '1909.11715'
    at_pub_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    at_pub_source_date_iso: '2019-09-25'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-25'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.05400000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8394
    true_std: 0.0057
    value_gap_source_arxiv: '1909.11715'
    value_gap_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05400000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8394
    sort_std: 0.0057
    global_rank: 371
    paper_rank: 787
    rank_delta: 416
    rank_delta_abs: 416
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphMix: Improved Training of GNNs for Semi-Supervised
      Learning'
    comparison_source_arxiv: '1909.11715'
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.8089
    std: 0.0095
    paper_value: 0.8089
    paper_std: 0.0095
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
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-11-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8123
    true_std: 0.0043
    value_gap_source_arxiv: '2511.19976'
    value_gap_source_title: Rethinking Semi-Supervised Node Classification with Self-Supervised
      Graph Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.0034000000000000696
    has_value_note: false
    value_note: ''
    sort_value: 0.8123
    sort_std: 0.0043
    global_rank: 672
    paper_rank: 704
    rank_delta: 32
    rank_delta_abs: 32
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
    value: 0.5034
    std: 0.0048
    paper_value: 0.5034
    paper_std: 0.0048
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
    source_ref: MLP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7414
    at_pub_std: 0.014
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.238
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2734000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 991
    rank_delta: 185
    rank_delta_abs: 185
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: Graph Mixup
    model_key: graph mixup
    model_plain: Graph Mixup
    value: 0.7716
    std: 0.0112
    paper_value: 0.7716
    paper_std: 0.0112
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
    source_ref: graphmixup
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7716
    true_std: 0.0112
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7716
    sort_std: 0.0112
    global_rank: 820
    paper_rank: 820
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixupForGraph
    model_key: mixupforgraph
    model_plain: MixupForGraph
    value: 0.6711
    std: 0.0063
    paper_value: 0.6711
    paper_std: 0.0063
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
    source_ref: GRAPH_MIXUP_1
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6711
    true_std: 0.0063
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6711
    sort_std: 0.0063
    global_rank: 931
    paper_rank: 931
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    value: 0.6241
    std: 0.0184
    paper_value: 0.6241
    paper_std: 0.0184
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
    source_ref: adagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6241
    true_std: 0.0184
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6241
    sort_std: 0.0184
    global_rank: 954
    paper_rank: 954
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
- &id005
  dataset: DBLP
  rows:
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.9566
    std: 0.002
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9566
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PSHGCN
    model_key: pshgcn
    model_plain: PSHGCN
    value: 0.9561
    std: 0.0012
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_display: May 2023
    date_iso: '2023-05-31'
    venue: The Web Conference
    codebase_url: https://github.com/ivam-he/PSHGCN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9561
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RpHGNN
    model_key: rphgnn
    model_plain: RpHGNN
    value: 0.9555
    std: 0.0029
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14481'
    title: Efficient Heterogeneous Graph Learning via Random Projection
    date: Oct 23, 2023
    date_display: Oct 2023
    date_iso: '2023-10-23'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/CrawlScript/RpHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9555
    sort_std: 0.0029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6764
    std: 0.0038
    paper_value: 0.6764
    paper_std: 0.0038
    metric: Micro-F1
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.931
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.25460000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.946
    true_std: 0.0031
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.26959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.946
    sort_std: 0.0031
    global_rank: 21
    paper_rank: 177
    rank_delta: 156
    rank_delta_abs: 156
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6858
    std: 0.0042
    paper_value: 0.6858
    paper_std: 0.0042
    metric: Micro-F1
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9339
    at_pub_std: 0.003
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.2481
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9448
    true_std: 0.0022
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.259
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0022
    global_rank: 23
    paper_rank: 174
    rank_delta: 151
    rank_delta_abs: 151
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.2949
    std: 0.0003
    paper_value: 0.2949
    paper_std: 0.0003
    metric: Micro-F1
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
    source_ref: Graphsage
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8473
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-10-23'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.5524
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9306
    true_std: 0.0047
    value_gap_source_arxiv: '2310.14481'
    value_gap_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    value_gap_source_is_current_paper: false
    value_gap: 0.6356999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9306
    sort_std: 0.0047
    global_rank: 46
    paper_rank: 195
    rank_delta: 149
    rank_delta_abs: 149
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.6789
    std: 0.0034
    paper_value: 0.6789
    paper_std: 0.0034
    metric: Micro-F1
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
    source_ref: MVGRL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9289
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-18'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.25
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9289
    true_std: null
    value_gap_source_arxiv: '2012.10024'
    value_gap_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.25
    has_value_note: false
    value_note: ''
    sort_value: 0.9289
    sort_std: null
    global_rank: 50
    paper_rank: 177
    rank_delta: 127
    rank_delta_abs: 127
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6784
    std: 0.003
    paper_value: 0.6784
    paper_std: 0.003
    metric: Micro-F1
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
    source_ref: GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9245
    true_std: 0.0076
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.24609999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9245
    sort_std: 0.0076
    global_rank: 60
    paper_rank: 177
    rank_delta: 117
    rank_delta_abs: 117
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.6888
    std: 0.0004
    paper_value: 0.6888
    paper_std: 0.0004
    metric: Micro-F1
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
    source_ref: GRACE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0007
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.22399999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0007
    global_rank: 74
    paper_rank: 174
    rank_delta: 100
    rank_delta_abs: 100
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.689
    std: 0.0134
    paper_value: 0.689
    paper_std: 0.0134
    metric: Micro-F1
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
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.72
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.031000000000000028
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9016
    true_std: 0.006
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.2126
    has_value_note: false
    value_note: ''
    sort_value: 0.9016
    sort_std: 0.006
    global_rank: 79
    paper_rank: 172
    rank_delta: 93
    rank_delta_abs: 93
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.872
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The node features come from the same distribution of
      the graph used to train the target model.
    is_global_top: true
    global_rank: 88
    sort_value: 0.872
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.6775
    std: 0.0044
    paper_value: 0.6775
    paper_std: 0.0044
    metric: Micro-F1
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
    source_ref: PPNP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.844
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-25'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.16649999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.844
    true_std: 0.0017
    value_gap_source_arxiv: '2110.13094'
    value_gap_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.16649999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.844
    sort_std: 0.0017
    global_rank: 114
    paper_rank: 177
    rank_delta: 63
    rank_delta_abs: 63
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.6011
    std: 0.0194
    paper_value: 0.6011
    paper_std: 0.0194
    metric: Micro-F1
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
    source_ref: GCA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-06'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8399
    true_std: 0.0021
    value_gap_source_arxiv: '2310.03977'
    value_gap_source_title: Perfect Alignment May be Poisonous to Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.2388
    has_value_note: false
    value_note: ''
    sort_value: 0.8399
    sort_std: 0.0021
    global_rank: 115
    paper_rank: 183
    rank_delta: 68
    rank_delta_abs: 68
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.6848
    std: 0.0056
    paper_value: 0.6848
    paper_std: 0.0056
    metric: Micro-F1
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
    source_ref: bgrl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-08-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.807
    true_std: null
    value_gap_source_arxiv: '2208.10493'
    value_gap_source_title: Relational Self-Supervised Learning on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.12220000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.807
    sort_std: null
    global_rank: 133
    paper_rank: 175
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    value: 0.706
    std: 0.0076
    paper_value: 0.706
    paper_std: 0.0076
    metric: Micro-F1
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
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.713
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-09-14'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.713
    true_std: null
    value_gap_source_arxiv: '2009.06211'
    value_gap_source_title: Implicit Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.007000000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.713
    sort_std: null
    global_rank: 169
    paper_rank: 170
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaGCN
    model_key: adagcn
    model_plain: AdaGCN
    value: 0.697
    std: 0.0135
    paper_value: 0.697
    paper_std: 0.0135
    metric: Micro-F1
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
    source_ref: adagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.697
    true_std: 0.0135
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.697
    sort_std: 0.0135
    global_rank: 171
    paper_rank: 171
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixupForGraph
    model_key: mixupforgraph
    model_plain: MixupForGraph
    value: 0.6851
    std: 0.0078
    paper_value: 0.6851
    paper_std: 0.0078
    metric: Micro-F1
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
    source_ref: GRAPH_MIXUP_1
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6851
    true_std: 0.0078
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6851
    sort_std: 0.0078
    global_rank: 175
    paper_rank: 175
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph Mixup
    model_key: graph mixup
    model_plain: Graph Mixup
    value: 0.6848
    std: 0.0152
    paper_value: 0.6848
    paper_std: 0.0152
    metric: Micro-F1
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
    source_ref: graphmixup
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6848
    true_std: 0.0152
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6848
    sort_std: 0.0152
    global_rank: 176
    paper_rank: 176
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMix
    model_key: graphmix
    model_plain: GraphMix
    value: 0.6798
    std: 0.0036
    paper_value: 0.6798
    paper_std: 0.0036
    metric: Micro-F1
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
    source_ref: graphmix
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6798
    true_std: 0.0036
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6798
    sort_std: 0.0036
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    value: 0.6451
    std: 0.0053
    paper_value: 0.6451
    paper_std: 0.0053
    metric: Micro-F1
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
    source_ref: JKNet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6451
    true_std: 0.0053
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6451
    sort_std: 0.0053
    global_rank: 178
    paper_rank: 178
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
    value: 0.6307
    std: 0.0233
    paper_value: 0.6307
    paper_std: 0.0233
    metric: Micro-F1
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
    source_ref: MLP
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-11'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6447
    true_std: 0.0136
    value_gap_source_arxiv: '2310.07365'
    value_gap_source_title: 'GraphControl: Adding Conditional Control to Universal
      Graph Pre-trained Models for Graph Domain Transfer Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.014000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.6447
    sort_std: 0.0136
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.5366
    std: 0.0215
    paper_value: 0.5366
    paper_std: 0.0215
    metric: Micro-F1
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
    source_ref: SGC
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-08-12'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.623
    true_std: 0.0009
    value_gap_source_arxiv: '2208.06129'
    value_gap_source_title: Multiplex Heterogeneous Graph Convolutional Network
    value_gap_source_is_current_paper: false
    value_gap: 0.08640000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.623
    sort_std: 0.0009
    global_rank: 180
    paper_rank: 188
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-Cheby
    model_key: gcn-cheby
    model_plain: GCN-Cheby
    value: 0.6048
    std: 0.0
    paper_value: 0.6048
    paper_std: 0.0
    metric: Micro-F1
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
    source_ref: GCN_CHEBY
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Semi-supervised node classification on DBLP
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6048
    true_std: 0.0
    value_gap_source_arxiv: '2206.02796'
    value_gap_source_title: Mixed Graph Contrastive Network for Semi-Supervised Node
      Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6048
    sort_std: 0.0
    global_rank: 183
    paper_rank: 183
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id005
  - *id006
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
single_proposed_model: MGCN
main_figure: /figures/2206.02796/main_figure.jpegoptim.jpg
---

