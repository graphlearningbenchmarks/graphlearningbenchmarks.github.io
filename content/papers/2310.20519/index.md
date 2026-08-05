---
title: Enhancing Graph Neural Networks with Quantum Computed Encodings
arxiv_id: '2310.20519'
source_url: ''
authors:
- name: Slimane Thabet
  orcid: null
  s2_author_id: '2264372370'
  s2_url: null
- name: Romain Fouilland
  orcid: null
  s2_author_id: '2188244062'
  s2_url: null
- name: Mehdi Djellabi
  orcid: null
  s2_author_id: '2380528479'
  s2_url: null
- name: Igor Sokolov
  orcid: null
  s2_author_id: '2264125151'
  s2_url: null
- name: Sachin Kasture
  orcid: null
  s2_author_id: '2264492832'
  s2_url: null
- name: L. Henry
  orcid: null
  s2_author_id: '145746091'
  s2_url: null
- name: L. Henriet
  orcid: null
  s2_author_id: '103072467'
  s2_url: null
published_date: Oct 31, 2023
published_date_iso: '2023-10-31'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Transformers are increasingly employed for graph data, demonstrating competitive
  performance in diverse tasks. To incorporate graph information into these models,
  it is essential to enhance node and edge features with positional encodings. In
  this work, we propose novel families of positional encodings tailored for graph
  transformers. These encodings leverage the long-range correlations inherent in quantum
  systems, which arise from mapping the topology of a graph onto interactions between
  qubits in a quantum computer. Our inspiration stems from the recent advancements
  in quantum processing units, which offer computational capabilities beyond the reach
  of classical hardware. We prove that some of these quantum features are theoretically
  more expressive for certain graphs than the commonly used relative random walk probabilities.
  Empirically, we show that the performance of state-of-the-art models can be improved
  on standard benchmarks and large-scale datasets by computing tractable versions
  of quantum features. Our findings highlight the potential of leveraging quantum
  computing capabilities to potentially enhance the performance of transformers in
  handling graph data.
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
- OGB
- Quantum Chemistry
- GNNBenchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 4
  total: 6
task_categories:
- graph_classification
- graph_regression
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id005
  dataset: CIFAR10
  rows:
  - model: Tango_GPS
    model_key: randalign
    model_plain: Tango_GPS
    value: 0.7942
    std: 0.00072
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: Apr 15, 2024
    date_display: Apr 2024
    date_iso: '2024-04-15'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7942
    sort_std: 0.00072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: differential encoding
    model_plain: Tango_GPS
    value: 0.79067
    std: 0.00269
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    venue: IEEE Transactions on Big Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.79067
    sort_std: 0.00269
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ppgt
    model_plain: Tango_GPS
    value: 0.7856
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7856
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.76468
    std: 0.00881
    paper_value: 0.76468
    paper_std: 0.00881
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76468
    true_std: 0.00881
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76468
    sort_std: 0.00881
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.76442
    std: 0.0107
    paper_value: 0.76442
    paper_std: 0.0107
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.76442
    sort_std: 0.0107
    global_rank: 8
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
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.76347
    std: 0.00704
    paper_value: 0.76347
    paper_std: 0.00704
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.76347
    sort_std: 0.00704
    global_rank: 10
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
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.72838
    std: 0.00417
    paper_value: 0.72838
    paper_std: 0.00417
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7284
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 2.0000000000020002e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7284
    true_std: 0.0042
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.7284
    sort_std: 0.0042
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.7219
    std: 0.0013
    paper_value: 0.7219
    paper_std: 0.0013
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7219
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7239
    true_std: 0.0038
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.7239
    sort_std: 0.0038
    global_rank: 41
    paper_rank: 46
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.72298
    std: 0.00356
    paper_value: 0.72298
    paper_std: 0.00356
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.72298
    at_pub_std: 0.00356
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.72356
    true_std: 0.00323
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: 0.0005800000000000249
    has_value_note: false
    value_note: ''
    sort_value: 0.72356
    sort_std: 0.00323
    global_rank: 43
    paper_rank: 45
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.67312
    std: 0.00311
    paper_value: 0.67312
    paper_std: 0.00311
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7133
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.040179999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7133
    true_std: 0.0039
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.040179999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: 0.0039
    global_rank: 57
    paper_rank: 85
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.68702
    std: 0.00409
    paper_value: 0.68702
    paper_std: 0.00409
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.68702
    at_pub_std: 0.00409
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.68702
    true_std: 0.00409
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.68702
    sort_std: 0.00409
    global_rank: 78
    paper_rank: 78
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
    value: 0.64223
    std: 0.00455
    paper_value: 0.64223
    paper_std: 0.00455
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6611
    at_pub_std: 0.0098
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.018870000000000053
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6611
    true_std: 0.0098
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.018870000000000053
    has_value_note: false
    value_note: ''
    sort_value: 0.6611
    sort_std: 0.0098
    global_rank: 98
    paper_rank: 109
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.55255
    std: 0.01527
    paper_value: 0.55255
    paper_std: 0.01527
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.651
    at_pub_std: 0.005
    at_pub_source_arxiv: '2107.04755'
    at_pub_source_title: 'Beyond Low-pass Filtering: Graph Convolutional Networks
      with Automatic Filtering'
    at_pub_source_date_iso: '2021-07-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.09845000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5982
    true_std: 0.0033
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.04564999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5982
    sort_std: 0.0033
    global_rank: 118
    paper_rank: 126
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Low-pass Filtering: Graph Convolutional Networks
      with Automatic Filtering'
    comparison_source_arxiv: '2107.04755'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5571
    std: 0.00381
    paper_value: 0.5571
    paper_std: 0.00381
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5839
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.026799999999999935
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5839
    true_std: 0.0073
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: false
    value_gap: 0.026799999999999935
    has_value_note: false
    value_note: ''
    sort_value: 0.5839
    sort_std: 0.0073
    global_rank: 121
    paper_rank: 125
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    comparison_source_arxiv: '2110.03753'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id006
  dataset: CLUSTER
  rows:
  - model: Tango_GPS
    model_key: grpe-small
    model_plain: Tango_GPS
    value: 0.81586
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 489.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.81586
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.80113
    std: 0.00138
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.80113
    sort_std: 0.00138
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.80026
    std: 0.00277
    paper_value: 0.80026
    paper_std: 0.00277
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8003
    true_std: 0.0028
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 4.0000000000040004e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8003
    sort_std: 0.0028
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.79777
    std: 0.00171
    paper_value: 0.79777
    paper_std: 0.00171
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.79777
    sort_std: 0.00171
    global_rank: 4
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.79232
    std: 0.00348
    paper_value: 0.79232
    paper_std: 0.00348
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.79232
    at_pub_std: 0.00348
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.79232
    true_std: 0.00348
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.79232
    sort_std: 0.00348
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.78895
    std: 0.001145
    paper_value: 0.78895
    paper_std: 0.001145
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.78895
    sort_std: 0.001145
    global_rank: 6
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.78016
    std: 0.0018
    paper_value: 0.78016
    paper_std: 0.0018
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.78016
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7802
    true_std: 0.0018
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 4.0000000000040004e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.7802
    sort_std: 0.0018
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: K-Subgraph SAT
    model_key: k-subgraph sat
    model_plain: K-Subgraph SAT
    value: 0.77856
    std: 0.00104
    paper_value: 0.77856
    paper_std: 0.00104
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.77856
    at_pub_std: 0.00104
    at_pub_source_arxiv: '2202.03036'
    at_pub_source_title: Structure-Aware Transformer for Graph Representation Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.77856
    true_std: 0.00104
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.77856
    sort_std: 0.00104
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
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.76691
    std: 0.0065
    paper_value: 0.76691
    paper_std: 0.0065
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76691
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76691
    true_std: 0.0065
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76691
    sort_std: 0.0065
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7384
    std: 0.00326
    paper_value: 0.7384
    paper_std: 0.00326
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76082
    at_pub_std: 0.00196
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022420000000000107
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76082
    true_std: 0.00196
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.022420000000000107
    has_value_note: false
    value_note: ''
    sort_value: 0.76082
    sort_std: 0.00196
    global_rank: 55
    paper_rank: 63
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    comparison_source_arxiv: '2201.12787'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.70587
    std: 0.00447
    paper_value: 0.70587
    paper_std: 0.00447
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.70587
    at_pub_std: 0.00447
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.70587
    true_std: 0.00447
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.70587
    sort_std: 0.00447
    global_rank: 69
    paper_rank: 69
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
    value: 0.68498
    std: 0.00976
    paper_value: 0.68498
    paper_std: 0.00976
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.69026
    at_pub_std: 0.01372
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.005279999999999951
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.69026
    true_std: 0.01372
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.005279999999999951
    has_value_note: false
    value_note: ''
    sort_value: 0.69026
    sort_std: 0.01372
    global_rank: 71
    paper_rank: 72
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.64716
    std: 0.01553
    paper_value: 0.64716
    paper_std: 0.01553
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.64716
    at_pub_std: 0.01553
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64716
    true_std: 0.01553
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64716
    sort_std: 0.01553
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: MNIST
  rows:
  - model: Tango_GPS
    model_key: schrödinger gnn
    model_plain: Tango_GPS
    value: 0.9913
    std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9913
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: cnn
    model_plain: Tango_GPS
    value: 0.9907
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9907
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: mpnn
    model_plain: Tango_GPS
    value: 0.9895
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
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9895
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.9734
    std: 0.00143
    paper_value: 0.9734
    paper_std: 0.00143
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9824
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.98552
    true_std: 0.00023
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.012119999999999909
    has_value_note: false
    value_note: ''
    sort_value: 0.98552
    sort_std: 0.00023
    global_rank: 11
    paper_rank: 85
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.96485
    std: 0.00252
    paper_value: 0.96485
    paper_std: 0.00252
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9723
    at_pub_std: null
    at_pub_source_arxiv: '2202.02296'
    at_pub_source_title: Graph-Coupled Oscillator Networks
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007450000000000068
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9833
    true_std: 0.0011
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: 0.018449999999999966
    has_value_note: false
    value_note: ''
    sort_value: 0.9833
    sort_std: 0.0011
    global_rank: 31
    paper_rank: 103
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Coupled Oscillator Networks
    comparison_source_arxiv: '2202.02296'
    is_best: false
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.98204
    std: 0.00048
    paper_value: 0.98204
    paper_std: 0.00048
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.98204
    sort_std: 0.00048
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.98173
    std: 0.00087
    paper_value: 0.98173
    paper_std: 0.00087
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98173
    at_pub_std: 0.00087
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98173
    true_std: 0.00087
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98173
    sort_std: 0.00087
    global_rank: 46
    paper_rank: 46
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT (our run)
    model_key: grit (our run)
    model_plain: GRIT (our run)
    value: 0.98164
    std: 0.00054
    paper_value: 0.98164
    paper_std: 0.00054
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.98164
    sort_std: 0.00054
    global_rank: 48
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
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.98108
    std: 0.00111
    paper_value: 0.98108
    paper_std: 0.00111
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.98108
    sort_std: 0.00111
    global_rank: 55
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.98051
    std: 0.00126
    paper_value: 0.98051
    paper_std: 0.00126
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98051
    at_pub_std: 0.00126
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.98082
    true_std: 0.00114
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: 0.00031000000000003247
    has_value_note: false
    value_note: ''
    sort_value: 0.98082
    sort_std: 0.00114
    global_rank: 56
    paper_rank: 57
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.95535
    std: 0.00205
    paper_value: 0.95535
    paper_std: 0.00205
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.965
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009649999999999936
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.97553
    true_std: 0.00034
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.020179999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.97553
    sort_std: 0.00034
    global_rank: 81
    paper_rank: 114
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.90705
    std: 0.00218
    paper_value: 0.90705
    paper_std: 0.00218
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9269
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.13350'
    at_pub_source_title: A Generalization of ViT/MLP-Mixer to Graphs
    at_pub_source_date_iso: '2022-12-27'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.019849999999999923
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.94051
    true_std: 0.00052
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.033459999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.94051
    sort_std: 0.00052
    global_rank: 129
    paper_rank: 133
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Generalization of ViT/MLP-Mixer to Graphs
    comparison_source_arxiv: '2212.13350'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id007
  dataset: PATTERN
  rows:
  - model: Tango_GPS
    model_key: deepgraph (48)
    model_plain: Tango_GPS
    value: 0.90657
    std: 0.00062
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2303.00579'
    title: Are More Layers Beneficial to Graph Transformers?
    date: Mar 1, 2023
    date_display: Mar 2023
    date_iso: '2023-03-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/zhao-ht/DeepGraph
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.90657
    sort_std: 0.00062
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRIT (our run)
    model_key: grit (our run)
    model_plain: GRIT (our run)
    value: 0.90405
    std: 0.00232
    paper_value: 0.90405
    paper_std: 0.00232
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.90405
    sort_std: 0.00232
    global_rank: 2
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
    is_best: true
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.90165
    std: 0.00446
    paper_value: 0.90165
    paper_std: 0.00446
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.90165
    sort_std: 0.00446
    global_rank: 2
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
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ppgt
    model_plain: Tango_GPS
    value: 0.89752
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.89752
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ckgcn
    model_plain: Tango_GPS
    value: 0.88661
    std: 0.00143
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.88661
    sort_std: 0.00143
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.87205
    std: 0.0004
    paper_value: 0.87205
    paper_std: 0.0004
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.87205
    sort_std: 0.0004
    global_rank: 5
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
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.8685
    std: 0.00057
    paper_value: 0.8685
    paper_std: 0.00057
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8685
    at_pub_std: 0.00057
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8685
    true_std: 0.057
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8685
    sort_std: 0.057
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: K-Subgraph SAT
    model_key: k-subgraph sat
    model_plain: K-Subgraph SAT
    value: 0.86848
    std: 0.00037
    paper_value: 0.86848
    paper_std: 0.00037
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86848
    at_pub_std: 0.00037
    at_pub_source_arxiv: '2202.03036'
    at_pub_source_title: Structure-Aware Transformer for Graph Representation Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86848
    true_std: 0.037
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86848
    sort_std: 0.037
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.86821
    std: 0.0002
    paper_value: 0.86821
    paper_std: 0.0002
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86821
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86821
    true_std: 0.02
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86821
    sort_std: 0.02
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.86685
    std: 0.00059
    paper_value: 0.86685
    paper_std: 0.00059
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86685
    at_pub_std: 0.00059
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86685
    true_std: 0.059
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86685
    sort_std: 0.059
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.8668
    std: 0.00034
    paper_value: 0.8668
    paper_std: 0.00034
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8668
    at_pub_std: 0.00034
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8668
    true_std: 0.034
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8668
    sort_std: 0.034
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.86581
    std: 0.00037
    paper_value: 0.86581
    paper_std: 0.00037
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86581
    at_pub_std: 0.00037
    at_pub_source_arxiv: '2202.03036'
    at_pub_source_title: Structure-Aware Transformer for Graph Representation Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86581
    true_std: 0.037
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86581
    sort_std: 0.037
    global_rank: 54
    paper_rank: 54
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
    value: 0.71892
    std: 0.00334
    paper_value: 0.71892
    paper_std: 0.00334
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85614
    at_pub_std: 0.032
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.13722
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.85614
    true_std: 0.032
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.13722
    has_value_note: false
    value_note: ''
    sort_value: 0.85614
    sort_std: 0.032
    global_rank: 84
    paper_rank: 116
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.85387
    std: 0.00136
    paper_value: 0.85387
    paper_std: 0.00136
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8559
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2010.05421'
    at_pub_source_title: Factorizable Graph Convolutional Networks
    at_pub_source_date_iso: '2020-10-12'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.0020299999999999763
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8559
    true_std: 0.0001
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.0020299999999999763
    has_value_note: false
    value_note: ''
    sort_value: 0.8559
    sort_std: 0.0001
    global_rank: 85
    paper_rank: 92
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Factorizable Graph Convolutional Networks
    comparison_source_arxiv: '2010.05421'
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.85568
    std: 0.00088
    paper_value: 0.85568
    paper_std: 0.00088
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86508
    at_pub_std: 0.00085
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009399999999999964
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8557
    true_std: 0.0009
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8557
    sort_std: 0.0009
    global_rank: 88
    paper_rank: 89
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: IJCAI--23 Formatting Instructions
    comparison_source_arxiv: '2305.11424'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.78271
    std: 0.00186
    paper_value: 0.78271
    paper_std: 0.00186
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.78271
    at_pub_std: 0.00186
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.78271
    true_std: 0.186
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.78271
    sort_std: 0.186
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
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
- &id002
  dataset: PCQM4Mv2
  rows:
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.0838
    std: null
    paper_value: 0.0838
    paper_std: null
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.0838
    sort_std: null
    global_rank: 1
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
    is_best: true
    is_std_outlier: false
  - model: GRIT (our run)
    model_key: grit (our run)
    model_plain: GRIT (our run)
    value: 0.0842
    std: null
    paper_value: 0.0842
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.0842
    sort_std: null
    global_rank: 1
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
  - model: GPS-medium
    model_key: gps-medium
    model_plain: GPS-medium
    value: 0.0858
    std: null
    paper_value: 0.0858
    paper_std: null
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.0858
    sort_std: null
    global_rank: 1
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
  - model: TorchMD-NET + Pre-training
    model_key: egt-large
    model_plain: TorchMD-NET + Pre-training
    value: 0.0872
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.0872
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-NET + Pre-training
    model_key: grpe-standard
    model_plain: TorchMD-NET + Pre-training
    value: 0.0898
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.0898
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.0947
    std: null
    paper_value: 0.0947
    paper_std: null
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.0947
    sort_std: null
    global_rank: 3
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
  - model: TorchMD-NET + Pre-training
    model_key: advsyngnn
    model_plain: TorchMD-NET + Pre-training
    value: 0.108
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.108
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1195
    std: null
    paper_value: 0.1195
    paper_std: null
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1195
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.1218
    true_std: null
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.0023000000000000104
    has_value_note: false
    value_note: ''
    sort_value: 0.1218
    sort_std: null
    global_rank: 7
    paper_rank: 6
    rank_delta: -1
    rank_delta_abs: 1
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.0864
    std: null
    paper_value: 0.0864
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0864
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.1328
    true_std: null
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.0464
    has_value_note: false
    value_note: ''
    sort_value: 0.1328
    sort_std: null
    global_rank: 11
    paper_rank: 1
    rank_delta: -10
    rank_delta_abs: 10
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.1195
    std: null
    paper_value: 0.1195
    paper_std: null
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1379
    at_pub_std: null
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0184
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1398
    true_std: null
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.020300000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.1398
    sort_std: null
    global_rank: 18
    paper_rank: 6
    rank_delta: -12
    rank_delta_abs: 12
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    comparison_source_arxiv: '2205.12454'
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
- &id003
  dataset: QM7b
  rows:
  - model: ISGR
    model_key: ani-1
    model_plain: ISGR
    value: 2.86
    std: 0.25
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 2.86
    sort_std: 0.25
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ISGR
    model_key: dtnn
    model_plain: ISGR
    value: 8.8
    std: 3.5
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 8.8
    sort_std: 3.5
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ISGR
    model_key: hanet
    model_plain: ISGR
    value: 9.5
    std: 0.71
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04786'
    title: Fast Haar Transforms for Graph Neural Networks
    date: Jul 10, 2019
    date_display: Jul 2019
    date_iso: '2019-07-10'
    venue: Neural Networks
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 9.5
    sort_std: 0.71
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS (4, 2, 128) LE
    model_key: gps (4, 2, 128) le
    model_plain: GPS (4, 2, 128) LE
    value: 14.03
    std: null
    paper_value: 14.03
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 14.03
    sort_std: null
    global_rank: 6
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
  - model: SAGE LE+RW
    model_key: sage le+rw
    model_plain: SAGE LE+RW
    value: 14.13
    std: null
    paper_value: 14.13
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 14.13
    sort_std: null
    global_rank: 6
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
  - model: GPS LE+RW
    model_key: gps le+rw
    model_plain: GPS LE+RW
    value: 14.66
    std: null
    paper_value: 14.66
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 14.66
    sort_std: null
    global_rank: 6
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
  - model: GPS LE
    model_key: gps le
    model_plain: GPS LE
    value: 14.68
    std: null
    paper_value: 14.68
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 14.68
    sort_std: null
    global_rank: 6
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
  - model: SAGE RW
    model_key: sage rw
    model_plain: SAGE RW
    value: 14.97
    std: null
    paper_value: 14.97
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 14.97
    sort_std: null
    global_rank: 6
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
  - model: GPS (4, 2, 128) Q
    model_key: gps (4, 2, 128) q
    model_plain: GPS (4, 2, 128) Q
    value: 15.36
    std: null
    paper_value: 15.36
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 15.36
    sort_std: null
    global_rank: 6
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
  - model: SAGE Q
    model_key: sage q
    model_plain: SAGE Q
    value: 15.85
    std: null
    paper_value: 15.85
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 15.85
    sort_std: null
    global_rank: 6
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
  - model: GPS Q
    model_key: gps q
    model_plain: GPS Q
    value: 16.15
    std: null
    paper_value: 16.15
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 16.15
    sort_std: null
    global_rank: 6
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
  - model: GPS RW
    model_key: gps rw
    model_plain: GPS RW
    value: 16.18
    std: null
    paper_value: 16.18
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 16.18
    sort_std: null
    global_rank: 6
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
  - model: GPS (4, 2, 128) RW
    model_key: gps (4, 2, 128) rw
    model_plain: GPS (4, 2, 128) RW
    value: 16.45
    std: null
    paper_value: 16.45
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 16.45
    sort_std: null
    global_rank: 6
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
  - model: GPS No PE
    model_key: gps no pe
    model_plain: GPS No PE
    value: 32.23
    std: null
    paper_value: 32.23
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 32.23
    sort_std: null
    global_rank: 7
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
  - model: GPS (4, 2, 128) No PE
    model_key: gps (4, 2, 128) no pe
    model_plain: GPS (4, 2, 128) No PE
    value: 34.97
    std: null
    paper_value: 34.97
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 34.97
    sort_std: null
    global_rank: 8
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
  - model: SAGE LE
    model_key: sage le
    model_plain: SAGE LE
    value: 36.62
    std: null
    paper_value: 36.62
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 36.62
    sort_std: null
    global_rank: 8
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
  - model: SAGE No PE
    model_key: sage no pe
    model_plain: SAGE No PE
    value: 60.45
    std: null
    paper_value: 60.45
    paper_std: null
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
    variant_inference_reason: 'dataset: fuzzy match to qm7b (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 60.45
    sort_std: null
    global_rank: 18
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
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.023
    std: 0.001
    paper_value: 0.023
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.023
    sort_std: 0.001
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.023
    std: 0.002
    paper_value: 0.023
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.023
    sort_std: 0.002
    global_rank: 10
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
  - model: SignNet
    model_key: signnet
    model_plain: SignNet
    value: 0.024
    std: 0.003
    paper_value: 0.024
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
    source_ref: rampavsek2022recipe
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.024
    at_pub_std: 0.003
    at_pub_source_arxiv: '2302.11556'
    at_pub_source_title: Equivariant Polynomials for Graph Neural Networks
    at_pub_source_date_iso: '2023-02-22'
    at_pub_source_date_label: ICML 2023
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
    true_value: 0.024
    true_std: 0.003
    value_gap_source_arxiv: '2302.11556'
    value_gap_source_title: Equivariant Polynomials for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.024
    sort_std: 0.003
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
  - model: GRIT 1-CQRW
    model_key: grit 1-cqrw
    model_plain: GRIT 1-CQRW
    value: 0.025
    std: 0.003
    paper_value: 0.025
    paper_std: 0.003
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
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
    sort_value: 0.025
    sort_std: 0.003
    global_rank: 14
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
  - model: Graphormer
    model_key: graphormer
    model_plain: Graphormer
    value: 0.052
    std: 0.005
    paper_value: 0.052
    paper_std: 0.005
    metric: MAE
    higher_is_better: false
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0309
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2305.15747'
    at_pub_source_title: Union Subgraph Neural Networks
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2025-01-30'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.021099999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.025
    true_std: 0.004
    value_gap_source_arxiv: '2501.18739'
    value_gap_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    value_gap_source_is_current_paper: false
    value_gap: 0.026999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.025
    sort_std: 0.004
    global_rank: 12
    paper_rank: 31
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Union Subgraph Neural Networks
    comparison_source_arxiv: '2305.15747'
    is_best: false
    is_std_outlier: false
  - model: Graphormer-GD
    model_key: graphormer-gd
    model_plain: Graphormer-GD
    value: 0.025
    std: 0.004
    paper_value: 0.025
    paper_std: 0.004
    metric: MAE
    higher_is_better: false
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.025
    true_std: 0.004
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.025
    sort_std: 0.004
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
  - model: Graphormer-URPE
    model_key: graphormer-urpe
    model_plain: Graphormer-URPE
    value: 0.028
    std: 0.002
    paper_value: 0.028
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.028
    true_std: 0.002
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.028
    sort_std: 0.002
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
  - model: GIN
    model_key: gin
    model_plain: GIN
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.111
    std: 0.002
    paper_value: 0.111
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.384
    at_pub_std: 0.007
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.273
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.111
    true_std: 0.002
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.111
    sort_std: 0.002
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: How Expressive are Transformers in Spectral Domain for
      Graphs?
    comparison_source_arxiv: '2201.09332'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.113
    std: 0.002
    paper_value: 0.113
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1152
    at_pub_std: 0.001
    at_pub_source_arxiv: '2305.15747'
    at_pub_source_title: Union Subgraph Neural Networks
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0021999999999999936
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.113
    true_std: 0.002
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.113
    sort_std: 0.002
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.126
    std: 0.003
    paper_value: 0.126
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1205
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2305.15747'
    at_pub_source_title: Union Subgraph Neural Networks
    at_pub_source_date_iso: '2023-05-25'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-05-25'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.005500000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.1205
    true_std: 0.0034
    value_gap_source_arxiv: '2305.15747'
    value_gap_source_title: Union Subgraph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.005500000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.1205
    sort_std: 0.0034
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: OGB
  datasets:
  - *id002
- benchmark: Quantum Chemistry
  datasets:
  - *id003
- benchmark: GNNBenchmark
  datasets:
  - *id004
  - *id005
  - *id006
  - *id007
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CLUSTER
      dataset_slug: cluster
    - dataset: PATTERN
      dataset_slug: pattern
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
    - dataset: PCQM4Mv2
      dataset_slug: pcqm4mv2
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM7b
      dataset_slug: qm7b
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
    - dataset: CIFAR10
      dataset_slug: cifar10
main_figure: /figures/2310.20519/main_figure.jpegoptim.jpg
---

