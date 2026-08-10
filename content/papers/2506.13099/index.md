---
title: Dynamic Graph Condensation
arxiv_id: '2506.13099'
source_url: ''
authors:
- name: Dong Chen
  orcid: null
  s2_author_id: '2296169074'
  s2_url: null
- name: Shuai Zheng
  orcid: null
  s2_author_id: '2111073268'
  s2_url: null
- name: Yeyu Yan
  orcid: null
  s2_author_id: '2149251040'
  s2_url: null
- name: Muhao Xu
  orcid: null
  s2_author_id: '2143583021'
  s2_url: null
- name: Zhenfeng Zhu
  orcid: null
  s2_author_id: '2157606419'
  s2_url: null
- name: Yao Zhao
  orcid: null
  s2_author_id: '2261899613'
  s2_url: null
- name: Kunlun He
  orcid: null
  s2_author_id: '2367269800'
  s2_url: null
published_date: Jun 16, 2025
published_date_iso: '2025-06-16'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Recent research on deep graph learning has shifted from static to dynamic
  graphs, motivated by the evolving behaviors observed in complex real-world systems.
  However, the temporal extension in dynamic graphs poses significant data efficiency
  challenges, including increased data volume, high spatiotemporal redundancy, and
  reliance on costly dynamic graph neural networks (DGNNs). To alleviate the concerns,
  we pioneer the study of dynamic graph condensation (DGC), which aims to substantially
  reduce the scale of dynamic graphs for data-efficient DGNN training. Accordingly,
  we propose DyGC, a novel framework that condenses the real dynamic graph into a
  compact version while faithfully preserving the inherent spatiotemporal characteristics.
  Specifically, to endow synthetic graphs with realistic evolving structures, a novel
  spiking structure generation mechanism is introduced. It draws on the dynamic behavior
  of spiking neurons to model temporally-aware connectivity in dynamic graphs. Given
  the tightly coupled spatiotemporal dependencies, DyGC proposes a tailored distribution
  matching approach that first constructs a semantically rich state evolving field
  for dynamic graphs, and then performs fine-grained spatiotemporal state alignment
  to guide the optimization of the condensed graph. Experiments across multiple dynamic
  graph datasets and representative DGNN architectures demonstrate the effectiveness
  of DyGC. Notably, our method retains up to 96.2\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DyGC
mrr: 0.0068
adjusted_mrr: 0.0023
mrr_dataset_count: 1
benchmark_categories:
- Classic
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
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
    value: 0.946
    std: 0.0031
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_display: Oct 2023
    date_iso: '2023-10-25'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 21
    sort_value: 0.946
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.741
    std: 0.011
    paper_value: 0.741
    paper_std: 0.011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9384
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2307.08430'
    at_pub_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    at_pub_source_date_iso: '2023-07-17'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.19740000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9384
    true_std: 0.0053
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.19740000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9384
    sort_std: 0.0053
    global_rank: 34
    paper_rank: 159
    rank_delta: 125
    rank_delta_abs: 125
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    comparison_source_arxiv: '2307.08430'
    is_best: false
    is_std_outlier: false
  - model: Whole
    model_key: whole
    model_plain: Whole
    value: 0.792
    std: 0.003
    paper_value: 0.792
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on full graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.792
    true_std: 0.003
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.003
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
  - model: DyGC
    model_key: dygc
    model_plain: DyGC
    value: 0.782
    std: 0.003
    paper_value: 0.782
    paper_std: 0.003
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
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.782
    true_std: 0.003
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.782
    sort_std: 0.003
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SimGC
    model_key: simgc
    model_plain: SimGC
    value: 0.74
    std: 0.008
    paper_value: 0.74
    paper_std: 0.008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.74
    true_std: 0.008
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.74
    sort_std: 0.008
    global_rank: 161
    paper_rank: 161
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CGC
    model_key: cgc
    model_plain: CGC
    value: 0.729
    std: 0.01
    paper_value: 0.729
    paper_std: 0.01
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: 0.01
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.01
    global_rank: 164
    paper_rank: 164
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
    value: 0.715
    std: 0.023
    paper_value: 0.715
    paper_std: 0.023
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.023
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.023
    global_rank: 167
    paper_rank: 167
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
    value: 0.697
    std: 0.017
    paper_value: 0.697
    paper_std: 0.017
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.697
    true_std: 0.017
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.697
    sort_std: 0.017
    global_rank: 172
    paper_rank: 172
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
    value: 0.689
    std: 0.024
    paper_value: 0.689
    paper_std: 0.024
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.689
    true_std: 0.024
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.024
    global_rank: 173
    paper_rank: 173
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
    value: 0.689
    std: 0.014
    paper_value: 0.689
    paper_std: 0.014
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Temporal node classification on condensed graph
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.689
    true_std: 0.014
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.689
    sort_std: 0.014
    global_rank: 174
    paper_rank: 174
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
    value: 0.6447
    std: 0.0136
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.07365'
    title: 'GraphControl: Adding Conditional Control to Universal Graph Pre-trained
      Models for Graph Domain Transfer Learning'
    date: Oct 11, 2023
    date_display: Oct 2023
    date_iso: '2023-10-11'
    venue: The Web Conference
    codebase_url: https://github.com/wykk00/GraphControl
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 179
    sort_value: 0.6447
    sort_std: 0.0136
    comparison_type: global_top
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
- &id001
  dataset: Reddit
  is_multi_metric: true
  rows:
  - model: DyGC
    model_key: dygc
    model_plain: DyGC
    metric_values:
    - null
    - 0.461
    - 0.457
    metric_stds:
    - null
    - 0.006
    - 0.006
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.461
    sort_std: 0.006
    true_value: 0.461
    true_std: 0.006
    paper_value: 0.461
    paper_std: 0.006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: K-Center
    model_key: k-center
    model_plain: K-Center
    metric_values:
    - null
    - 0.422
    - null
    metric_stds:
    - null
    - 0.009
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.422
    sort_std: 0.009
    true_value: 0.422
    true_std: 0.009
    paper_value: 0.422
    paper_std: 0.009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: Herding
    model_key: herding
    model_plain: Herding
    metric_values:
    - null
    - 0.413
    - null
    metric_stds:
    - null
    - 0.007
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.413
    sort_std: 0.007
    true_value: 0.413
    true_std: 0.007
    paper_value: 0.413
    paper_std: 0.007
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: Random
    model_key: random
    model_plain: Random
    metric_values:
    - null
    - 0.392
    - null
    metric_stds:
    - null
    - 0.009
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.392
    sort_std: 0.009
    true_value: 0.392
    true_std: 0.009
    paper_value: 0.392
    paper_std: 0.009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: CGC
    model_key: cgc
    model_plain: CGC
    metric_values:
    - null
    - 0.389
    - null
    metric_stds:
    - null
    - 0.011
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.389
    sort_std: 0.011
    true_value: 0.389
    true_std: 0.011
    paper_value: 0.389
    paper_std: 0.011
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: GCDM
    model_key: gcdm
    model_plain: GCDM
    metric_values:
    - null
    - 0.327
    - null
    metric_stds:
    - null
    - 0.01
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.327
    sort_std: 0.01
    true_value: 0.327
    true_std: 0.01
    paper_value: 0.327
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: SimGC
    model_key: simgc
    model_plain: SimGC
    metric_values:
    - null
    - 0.308
    - null
    metric_stds:
    - null
    - 0.009
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.308
    sort_std: 0.009
    true_value: 0.308
    true_std: 0.009
    paper_value: 0.308
    paper_std: 0.009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: GCond
    model_key: gcond
    model_plain: GCond
    metric_values:
    - null
    - 0.288
    - null
    metric_stds:
    - null
    - 0.014
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.288
    sort_std: 0.014
    true_value: 0.288
    true_std: 0.014
    paper_value: 0.288
    paper_std: 0.014
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2506.13099'
    value_gap_source_title: Dynamic Graph Condensation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
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
    date: Jun 16, 2025
    date_display: Jun 2025
    date_iso: '2025-06-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  metrics:
  - F1
  - Micro-F1
  - Macro-F1
  primary_metric: F1
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - Micro-F1
  - Macro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
single_proposed_model: DyGC
main_figure: /figures/2506.13099/main_figure.jpegoptim.jpg
---

