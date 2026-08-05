---
title: Deformable Graph Transformer
arxiv_id: '2206.14337'
source_url: ''
authors:
- name: Jinyoung Park
  orcid: null
  s2_author_id: '2149155177'
  s2_url: null
- name: Seongjun Yun
  orcid: null
  s2_author_id: '3110007'
  s2_url: null
- name: Hyeon-ju Park
  orcid: null
  s2_author_id: '2110832174'
  s2_url: null
- name: Jaewoo Kang
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jisu Jeong
  orcid: null
  s2_author_id: '2115678107'
  s2_url: null
- name: KyungHyun Kim
  orcid: null
  s2_author_id: '2109351321'
  s2_url: null
- name: Jung-Woo Ha
  orcid: null
  s2_author_id: '2577039'
  s2_url: null
- name: Hyunwoo J. Kim
  orcid: null
  s2_author_id: '2108926667'
  s2_url: null
published_date: Jun 29, 2022
published_date_iso: '2022-06-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Transformer-based models have recently shown success in representation learning
  on graph-structured data beyond natural language processing and computer vision.
  However, the success is limited to small-scale graphs due to the drawbacks of full
  dot-product attention on graphs such as the quadratic complexity with respect to
  the number of nodes and message aggregation from enormous irrelevant nodes. To address
  these issues, we propose Deformable Graph Transformer (DGT) that performs sparse
  attention via dynamically sampled relevant nodes for efficiently handling large-scale
  graphs with a linear complexity in the number of nodes. Specifically, our framework
  first constructs multiple node sequences with various criteria to consider both
  structural and semantic proximity. Then, combining with our learnable Katz Positional
  Encodings, the sparse attention is applied to the node sequences for learning node
  representations with a significantly reduced computational cost. Extensive experiments
  demonstrate that our DGT achieves state-of-the-art performance on 7 graph benchmark
  datasets with 2.5 $ $ 449 times less computational cost compared to transformer-based
  graph models with full attention.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DGT
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Heterophilic Graphs
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Actor
  rows:
  - model: R-SoftGraphAIN
    model_key: nodeformer
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: diggr
    model_plain: R-SoftGraphAIN
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
    input_feature_source: null
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
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.432
    std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 3
    sort_value: 0.432
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.3505
    std: 0.0038
    paper_value: 0.3505
    paper_std: 0.0038
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4018
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.05130000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4018
    true_std: 0.0055
    value_gap_source_arxiv: '2202.03580'
    value_gap_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    value_gap_source_is_current_paper: false
    value_gap: 0.05130000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.4018
    sort_std: 0.0055
    global_rank: 48
    paper_rank: 251
    rank_delta: 203
    rank_delta_abs: 203
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3524
    std: 0.0049
    paper_value: 0.3524
    paper_std: 0.0049
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3423
    at_pub_std: 0.0099
    at_pub_source_arxiv: '2103.06064'
    at_pub_source_title: Graph Neural Networks Inspired by Classical Iterative Algorithms
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.010099999999999998
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3899
    true_std: 0.0085
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03750000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3899
    sort_std: 0.0085
    global_rank: 70
    paper_rank: 239
    rank_delta: 169
    rank_delta_abs: 169
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.3532
    std: 0.0034
    paper_value: 0.3532
    paper_std: 0.0034
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.384
    at_pub_std: 0.01
    at_pub_source_arxiv: '2205.13700'
    at_pub_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    at_pub_source_date_iso: '2022-05-27'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.030799999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3885
    true_std: 0.0117
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0353
    has_value_note: false
    value_note: ''
    sort_value: 0.3885
    sort_std: 0.0117
    global_rank: 73
    paper_rank: 237
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ES-GNN: Generalizing Graph Neural Networks Beyond Homophily
      with Edge Splitting'
    comparison_source_arxiv: '2205.13700'
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.3654
    std: 0.0044
    paper_value: 0.3654
    paper_std: 0.0044
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3785
    true_std: 0.0029
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.0131
    has_value_note: false
    value_note: ''
    sort_value: 0.3785
    sort_std: 0.0029
    global_rank: 105
    paper_rank: 167
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGT
    model_key: dgt
    model_plain: DGT
    value: 0.3693
    std: 0.0039
    paper_value: 0.3693
    paper_std: 0.0039
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3693
    sort_std: 0.0039
    global_rank: 148
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGT-light
    model_key: dgt-light
    model_plain: DGT-light
    value: 0.3686
    std: 0.0053
    paper_value: 0.3686
    paper_std: 0.0053
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3686
    sort_std: 0.0053
    global_rank: 150
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer
    model_key: transformer
    model_plain: Transformer
    value: 0.3661
    std: 0.0039
    paper_value: 0.3661
    paper_std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3661
    sort_std: 0.0039
    global_rank: 166
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeformableGCN
    model_key: deformablegcn
    model_plain: DeformableGCN
    value: 0.3653
    std: 0.0042
    paper_value: 0.3653
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3653
    sort_std: 0.0042
    global_rank: 169
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.3579
    std: 0.0033
    paper_value: 0.3579
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3222
    at_pub_std: 0.0234
    at_pub_source_arxiv: '2105.07634'
    at_pub_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    at_pub_source_date_iso: '2021-05-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.03570000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3648
    true_std: 0.012
    value_gap_source_arxiv: '2306.02376'
    value_gap_source_title: 'Towards Deep Attention in Graph Neural Networks: Problems
      and Remedies'
    value_gap_source_is_current_paper: false
    value_gap: 0.006900000000000017
    has_value_note: false
    value_note: ''
    sort_value: 0.3648
    sort_std: 0.012
    global_rank: 170
    paper_rank: 208
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Improving Graph Neural Networks with Simple Architecture
      Design
    comparison_source_arxiv: '2105.07634'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3013
    std: 0.003
    paper_value: 0.3013
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.369
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.06769999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.362
    true_std: 0.01
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.060699999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.362
    sort_std: 0.01
    global_rank: 184
    paper_rank: 363
    rank_delta: 179
    rank_delta_abs: 179
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.2943
    std: 0.0041
    paper_value: 0.2943
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.349
    at_pub_std: 0.007
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05469999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.361
    true_std: 0.0155
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.06669999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.361
    sort_std: 0.0155
    global_rank: 189
    paper_rank: 376
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.3025
    std: 0.0039
    paper_value: 0.3025
    paper_std: 0.0039
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.356
    at_pub_std: 0.007
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.05349999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3605
    true_std: 0.0035
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.057999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 191
    paper_rank: 357
    rank_delta: 166
    rank_delta_abs: 166
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.3054
    std: 0.0041
    paper_value: 0.3054
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.351
    true_std: 0.002
    value_gap_source_arxiv: '2505.11346'
    value_gap_source_title: What Can We Learn From MIMO Graph Convolutions?
    value_gap_source_is_current_paper: false
    value_gap: 0.045599999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.351
    sort_std: 0.002
    global_rank: 248
    paper_rank: 351
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT-sparse
    model_key: gt-sparse
    model_plain: GT-sparse
    value: 0.3469
    std: 0.0035
    paper_value: 0.3469
    paper_std: 0.0035
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3469
    sort_std: 0.0035
    global_rank: 263
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT-full
    model_key: gt-full
    model_plain: GT-full
    value: 0.3453
    std: 0.0038
    paper_value: 0.3453
    paper_std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3453
    sort_std: 0.0038
    global_rank: 269
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.3039
    std: 0.0035
    paper_value: 0.3039
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.288
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2108.10521'
    at_pub_source_title: 'Bag of Tricks for Training Deeper Graph Neural Networks:
      A Comprehensive Benchmark Study'
    at_pub_source_date_iso: '2021-08-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.015900000000000025
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3342
    true_std: 0.0028
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.030299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.3342
    sort_std: 0.0028
    global_rank: 298
    paper_rank: 354
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Bag of Tricks for Training Deeper Graph Neural Networks:
      A Comprehensive Benchmark Study'
    comparison_source_arxiv: '2108.10521'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.3153
    std: 0.0031
    paper_value: 0.3153
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.381
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.06569999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3163
    true_std: 0.0115
    value_gap_source_arxiv: '2307.16092'
    value_gap_source_title: Feature Transportation Improves Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.3163
    sort_std: 0.0115
    global_rank: 325
    paper_rank: 329
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
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
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.9528
    std: 0.0002
    paper_value: 0.9528
    paper_std: 0.0002
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9702
    at_pub_std: null
    at_pub_source_arxiv: '1907.10903'
    at_pub_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on Node
      Classification'
    at_pub_source_date_iso: '2019-07-25'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-07-25'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.01739999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9702
    true_std: null
    value_gap_source_arxiv: '1907.10903'
    value_gap_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on
      Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.01739999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9702
    sort_std: null
    global_rank: 6
    paper_rank: 50
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks
      on Node Classification'
    comparison_source_arxiv: '1907.10903'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9627
    std: 0.0001
    paper_value: 0.9627
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9647
    at_pub_std: null
    at_pub_source_arxiv: '1907.10903'
    at_pub_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on Node
      Classification'
    at_pub_source_date_iso: '2019-07-25'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2023-05-04'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.0026000000000000467
    has_value_note: false
    value_note: ''
    sort_value: 0.9653
    sort_std: 0.0011
    global_rank: 19
    paper_rank: 28
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks
      on Node Classification'
    comparison_source_arxiv: '1907.10903'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9506
    std: 0.0003
    paper_value: 0.9506
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9648
    at_pub_std: null
    at_pub_source_arxiv: '1907.10903'
    at_pub_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on Node
      Classification'
    at_pub_source_date_iso: '2019-07-25'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-07-25'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.01419999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9648
    true_std: null
    value_gap_source_arxiv: '1907.10903'
    value_gap_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks on
      Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.01419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9648
    sort_std: null
    global_rank: 24
    paper_rank: 60
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'DropEdge: Towards Deep Graph Convolutional Networks
      on Node Classification'
    comparison_source_arxiv: '1907.10903'
    is_best: false
    is_std_outlier: false
  - model: DGT
    model_key: dgt
    model_plain: DGT
    value: 0.9632
    std: 0.0002
    paper_value: 0.9632
    paper_std: 0.0002
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.9632
    sort_std: 0.0002
    global_rank: 28
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.9623
    std: 0.0004
    paper_value: 0.9623
    paper_std: 0.0004
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.9623
    sort_std: 0.0004
    global_rank: 35
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGT-light
    model_key: dgt-light
    model_plain: DGT-light
    value: 0.9614
    std: 0.0005
    paper_value: 0.9614
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.9614
    sort_std: 0.0005
    global_rank: 35
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.9472
    std: 0.0
    paper_value: 0.9472
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.949
    at_pub_std: 0.012
    at_pub_source_arxiv: '1905.09550'
    at_pub_source_title: 'Revisiting Graph Neural Networks: All We Have is Low-Pass
      Filters'
    at_pub_source_date_iso: '2019-05-23'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.0017999999999999128
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.949
    true_std: null
    value_gap_source_arxiv: '2102.10739'
    value_gap_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0017999999999999128
    has_value_note: false
    value_note: ''
    sort_value: 0.949
    sort_std: null
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7003
    std: 0.0016
    paper_value: 0.7003
    paper_std: 0.0016
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.824
    at_pub_std: 0.001
    at_pub_source_arxiv: '2203.00949'
    at_pub_source_title: 'GAP: Differentially Private Graph Neural Networks with Aggregation
      Perturbation'
    at_pub_source_date_iso: '2022-03-02'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2021-03-24'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.12369999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7312
    true_std: 0.0009
    value_gap_source_arxiv: '2103.13355'
    value_gap_source_title: Bag of Tricks for Node Classification with Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.030899999999999928
    has_value_note: false
    value_note: ''
    sort_value: 0.7312
    sort_std: 0.0009
    global_rank: 138
    paper_rank: 142
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GAP: Differentially Private Graph Neural Networks with
      Aggregation Perturbation'
    comparison_source_arxiv: '2203.00949'
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
- &id003
  dataset: twitch-gamers
  rows:
  - model: Polynormer + Wideformer
    model_key: cpf
    model_plain: Polynormer + Wideformer
    value: 0.6977
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.14033'
    title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens
      of Graph Coarsening'
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/vasile-paskardlgm/CPF
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6977
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Polynormer + Wideformer
    model_key: polynormer + wideformer
    model_plain: Polynormer + Wideformer
    value: 0.6733
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6733
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer + Wideformer
    model_key: polynormer
    model_plain: Polynormer + Wideformer
    value: 0.6715
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6715
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGT
    model_key: dgt
    model_plain: DGT
    value: 0.6609
    std: 0.0022
    paper_value: 0.6609
    paper_std: 0.0022
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6609
    sort_std: 0.0022
    global_rank: 15
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.652
    std: 0.0012
    paper_value: 0.652
    paper_std: 0.0012
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.656
    true_std: 0.003
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.656
    sort_std: 0.003
    global_rank: 22
    paper_rank: 23
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGT-light
    model_key: dgt-light
    model_plain: DGT-light
    value: 0.6559
    std: 0.0025
    paper_value: 0.6559
    paper_std: 0.0025
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6559
    sort_std: 0.0025
    global_rank: 23
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.6508
    std: 0.0007
    paper_value: 0.6508
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6508
    sort_std: 0.0007
    global_rank: 27
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6434
    std: 0.0012
    paper_value: 0.6434
    paper_std: 0.0012
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6274
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-08-13'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6456
    true_std: 0.0019
    value_gap_source_arxiv: '2408.07191'
    value_gap_source_title: Joint Graph Rewiring and Feature Denoising via Spectral
      Resonance
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.6456
    sort_std: 0.0019
    global_rank: 32
    paper_rank: 34
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6473
    std: 0.0011
    paper_value: 0.6473
    paper_std: 0.0011
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6437
    true_std: 0.0039
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0035999999999999366
    has_value_note: false
    value_note: ''
    sort_value: 0.6437
    sort_std: 0.0039
    global_rank: 34
    paper_rank: 31
    rank_delta: -3
    rank_delta_abs: 3
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATv2
    model_key: gatv2
    model_plain: GATv2
    value: 0.6415
    std: 0.0009
    paper_value: 0.6415
    paper_std: 0.0009
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6415
    sort_std: 0.0009
    global_rank: 39
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT-sparse
    model_key: gt-sparse
    model_plain: GT-sparse
    value: 0.6309
    std: 0.0071
    paper_value: 0.6309
    paper_std: 0.0071
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6309
    sort_std: 0.0071
    global_rank: 42
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6114
    std: 0.0006
    paper_value: 0.6114
    paper_std: 0.0006
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6092
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0022000000000000908
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6092
    true_std: 0.0007
    value_gap_source_arxiv: '2202.03580'
    value_gap_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    value_gap_source_is_current_paper: false
    value_gap: 0.0022000000000000908
    has_value_note: false
    value_note: ''
    sort_value: 0.6092
    sort_std: 0.0007
    global_rank: 54
    paper_rank: 50
    rank_delta: -4
    rank_delta_abs: 4
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.6047
    std: 0.0014
    paper_value: 0.6047
    paper_std: 0.0014
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6047
    sort_std: 0.0014
    global_rank: 57
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.629
    std: 0.0022
    paper_value: 0.629
    paper_std: 0.0022
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-09'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5989
    true_std: 0.0412
    value_gap_source_arxiv: '2311.05185'
    value_gap_source_title: Mixture of Weak & Strong Experts on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.030100000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.5989
    sort_std: 0.0412
    global_rank: 58
    paper_rank: 42
    rank_delta: -16
    rank_delta_abs: 16
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
- benchmark: LINKX Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Actor
      dataset_slug: actor
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: twitch-gamers
      dataset_slug: twitch-gamers
single_proposed_model: DGT
main_figure: /figures/2206.14337/main_figure.jpegoptim.jpg
---

