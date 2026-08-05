---
title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
arxiv_id: '2210.13978'
source_url: ''
authors:
- name: Yinan Huang
  orcid: null
  s2_author_id: '2118799134'
  s2_url: null
- name: Xingang Peng
  orcid: null
  s2_author_id: '8249753'
  s2_url: null
- name: Jianzhu Ma
  orcid: null
  s2_author_id: '5214991'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '1390814008'
  s2_url: null
published_date: Oct 22, 2022
published_date_iso: '2022-10-22'
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Message Passing Neural Networks (MPNNs) are a widely used class of Graph
  Neural Networks (GNNs). The limited representational power of MPNNs inspires the
  study of provably powerful GNN architectures. However, knowing one model is more
  powerful than another gives little insight about what functions they can or cannot
  express. It is still unclear whether these models are able to approximate specific
  functions such as counting certain graph substructures, which is essential for applications
  in biology, chemistry and social network analysis. Motivated by this, we propose
  to study the counting power of Subgraph MPNNs, a recent and popular class of powerful
  GNN models that extract rooted subgraphs for each node, assign the root node a unique
  identifier and encode the root node's representation within its rooted subgraph.
  Specifically, we prove that Subgraph MPNNs fail to count more-than-4-cycles at node
  level, implying that node representations cannot correctly encode the surrounding
  substructures like ring systems with more than four atoms. To overcome this limitation,
  we propose I$^2$-GNNs to extend Subgraph MPNNs by assigning different identifiers
  for the root node and its neighbors in each subgraph. I$^2$-GNNs' discriminative
  power is shown to be strictly stronger than Subgraph MPNNs and partially stronger
  than the 3-WL test. More importantly, I$^2$-GNNs are proven capable of counting
  all 3, 4, 5 and 6-cycles, covering common substructures like benzene rings in organic
  chemistry, while still keeping linear complexity. To the best of our knowledge,
  it is the first linear-time GNN model that can count 6-cycles with theoretical guarantees.
  We validate its counting power in cycle counting tasks and demonstrate its competitive
  performance in molecular prediction benchmarks.
codebase_url: https://github.com/GraphPKU/I2GNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- I^2-GNNs
mrr: 0.0617
adjusted_mrr: 0.0411
mrr_dataset_count: 2
benchmark_categories:
- Classic
- OGB
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ZINC
  rows:
  - model: GPS
    model_key: tigt
    model_plain: GPS
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS
    model_key: ppgn++
    model_plain: GPS
    value: 0.02
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_display: Feb 2023
    date_iso: '2023-02-22'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.02
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: subgraphormer
    model_plain: GPS
    value: 0.02
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.02
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.022
    std: 0.002
    paper_value: 0.022
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.022
    at_pub_std: 0.002
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.021
    true_std: 0.001
    value_gap_source_arxiv: '2306.03561'
    value_gap_source_title: 'CIN++: Enhancing Topological Message Passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.0009999999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.021
    sort_std: 0.001
    global_rank: 4
    paper_rank: 6
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: I^2-GNNs
    model_key: i^2-gnns
    model_plain: I^2-GNNs
    value: 0.023
    std: 0.001
    paper_value: 0.023
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.023
    true_std: 0.001
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.023
    sort_std: 0.001
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested GIN*
    model_key: nested gin
    model_plain: Nested GIN*
    value: 0.029
    std: 0.001
    paper_value: 0.029
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.029
    true_std: 0.001
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.029
    sort_std: 0.001
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.036
    std: 0.002
    paper_value: 0.036
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.036
    true_std: 0.002
    value_gap_source_arxiv: '2302.11556'
    value_gap_source_title: Equivariant Polynomials for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.036
    sort_std: 0.002
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN-Small
    model_key: cin-small
    model_plain: CIN-Small
    value: 0.044
    std: 0.003
    paper_value: 0.044
    paper_std: 0.003
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.044
    at_pub_std: 0.003
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-06-23'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.044
    true_std: 0.003
    value_gap_source_arxiv: '2106.12575'
    value_gap_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.044
    sort_std: 0.003
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN*
    model_key: gin
    model_plain: GIN*
    value: 0.088
    std: 0.002
    paper_value: 0.088
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: fuzzy match to zinc 250k (score=100)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Uses the canonical 250K split for ZINC.
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.088
    at_pub_std: 0.002
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.088
    true_std: 0.002
    value_gap_source_arxiv: '2302.11556'
    value_gap_source_title: Equivariant Polynomials for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.088
    sort_std: 0.002
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: ogbg-molhiv
  rows:
  - model: SigGate-GT
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: SigGate-GT
    value: 0.8476
    std: 0.0002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: mixed
    feature_source_evidence: Mixing pharmacophoric (FCFP) and structural (ECFP) fingerprints...
      GNNs contributing only 12%
    is_global_top: true
    global_rank: 1
    sort_value: 0.8476
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: hyperfusion
    model_plain: SigGate-GT
    value: 0.8475
    std: 0.0003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8475
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SigGate-GT
    model_key: pas+fps
    model_plain: SigGate-GT
    value: 0.842
    std: 0.0015
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: unknown
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.842
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.8094
    std: 0.0057
    paper_value: 0.8094
    paper_std: 0.0057
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8094
    true_std: 0.006
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8094
    sort_std: 0.006
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSN
    model_key: gsn
    model_plain: GSN
    value: 0.8039
    std: 0.009
    paper_value: 0.8039
    paper_std: 0.009
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.779
    at_pub_std: 0.001
    at_pub_source_arxiv: '2202.00529'
    at_pub_source_title: Molecular Representation Learning via Heterogeneous Motif
      Graph Neural Networks
    at_pub_source_date_iso: '2022-02-01'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.024899999999999922
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8039
    true_std: 0.009
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8039
    sort_std: 0.009
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Molecular Representation Learning via Heterogeneous Motif
      Graph Neural Networks
    comparison_source_arxiv: '2202.00529'
    is_best: false
    is_std_outlier: false
  - model: CIN-Small
    model_key: cin-small
    model_plain: CIN-Small
    value: 0.8005
    std: 0.0104
    paper_value: 0.8005
    paper_std: 0.0104
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8005
    true_std: 0.0104
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8005
    sort_std: 0.0104
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
  - model: SUN (EGO)
    model_key: sun (ego)
    model_plain: SUN (EGO)
    value: 0.8003
    std: 0.0055
    paper_value: 0.8003
    paper_std: 0.0055
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8003
    true_std: 0.0055
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8003
    sort_std: 0.0055
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.797
    std: 0.0097
    paper_value: 0.797
    paper_std: 0.0097
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.797
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.797
    true_std: 0.0097
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.0097
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNNAK+
    model_key: gnnak+
    model_plain: GNNAK+
    value: 0.7961
    std: 0.0119
    paper_value: 0.7961
    paper_std: 0.0119
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7961
    true_std: 0.0119
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7961
    sort_std: 0.0119
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
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.7905
    std: 0.0132
    paper_value: 0.7905
    paper_std: 0.0132
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.7905
    at_pub_std: 0.0132
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7905
    true_std: 0.0132
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7905
    sort_std: 0.0132
    global_rank: 68
    paper_rank: 68
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.788
    std: 0.0082
    paper_value: 0.788
    paper_std: 0.0082
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.788
    at_pub_std: 0.008
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.0082
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.0082
    global_rank: 74
    paper_rank: 74
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: I^2-GNNs
    model_key: i^2-gnns
    model_plain: I^2-GNNs
    value: 0.7868
    std: 0.0093
    paper_value: 0.7868
    paper_std: 0.0093
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7868
    true_std: 0.0093
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7868
    sort_std: 0.0093
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Nested GIN*
    model_key: nested gin
    model_plain: Nested GIN*
    value: 0.7834
    std: 0.0186
    paper_value: 0.7834
    paper_std: 0.0186
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7834
    true_std: 0.0186
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7834
    sort_std: 0.0186
    global_rank: 92
    paper_rank: 92
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN*
    model_key: gin
    model_plain: GIN*
    value: 0.7707
    std: 0.0149
    paper_value: 0.7707
    paper_std: 0.0149
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: 0.778
    at_pub_std: 0.0182
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.007299999999999973
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.778
    true_std: 0.0182
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.007299999999999973
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.0182
    global_rank: 120
    paper_rank: 162
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepLRP
    model_key: deeplrp
    model_plain: DeepLRP
    value: 0.7719
    std: 0.014
    paper_value: 0.7719
    paper_std: 0.014
    metric: ROC-AUC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: OGB scaffold split
    date: Oct 22, 2022
    date_display: Oct 2022
    date_iso: '2022-10-22'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-22'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7719
    true_std: 0.014
    value_gap_source_arxiv: '2210.13978'
    value_gap_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7719
    sort_std: 0.014
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: OGB
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
single_proposed_model: I^2-GNNs
main_figure: /figures/2210.13978/main_figure.jpegoptim.jpg
---

