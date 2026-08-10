---
title: Equivariant Matrix Function Neural Networks
arxiv_id: '2310.10434'
source_url: ''
authors:
- name: Ilyes Batatia
  orcid: null
  s2_author_id: '2040711516'
  s2_url: null
- name: L. Schaaf
  orcid: null
  s2_author_id: '2258711301'
  s2_url: null
- name: Huajie Chen
  orcid: null
  s2_author_id: '2259803438'
  s2_url: null
- name: Gábor Csányi
  orcid: null
  s2_author_id: '2258710656'
  s2_url: null
- name: Christoph Ortner
  orcid: null
  s2_author_id: '2237990676'
  s2_url: null
- name: Felix A. Faber
  orcid: null
  s2_author_id: '2385424049'
  s2_url: null
published_date: Oct 16, 2023
published_date_iso: '2023-10-16'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Graph Neural Networks (GNNs), especially message-passing neural networks
  (MPNNs), have emerged as powerful architectures for learning on graphs in diverse
  applications. However, MPNNs face challenges when modeling non-local interactions
  in graphs such as large conjugated molecules, and social networks due to oversmoothing
  and oversquashing. Although Spectral GNNs and traditional neural networks such as
  recurrent neural networks and transformers mitigate these challenges, they often
  lack generalizability, or fail to capture detailed structural relationships or symmetries
  in the data. To address these concerns, we introduce Matrix Function Neural Networks
  (MFNs), a novel architecture that parameterizes non-local interactions through analytic
  matrix equivariant functions. Employing resolvent expansions offers a straightforward
  implementation and the potential for linear scaling with system size. The MFN architecture
  achieves state-of-the-art performance in standard graph benchmarks, such as the
  ZINC and TU datasets, and is able to capture intricate non-local interactions in
  quantum systems, paving the way to new state-of-the-art force fields. The code and
  the datasets will be made public.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
- MFN
mrr: 0.0423
adjusted_mrr: 0.0423
mrr_dataset_count: 3
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id003
  dataset: ENZYMES
  rows:
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.7866
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7866
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MemGNN
    model_key: memgnn
    model_plain: MemGNN
    value: 0.755
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.755
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGW SP
    model_key: tfgw sp (l=2)
    model_plain: TFGW SP
    value: 0.751
    std: 0.05
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.751
    sort_std: 0.05
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PDF
    model_key: pdf
    model_plain: PDF
    value: 0.735
    std: 0.0639
    paper_value: 0.735
    paper_std: 0.0639
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.472
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.735
    at_pub_std: 0.0639
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.735
    true_std: 0.0639
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.735
    sort_std: 0.0639
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MFN
    model_key: mfn
    model_plain: MFN
    value: 0.729
    std: 0.0755
    paper_value: 0.729
    paper_std: 0.0755
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: 0.0755
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.0755
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7
    std: 0.04944
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.7
    sort_std: 0.04944
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.582
    std: 0.06
    paper_value: 0.582
    paper_std: 0.06
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.68167
    at_pub_std: 0.05449
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.09967000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.68167
    true_std: 0.05449
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.09967000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.68167
    sort_std: 0.05449
    global_rank: 27
    paper_rank: 121
    rank_delta: 94
    rank_delta_abs: 94
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
    value: 0.67667
    std: 0.05831
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.67667
    sort_std: 0.05831
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.55833
    std: 0.03516
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 133
    sort_value: 0.55833
    sort_std: 0.03516
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CapsGNN
    model_key: capsgnn
    model_plain: CapsGNN
    value: 0.5467
    std: 0.0567
    paper_value: 0.5467
    paper_std: 0.0567
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.5531
    at_pub_std: 0.0423
    at_pub_source_arxiv: '2210.00084'
    at_pub_source_title: Contrastive Graph Few-Shot Learning
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.006400000000000072
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5531
    true_std: 0.0423
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.006400000000000072
    has_value_note: false
    value_note: ''
    sort_value: 0.5531
    sort_std: 0.0423
    global_rank: 136
    paper_rank: 145
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: ecc
    model_plain: ECC
    value: 0.4567
    std: null
    paper_value: 0.4567
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.535
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.07830000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.535
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07830000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.535
    sort_std: null
    global_rank: 153
    paper_rank: 187
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.5343
    std: 0.0091
    paper_value: 0.5343
    paper_std: 0.0091
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.5343
    at_pub_std: 0.0091
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5343
    true_std: 0.0091
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5343
    sort_std: 0.0091
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AWE
    model_key: awe
    model_plain: AWE
    value: 0.3577
    std: 0.0593
    paper_value: 0.3577
    paper_std: 0.0593
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.4558
    at_pub_std: 0.0211
    at_pub_source_arxiv: '2210.00084'
    at_pub_source_title: Contrastive Graph Few-Shot Learning
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.09809999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4558
    true_std: 0.0211
    value_gap_source_arxiv: '2210.00084'
    value_gap_source_title: Contrastive Graph Few-Shot Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.09809999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4558
    sort_std: 0.0211
    global_rank: 188
    paper_rank: 239
    rank_delta: 51
    rank_delta_abs: 51
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Contrastive Graph Few-Shot Learning
    comparison_source_arxiv: '2210.00084'
    is_best: false
    is_std_outlier: false
  - model: GK
    model_key: gk
    model_plain: GK
    value: 0.327
    std: 0.012
    paper_value: 0.327
    paper_std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.327
    at_pub_std: 0.012
    at_pub_source_arxiv: '1805.11921'
    at_pub_source_title: Anonymous Walk Embeddings
    at_pub_source_date_iso: '2018-05-30'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.327
    true_std: 0.012
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.327
    sort_std: 0.012
    global_rank: 252
    paper_rank: 252
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RW
    model_key: rw
    model_plain: RW
    value: 0.2416
    std: 0.0164
    paper_value: 0.2416
    paper_std: 0.0164
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.2416
    at_pub_std: 0.0164
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2416
    true_std: 0.0164
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2416
    sort_std: 0.0164
    global_rank: 292
    paper_rank: 292
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
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
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.894
    std: 0.056
    paper_value: 0.894
    paper_std: 0.056
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.933
    at_pub_std: 0.029
    at_pub_source_arxiv: '2112.00911'
    at_pub_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.039000000000000035
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 254
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PSCN
    model_key: pscn
    model_plain: PSCN
    value: 0.8895
    std: 0.044
    paper_value: 0.8895
    paper_std: 0.044
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.9263
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2020-08-12'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.036800000000000055
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9263
    true_std: 0.0421
    value_gap_source_arxiv: '2008.05089'
    value_gap_source_title: Quaternion Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.036800000000000055
    has_value_note: false
    value_note: ''
    sort_value: 0.9263
    sort_std: 0.0421
    global_rank: 56
    paper_rank: 296
    rank_delta: 240
    rank_delta_abs: 240
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.922
    std: 0.044
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 71
    sort_value: 0.922
    sort_std: 0.044
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MFN
    model_key: mfn
    model_plain: MFN
    value: 0.915
    std: 0.0735
    paper_value: 0.915
    paper_std: 0.0735
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.915
    true_std: 0.0735
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.0735
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PPGNN
    model_key: ppgnn
    model_plain: PPGNN
    value: 0.9055
    std: 0.087
    paper_value: 0.9055
    paper_std: 0.087
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.9055
    at_pub_std: 0.087
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9055
    true_std: 0.087
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9055
    sort_std: 0.087
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.851
    std: 0.076
    paper_value: 0.851
    paper_std: 0.076
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.904
    at_pub_std: 0.078
    at_pub_source_arxiv: '2205.12245'
    at_pub_source_title: Asynchronous Neural Networks for Learning in Graphs
    at_pub_source_date_iso: '2022-05-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05300000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.904
    true_std: 0.078
    value_gap_source_arxiv: '2205.12245'
    value_gap_source_title: Asynchronous Neural Networks for Learning in Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.05300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.078
    global_rank: 170
    paper_rank: 483
    rank_delta: 313
    rank_delta_abs: 313
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PDF
    model_key: pdf
    model_plain: PDF
    value: 0.8991
    std: 0.0435
    paper_value: 0.8991
    paper_std: 0.0435
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.472
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8991
    true_std: 0.0435
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8991
    sort_std: 0.0435
    global_rank: 215
    paper_rank: 215
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: ecc
    model_plain: ECC
    value: 0.7611
    std: null
    paper_value: 0.7611
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.8944
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2021-01-20'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.13329999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8944
    true_std: null
    value_gap_source_arxiv: '2101.08170'
    value_gap_source_title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling
      and Self-Supervised Mutual Information Mechanism'
    value_gap_source_is_current_paper: false
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8944
    sort_std: null
    global_rank: 253
    paper_rank: 762
    rank_delta: 509
    rank_delta_abs: 509
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  - model: GCN^2
    model_key: gcn^2
    model_plain: GCN^2
    value: 0.8939
    std: 0.016
    paper_value: 0.8939
    paper_std: 0.016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.8939
    at_pub_std: 0.016
    at_pub_source_arxiv: '2007.08349'
    at_pub_source_title: Natural Graph Networks
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8939
    true_std: 0.016
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8939
    sort_std: 0.016
    global_rank: 272
    paper_rank: 272
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CapsGNN
    model_key: capsgnn
    model_plain: CapsGNN
    value: 0.8867
    std: 0.0688
    paper_value: 0.8867
    paper_std: 0.0688
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.8867
    at_pub_std: 0.0688
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8867
    true_std: 0.0688
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8867
    sort_std: 0.0688
    global_rank: 320
    paper_rank: 320
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AWE
    model_key: awe
    model_plain: AWE
    value: 0.8787
    std: 0.0976
    paper_value: 0.8787
    paper_std: 0.0976
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.8787
    at_pub_std: 0.0976
    at_pub_source_arxiv: '1805.11921'
    at_pub_source_title: Anonymous Walk Embeddings
    at_pub_source_date_iso: '2018-05-30'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8787
    true_std: 0.0976
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8787
    sort_std: 0.0976
    global_rank: 361
    paper_rank: 361
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.8744
    std: 0.0272
    paper_value: 0.8744
    paper_std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.8744
    at_pub_std: 0.027
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8744
    true_std: 0.0272
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8744
    sort_std: 0.0272
    global_rank: 385
    paper_rank: 385
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
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: k-GNN
    model_key: k-gnn
    model_plain: k-GNN
    value: 0.861
    std: null
    paper_value: 0.861
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.861
    at_pub_std: null
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.861
    true_std: null
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.861
    sort_std: null
    global_rank: 444
    paper_rank: 444
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PK
    model_key: pk
    model_plain: PK
    value: 0.76
    std: 0.027
    paper_value: 0.76
    paper_std: 0.027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.845
    at_pub_std: 0.006
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2014-10-13'
    value_gap_source_date_label: '2014'
    gap_vs_at_pub: 0.08499999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.845
    true_std: 0.006
    value_gap_source_arxiv: '1410.3314'
    value_gap_source_title: Propagation Kernels
    value_gap_source_is_current_paper: false
    value_gap: 0.08499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.006
    global_rank: 508
    paper_rank: 767
    rank_delta: 259
    rank_delta_abs: 259
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Propagation Kernels
    comparison_source_arxiv: '1410.3314'
    is_best: false
    is_std_outlier: false
  - model: IGN
    model_key: ign
    model_plain: IGN
    value: 0.8389
    std: 0.1295
    paper_value: 0.8389
    paper_std: 0.1295
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.839
    at_pub_std: 0.13
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.13
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.13
    global_rank: 543
    paper_rank: 548
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RW
    model_key: rw
    model_plain: RW
    value: 0.7911
    std: 0.021
    paper_value: 0.7911
    paper_std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.837
    at_pub_std: 0.015
    at_pub_source_arxiv: '2103.13125'
    at_pub_source_title: Learning Graph Representation by Aggregating Subgraphs via
      Mutual Information Maximization
    at_pub_source_date_iso: '2021-03-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-03-24'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.04589999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.837
    true_std: 0.015
    value_gap_source_arxiv: '2103.13125'
    value_gap_source_title: Learning Graph Representation by Aggregating Subgraphs
      via Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.04589999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.015
    global_rank: 553
    paper_rank: 713
    rank_delta: 160
    rank_delta_abs: 160
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Representation by Aggregating Subgraphs
      via Mutual Information Maximization
    comparison_source_arxiv: '2103.13125'
    is_best: false
    is_std_outlier: false
  - model: GK
    model_key: gk
    model_plain: GK
    value: 0.8152
    std: 0.0211
    paper_value: 0.8152
    paper_std: 0.0211
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.835
    at_pub_std: 0.006
    at_pub_source_arxiv: '2101.08170'
    at_pub_source_title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling
      and Self-Supervised Mutual Information Mechanism'
    at_pub_source_date_iso: '2021-01-20'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2022-03-15'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.01979999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.006
    value_gap_source_arxiv: '2203.07691'
    value_gap_source_title: Supervised Contrastive Learning with Structure Inference
      for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.01979999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.006
    global_rank: 559
    paper_rank: 641
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
- &id002
  dataset: PROTEINS
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.941
    std: 0.033
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.941
    sort_std: 0.033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRDL
    model_key: grdl
    model_plain: GRDL
    value: 0.826
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
    arxiv_id: '2408.11370'
    title: 'Graph Classification via Reference Distribution Learning: Theory and Practice'
    date: Aug 21, 2024
    date_display: Aug 2024
    date_iso: '2024-08-21'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.826
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8225
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.762
    std: 0.028
    paper_value: 0.762
    paper_std: 0.028
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.77
    at_pub_std: 0.03
    at_pub_source_arxiv: '2301.01642'
    at_pub_source_title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network
      for Interpretable Brain Network-Based Psychiatric Diagnosis'
    at_pub_source_date_iso: '2023-01-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.041
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.026000000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.041
    global_rank: 38
    paper_rank: 157
    rank_delta: 119
    rank_delta_abs: 119
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
    value: 0.7726
    std: 0.0228
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.05416'
    title: Semi-Supervised Hierarchical Graph Classification
    date: Jun 11, 2022
    date_display: Jun 2022
    date_iso: '2022-06-11'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 80
    sort_value: 0.7726
    sort_std: 0.0228
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PPGNN
    model_key: ppgnn
    model_plain: PPGNN
    value: 0.772
    std: 0.0473
    paper_value: 0.772
    paper_std: 0.0473
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.772
    at_pub_std: 0.0473
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.772
    true_std: 0.0473
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: 0.0473
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: IGN
    model_key: ign
    model_plain: IGN
    value: 0.7658
    std: 0.0549
    paper_value: 0.7658
    paper_std: 0.0549
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.766
    at_pub_std: 0.055
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-05-21'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.766
    true_std: 0.055
    value_gap_source_arxiv: '2505.15015'
    value_gap_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.766
    sort_std: 0.055
    global_rank: 118
    paper_rank: 123
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CapsGNN
    model_key: capsgnn
    model_plain: CapsGNN
    value: 0.762
    std: 0.036
    paper_value: 0.762
    paper_std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.763
    at_pub_std: 0.036
    at_pub_source_arxiv: '2006.09430'
    at_pub_source_title: Wasserstein Embedding for Graph Learning
    at_pub_source_date_iso: '2020-06-16'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2022-02-01'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.763
    true_std: 0.036
    value_gap_source_arxiv: '2202.00529'
    value_gap_source_title: Molecular Representation Learning via Heterogeneous Motif
      Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.763
    sort_std: 0.036
    global_rank: 148
    paper_rank: 157
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PDF
    model_key: pdf
    model_plain: PDF
    value: 0.7628
    std: 0.051
    paper_value: 0.7628
    paper_std: 0.051
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.472
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7628
    at_pub_std: 0.051
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7628
    true_std: 0.051
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7628
    sort_std: 0.051
    global_rank: 153
    paper_rank: 153
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MFN
    model_key: mfn
    model_plain: MFN
    value: 0.7618
    std: 0.0407
    paper_value: 0.7618
    paper_std: 0.0407
    metric: Accuracy
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7618
    true_std: 0.0407
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7618
    sort_std: 0.0407
    global_rank: 163
    paper_rank: 163
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
    value: 0.76
    std: 0.032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.76
    sort_std: 0.032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PSCN
    model_key: pscn
    model_plain: PSCN
    value: 0.75
    std: 0.025
    paper_value: 0.75
    paper_std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7589
    at_pub_std: 0.0276
    at_pub_source_arxiv: '1904.05003'
    at_pub_source_title: 'Semi-Supervised Graph Classification: A Hierarchical Graph
      Perspective'
    at_pub_source_date_iso: '2019-04-10'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2022-06-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.008900000000000019
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7589
    true_std: 0.0276
    value_gap_source_arxiv: '2206.05416'
    value_gap_source_title: Semi-Supervised Hierarchical Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.008900000000000019
    has_value_note: false
    value_note: ''
    sort_value: 0.7589
    sort_std: 0.0276
    global_rank: 182
    paper_rank: 275
    rank_delta: 93
    rank_delta_abs: 93
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.7568
    std: 0.005
    paper_value: 0.7568
    paper_std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7568
    at_pub_std: 0.0255
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7568
    true_std: 0.005
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7568
    sort_std: 0.005
    global_rank: 203
    paper_rank: 203
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: k-GNN
    model_key: k-gnn
    model_plain: k-GNN
    value: 0.755
    std: null
    paper_value: 0.755
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.755
    at_pub_std: null
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.755
    true_std: null
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.755
    sort_std: null
    global_rank: 216
    paper_rank: 216
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RW
    model_key: rw
    model_plain: RW
    value: 0.5957
    std: 0.001
    paper_value: 0.5957
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7422
    at_pub_std: 0.013
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2022-06-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.14649999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7422
    true_std: 0.0042
    value_gap_source_arxiv: '2206.05416'
    value_gap_source_title: Semi-Supervised Hierarchical Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.14649999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7422
    sort_std: 0.0042
    global_rank: 337
    paper_rank: 560
    rank_delta: 223
    rank_delta_abs: 223
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Capsule Convolutional Neural Networks
    comparison_source_arxiv: '1805.08090'
    is_best: false
    is_std_outlier: false
  - model: PK
    model_key: pk
    model_plain: PK
    value: 0.7368
    std: 0.007
    paper_value: 0.7368
    paper_std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.737
    at_pub_std: 0.007
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2024-10-11'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.737
    true_std: 0.007
    value_gap_source_arxiv: '2410.08524'
    value_gap_source_title: 'IGNN-Solver: A Graph Neural Solver for Implicit Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.737
    sort_std: 0.007
    global_rank: 363
    paper_rank: 370
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN^2
    model_key: gcn^2
    model_plain: GCN^2
    value: 0.7171
    std: 0.0104
    paper_value: 0.7171
    paper_std: 0.0104
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: ''
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7171
    at_pub_std: 0.0104
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7171
    true_std: 0.0104
    value_gap_source_arxiv: '2310.10434'
    value_gap_source_title: Equivariant Matrix Function Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7171
    sort_std: 0.0104
    global_rank: 464
    paper_rank: 464
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GK
    model_key: gk
    model_plain: GK
    value: 0.7139
    std: 0.003
    paper_value: 0.7139
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yang2023better
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold cross-validation
    date: Oct 16, 2023
    date_display: Oct 2023
    date_iso: '2023-10-16'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: 0.7167
    at_pub_std: 0.0055
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2022-06-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0028000000000000247
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7167
    true_std: 0.0055
    value_gap_source_arxiv: '2206.05416'
    value_gap_source_title: Semi-Supervised Hierarchical Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.0028000000000000247
    has_value_note: false
    value_note: ''
    sort_value: 0.7167
    sort_std: 0.0055
    global_rank: 470
    paper_rank: 475
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: ENZYMES
      dataset_slug: enzymes
main_figure: /figures/2310.10434/main_figure.jpegoptim.jpg
---

